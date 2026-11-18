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

## Editing content

Shops, stamps and series live in two objects near the top of the `<script>` in `index.html`:

- `SHOPS`: name, area, story, map position, stamp artwork and frame colour
- `SERIES`: series names and the seal earned for completing each one

## Publishing with GitHub Pages

Settings → Pages → Source: "Deploy from a branch" → Branch: `main` / root → Save.
The site appears at `https://<username>.github.io/ShopPassport/`.
