# RIVIAN — $RIVN on Robinhood Chain

Community takeover landing page for **$RIVN** on Robinhood Chain — the memecoin that took the stock's ticker. Name: Rivian. Ticker: $RIVN.

## Stack

Static, zero-build: one `index.html` with inline CSS/JS, one SVG favicon, one image.
Deploy to Vercel as a static site — no framework preset, no build command needed.

## Editing the live links

Open `index.html` and edit the `CONFIG` block near the bottom of the file:

```js
var CONFIG = {
  X_URL: "#",                                  // paste the X / Twitter profile URL
  CONTRACT: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx" // paste the contract address
};
```

Both the hero contract box (with copy-to-clipboard) and every X button on the page
read from this one place — nothing else needs to change.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole site |
| `logo.jpg` | Logo, favicon, hero image and social preview |

## Deploy

1. Push to GitHub.
2. Import the repo on Vercel.
3. Framework preset: **Other**. Build command: *none*. Output directory: `.`
