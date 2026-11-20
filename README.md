# FoodFlow DBMS Presentation — deploy-ready static export

Source: artifact `foodflow-dbms-presentation` (24 slides, 12 working pages),
exported 2026-11-20. Single file `index.html` (103,015 bytes,
SHA-256 5bb64b088d42b901f88b2e870ce6863e589f94b500b7c0a076efc0c546ea071d).
Verified: 24 slides, no CAT-3 / CAT3 mention, no local assets, only external
dependency is Google Fonts (falls back to system fonts offline).

## What this is / is not
- This is the presentation deck only — NOT the FoodFlow Next.js app.
- The FoodFlow app is what is on GitHub at
  https://github.com/harshitshetty175-create/PRESENTO-DIGIO-DBMS.git
  (commit 6cc24c32). The presentation was never pushed there.

## Deployment routes (easiest first)
1. GitHub Pages from the same repo: push this `index.html` as
   `presentation/index.html` on `main`, then Settings → Pages → deploy from
   branch `main`, folder `/presentation`. Public URL would be
   https://harshitshetty175-create.github.io/PRESENTO-DIGIO-DBMS/presentation/
   (verify at delivery — Pages must be enabled by the repo owner / Muse via
   the GitHub connector; no Vercel, database, or secrets needed).
2. Vercel static site: import the same repo or drag this folder in; no build
   command, no environment variables. Also needs Harshit's choice/approval.
3. Render static site (like the reference deck Harshit copied the style from,
   https://dbms-cat3-presentation.onrender.com/): same single file, no build.

## What is still needed from Harshit
- Confirm he means the presentation deck (not the FoodFlow app), and pick
  route 1, 2 or 3. Route 1 is recommended: same repo, free, no new account.
- Do NOT deploy the FoodFlow app this way — it needs Vercel + live MySQL
  (Railway), a fresh AUTH_SECRET, and the demo-data-or-clean choice, all
  still open from 2026-11-19.
