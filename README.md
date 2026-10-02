# Speed website

The marketing site at https://myspeedapp.com. Plain HTML, CSS and JavaScript
with no build step: `index.html`, `styles.css`, `main.js` and `assets/`.

## Run locally

Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

## Deploy

Hosted on Cloudflare Workers (static assets) in the developers@myspeedapp.com
account, project `speed-website`. Every push to `main` builds and deploys.
Manual deploy from a machine logged in with `npx wrangler login`:

```
npx wrangler deploy
```

`wrangler.jsonc` holds the Worker config; `.assetsignore` lists the files the
Worker must not serve.
