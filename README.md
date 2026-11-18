# Shop Passport

Turn local shopping into a collectible city adventure.

An interactive, front-end-only prototype of a city stamp-collecting app set in Bristol. No backend, no build step: every page is a single self-contained HTML file.

## Pages

| File | What it is |
|------|------------|
| `index.html` | Interactive prototype: passport, map, scan, unlock animation, achievements |
| `concept.html` | Visual direction, stamp system and AI image prompts |

## Try it

Open `index.html` in any browser. On a phone it runs full screen. Use "Add to Home Screen" for an app-like icon.

## What's in v2

- First open: choose **customer** or **merchant**, then one question per screen (Duolingo-style)
- Customer: passport cover opening animation, full-screen passport pages, next-stamp hint
- Explore: real cartoon-styled map (MapLibre + OpenFreeMap, no API key) with landmarks, partner shops, routes and a weekly district event; falls back to an illustrated map if tiles can't load
- Check-in: stamp ceremony, three-choose-one reward (two clear coupons + one mystery with a stated value range), "another stamp nearby"
- Rewards: coupon wallet with swipe-to-redeem and 4-digit code; collectible numbered stamps
- Shop pages: enamel-style feature pins, owner story, signature items, sticky Collect Stamp button
- Profile: series seals, pin badges, route postcards, seasonal skins (Christmas, Halloween, Lunar New Year)
- Merchant back office: weekly check-ins, returning customers, redemptions, coupon editing, code check
- Progress is saved in the browser; add to home screen to open full screen like an app

## Editing content

Shops, stamps and series live in two objects near the top of the `<script>` in `index.html`:

- `SHOPS`: name, area, story, map position, stamp artwork and frame colour
- `SERIES`: series names, paper colour and the seal earned for completing each one
- `PINS`: the shop feature pins and what each one means
- `ROUTES` and `WEEK`: walking routes and the weekly district event

Shop coordinates are approximate. Shop details come from our field interviews and need each owner's confirmation before launch.

## Publishing with GitHub Pages

Settings → Pages → Source: "Deploy from a branch" → Branch: `main` / root → Save.
The site appears at `https://<username>.github.io/ShopPassport/`.
