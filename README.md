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

- **No real photos are used anywhere.** Every image on the page is a coded
  placeholder (soft gradient + icon + a caption like "Add a headshot of
  Gianni"). We don't have rights to redistribute his Yelp/Facebook photos.
  Collect a headshot and 4–6 finished-piece / before-after photos from him
  directly.
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

Full sourcing notes and build decisions are also saved in the Parra Marketing
Solutions project (`claude/gianni-corvasce-build-notes.md`).
