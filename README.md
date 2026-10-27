# Winx Club — Card Tracker

A free, fan-made collection tracker and checklist for the Kayou *Winx Club: Fairy Diary* collectible cards, Series 1:

- **Magic Edition** — 123 cards, 14 rarities
- **Daily Edition** — 94 cards, 9 rarities
- 62 cards are the same in both editions, so there are 155 different cards in total

Live at **https://winx-tracker.vercel.app/**

## What's in here

| File | What it is |
|------|------------|
| `index.html` | The whole app: page, styles, code and the card list. |
| `img/` | Card art as small WebP files. Shared cards have one file (e.g. `tr-001.webp`); edition-only cards start with `m-` (Magic) or `d-` (Daily). Images load lazily as you scroll. |
| `og-cover.svg` / `og-cover.png` | The share image for links on social media (1200×630). Edit the SVG, then re-render the PNG. |
| `robots.txt`, `sitemap.xml` | For search engines. Update the sitemap's `lastmod` when the page changes. |
| `vercel.json` | Cache and security headers. |

## How it's served

Plain static files on Vercel (framework preset **Other**, no build step). `index.html` is served at `/`. No server code.

## Saving

Counts and serial numbers save in the visitor's browser (local storage), keyed by card code. **Export backup** downloads a `.json` file; **Import backup** restores it and drops anything it doesn't recognise.

## Accessibility

Aims for WCAG 2.1 AA: skip link, labelled controls, every card described by name, character and code, announcements when counts or editions change, keyboard focus kept after the cards redraw, AA colour contrast, and sparkles that stop after 4 seconds (none with reduced motion).

## Not affiliated

Fan-made. Not official or affiliated with Winx Club, Rainbow or Kayou in any way. Card names and groupings come from Kayou's checklist and may not be 100% accurate.
