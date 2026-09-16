# Gianni Corvasce Restoration — Website Mockup

A single-page pitch/demo site for **Gianni Corvasce Restoration**, a furniture
repair and restoration studio in Berkeley, CA (2703 Seventh St, ActivSpace).
Built by Parra Marketing Solutions as pre-outreach demo collateral — this
business hasn't been contacted yet and has no live website of its own.

## What's in this repo

- `index.html` — the entire site (nav, hero, about, services, gallery,
  reviews, hours/location, contact, footer). No build step, no dependencies
  beyond Google Fonts — just a static file.

## Deploying with GitHub Pages

1. Push this repo to GitHub (see commands below if you haven't already).
2. In the repo, go to **Settings → Pages**.
3. Under "Build and deployment," set **Source: Deploy from a branch**.
4. Set **Branch: `main`**, folder **`/ (root)`**, then **Save**.
5. GitHub will publish it at `https://<your-username>.github.io/<repo-name>/`
   within a minute or two.

```bash
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

## Before this becomes Gianni's real, live site

This is a **mockup** built from public information (Yelp, Facebook, and
directory listings), not from an intake call with the business owner. Before
publishing it as his actual site:

- **Real photos are now used in the gallery, as of 2026-09-15.** Update:
  the user initially supplied 11 photos of finished pieces (a secretary
  desk, live-edge table, sideboard, tansu cabinet, art deco pieces, an
  Eames-style chair, a guitar, etc.) and first said they'd been pulled from
  Yelp/Google/social — at that point they were withheld, since files-in-hand
  doesn't equal redistribution rights. The user then clarified these are
  **Gianni's own photos of his own finished work**, publicly posted by him
  (not a customer's or a third party's), and explicitly directed they be
  used, specifically because this mockup is going straight back to Gianni
  himself as a pitch ("I made a mockup using photos you already have out
  there"). On that basis, 9 of the 11 are now in `images/` and used across
  the gallery grid and the two before/after slider "after" panels (see
  build notes for the exact mapping). Two things still don't have a real
  photo: **a headshot of Gianni** (none of the 11 are one), and genuine
  **"before" (damaged/pre-restoration) shots** — the sliders pair a real
  finished photo against a placeholder "before" panel for exactly that
  reason, clearly labeled as such on the page.
  **Before this goes further than a private pitch to Gianni himself** (i.e.
  before it's ever published as his actual public site), it's still worth
  getting his explicit yes on reusing these specific photos, even though
  they're his own and already public — that's a quick ask once he's
  responded to outreach, not a blocker on sending him the pitch.
- **One genuine before/after pair added**, same day: a double dresser,
  original brown wood finish → refinished in black lacquer with new brass
  pulls. Found among an earlier upload batch in this session tied to
  Gianni's Yelp business photos (a screenshot of his Yelp "Photos and
  videos" tab, which has a dedicated "Before & After (3)" category, was
  also uploaded around the same time). Cropped the phone-Photos-app UI
  chrome out of both shots before use. This is the only fully real
  before/after on the page — the other two sliders still pair a real
  "after" against a placeholder "before."
- **Broadened positioning:** the mockup now frames Gianni as full-service
  ("furniture, cabinetry, doors, and specialty pieces") rather than
  furniture-only, and adds a "Specialty & Instrument Pieces" service card
  plus a real guitar-restoration gallery photo. This is based on the user
  reporting they'd seen a guitar restoration photo among Gianni's work —
  **unverified beyond that**, same caveat as "Since 1989" below. Confirm at
  intake how often he actually takes on instrument/specialty work before
  making it a headline claim rather than a mentioned capability.
- **Address discrepancy:** Yelp lists 50 West Hornet Ave, Alameda, CA; every
  other source (Facebook, Manta, Google Maps, Yellow Pages, Cylex) lists
  2703 Seventh St, Berkeley (ActivSpace), which is what this mockup uses.
  Confirm which is current.
- **Hours** vary by source. The mockup uses "By appointment" as an honest
  default — get his real schedule.
- **"Since 1989"** is not used anywhere in the copy — it only appears on an
  unclaimed, self-submitted Manta listing and isn't confirmed.
- Reviews quoted on the page are real, attributed Yelp reviews (4.9★ / 44
  reviews) — verify he's comfortable with them being reproduced before this
  goes live, and swap in Google reviews too if he'd like (he separately shows
  5.0★ on Google Maps).

- **Hero photo swapped for a sharp one, sliders rebuilt (2026-09-15).** The
  hero previously used a 348×348 Yelp-thumbnail photo stretched to ~650px
  wide, which looked visibly blurry. Replaced it with a higher-resolution
  (750×1000) photo of the live-edge table found in an earlier upload, cropped
  and now displayed *smaller* than its native size — it's a downscale, not
  an upscale, so it stays sharp. The before/after sliders also got rebuilt:
  they used to rely on a native `<input type="range">`'s own touch/drag
  handling, which turned out to be unreliable once the input was stretched
  invisibly across the whole frame; they now use explicit pointer-event
  handling (works the same for mouse, touch, and keyboard), verified with a
  real simulated touch-drag, not just a mouse test.

- **Typography scaled up across the whole page (2026-09-16).** Base body
  text, headings, nav, buttons, captions, review copy, and footer text were
  all bumped to a larger size (body text 16px → 18px, hero headline up to
  ~4.5rem at wide widths, section headings, stat numbers, and review quotes
  all increased proportionally) for better readability and more visual
  weight, per request. Layout, spacing, and responsiveness were re-checked
  after the change — everything still fits and wraps cleanly.

- **Down to one before/after example (2026-09-16).** The two placeholder
  sliders (Extension Dining Table, Burl Coffee Table — each pairing a real
  "after" photo with a generic icon "before" panel) were removed per
  request, leaving only the one genuine, fully-photographed example: the
  double dresser.
- **Slider replaced with a plain static before/after (2026-09-16, same
  day).** The drag-to-compare interaction was dropped entirely per request
  in favor of a simple side-by-side layout — a "Before" panel, an arrow
  graphic, and an "After" panel, no JavaScript interaction required. This
  removes any dependency on pointer/touch event support in whatever browser
  or embedding surface displays the page.

Full sourcing notes and build decisions are also saved in the Parra Marketing
Solutions project (`claude/gianni-corvasce-build-notes.md`).
