# Golden Wishes — React + Vite

A starter website for free digital greeting cards, in English, responsive for desktop and mobile.

## Run locally

1. Open this folder in VS Code.
2. Open the terminal and run `npm install`.
3. Run `npm run dev` and open the local address shown by Vite.
4. Run `npm run build` to create the production `dist` folder.

## Deploy for free on Cloudflare Pages

1. Create a GitHub repository and upload the files from this project (do not upload `node_modules`).
2. In Cloudflare dashboard → Workers & Pages → Create → Pages → Import Git repository.
3. Choose the repository, framework **React (Vite)**, build command `npm run build`, output directory `dist`.
4. Deploy. You will receive a `*.pages.dev` URL.

## Add or replace cards

- Put optimized card thumbnails in `public/cards`.
- Put actual GIF/MP4 files in `public/cards`.
- Edit the `cards` array near the top of `src/main.jsx`.
- Set `ready:true` only when the download is real and available; otherwise `ready:false` shows “Coming soon”.
- Existing starter files are examples based on user-provided media. Check licenses and verify animations before publication.

## Before publishing

- Replace `hello@example.com` in `src/main.jsx` with your real contact email.
- Choose a final brand name, and update text in `index.html`.
- Review each downloadable file and check it is intended to be given away for free.
- Create Privacy Policy, Terms of Use and contact pages before seeking ad monetization. Add consent management where required.
- Google Search Console: verify the live site, then request indexing and submit a sitemap (add real canonical URLs after deployment).
- **SEO limitation:** this is a client-rendered React SPA; individual card pages and prerendered HTML are a recommended next step for search traffic. Do not expect Google traffic simply from publishing.
- **Ads are not configured:** monetization requires separate approval and compliance with an ad network's policies.

## Technical notes

- No paid API, database, account, or subscription required.
- Favorites only last until the page is refreshed. The search and category filters work locally.
- “Coming soon” images are illustrative previews, not downloadable cards.
