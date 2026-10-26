# Nature's Blooms — Creator Brief

Single-page interactive creator brief. One `index.html`, no build step, no backend, no external
requests — fonts, product photography and the botanical pattern are all inlined.

**Deploy:** Render → New Static Site → connect this repo.

| Setting | Value |
|---|---|
| Build command | *(blank)* |
| Publish directory | `.` |

## What's in it

- Product picker across the three flavours; selecting one re-renders payouts, bundles, claims and all four concepts
- Accent colour follows the selected flavour (`--acc`)
- Bundle cards showing which bundles contain the selected flavour, with per-sale payout
- 12 concepts across 4 angles, each with a 4-beat stepper, phone mock, shoot direction, on-screen text and full script
- Earnings calculator — sales/month × bundle share × live-price share
- Script checker against the banned-phrase list plus a results-vary check
- Pre-post checklist persisted to localStorage
- Light and dark themes, with a manual toggle

## Editing

All content lives in the `PRODUCTS`, `BUNDLES`, `BANNED`, `CHECKLIST` and `TIMELINE` objects in the
inline `<script>`. Prices and payouts are plain strings — change them there and redeploy.
