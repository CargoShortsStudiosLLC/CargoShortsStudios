# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

- **Magic: The Gathering Commander players** who find an app (Commander Crush today) through a store listing, a community post or a search. They want to know quickly what it does, whether it's free and safe, and where to get it.
- **Store reviewers and platforms** (Apple App Review, Google Play, ad networks) checking the privacy policy, terms, support contacts, data-deletion instructions and `app-ads.txt`. These pages must be easy to find, stable and accurate.
- **Partners, press and potential hires** sizing up the studio. They need a credible, legitimate small company, not a pitch.

Existing app users looking for support are served too, but they weren't named as a primary audience.

## Product Purpose

The site is the public home of Cargo Shorts Studios LLC, a small software studio in Minnesota that makes apps for tabletop and card game players. It exists to:

1. explain each app and send players to the right store,
2. host the legal and support pages that app stores and platforms require,
3. show that a real, accountable company stands behind the apps.

The site is working when a Commander player understands an app and installs it, when a reviewer finds every required page on the first try, and when an outsider leaves thinking "small, real, careful studio".

## Positioning

The site is a quiet umbrella. The studio stays in the background, each app gets its own page, and the apps are the stars. The site should grow by adding app pages, not by building up a big studio brand.

## Operating Context

- Visitors usually arrive straight on an app page or a legal URL from a store listing, and often on a phone.
- The legal pages (`/commandercrush/privacypolicy/`, `/commandercrush/tos/`) are copies of the source documents in the `commander_crush` repo's `docs/`. They're re-rendered when those documents change and are never edited here.
- Search console and canonical/sitemap hygiene matters (`sitemap.xml`, `robots.txt`, canonical tags).

## Capabilities and Constraints

- Plain static HTML/CSS with one shared `style.css` and no build step. It's deployed to GitHub Pages from the repo root on every push to `main`.
- Pages: studio home (`index.html`), Commander Crush (`commandercrush.html`), Support (`support/`), and the Commander Crush Privacy Policy and Terms of Service.
- Light and dark modes follow the system setting (`prefers-color-scheme`).
- Required to stay: `app-ads.txt` at the root, working store links, support and legal email addresses, and the Wizards of the Coast Fan Content Policy disclaimer on Commander Crush surfaces.
- **Commander Crush facts:** free, rated 13+, no account needed, on Google Play (`com.cargoshortsstudios.commandercrush`) and the App Store (id6812471605). Data deletion is in the app under Settings → Delete my data.
- **Open:** the Details table on the Commander Crush page still lists Status as "Available on Google Play", even though the App Store badge now links to the live listing. Confirm the wording before changing it.

## Brand Commitments

- Name: **Cargo Shorts Studios** (legal entity Cargo Shorts Studios LLC). Assets: `assets/logo.svg`, `assets/icon.svg`.
- App name: **Commander Crush**. Assets: `assets/commander-crush-icon.png` and the store screenshots in `assets/commander-crush/`.
- Commander Crush is unofficial Fan Content, not approved or endorsed by Wizards. Never imply affiliation with Wizards of the Coast, and never use Wizards' trademarks as decoration.
- Official store badges (Google Play, App Store) must follow each platform's badge guidelines.
- **Voice:** playful, wry and nerdy everywhere (studio, app and support pages), in the spirit of the "Hot singles in your commander deck?" line. The exception is the **Privacy Policy and Terms of Service**, which stay plain, precise and joke-free.

## Evidence on Hand

- Three real Commander Crush screenshots: `assets/commander-crush/01-deck.webp`, `02-detail.webp`, `03-alt-art.webp`.
- Live store listings on Google Play and the App Store.
- There are no testimonials, reviews, ratings, download counts, press quotes or customer logos. Don't make any up.

## Product Principles

1. **Apps first, studio second.** Every page should help someone understand or get an app. The studio is the trustworthy byline, not the headline.
2. **Compliance pages are part of the product.** Legal, support and data-deletion information is always one click away, accurate and kept in sync with its source.
3. **Fun where it's earned, plain where it counts.** Jokes and personality go wherever they help; legal text stays dead straight.
4. **Only claim what's true.** No made-up proof, no implied Wizards endorsement, and no platform claims that the stores don't back up.
5. **Small and fast.** Static pages and no dependencies beyond what a page actually needs. Easy to add the next app.
