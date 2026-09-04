# RIVIAN — $RIVN on Robinhood Chain

Community takeover landing page for **$RIVN** on Robinhood Chain — a stock-paired memecoin quoted in the tokenized RIVN stock token. Name: Rivian. Ticker: $RIVN.

Section 02 describes the real stock-pairing mechanic on Robinhood Chain (stock token as quote asset, float locked in the pool, mint-only-by-authorised-party ceiling). The figures and the BONER/HIMS episode cited there are sourced and dated in the footnote — update or drop them if they go stale.

## Stack

Static, zero-build: one `index.html` with inline CSS/JS, one SVG favicon, one image.
Deploy to Vercel as a static site — no framework preset, no build command needed.

## Editing the live links

Open `index.html` and edit the `CONFIG` block near the bottom of the file:

```js
var CONFIG = {
  X_URL:        "https://x.com/rivianctorh",
  CONTRACT:     "0x6f2eaa...",  // token contract
  ANSEM_WALLET: "0xB2b7E6...",  // creator-reward + 11.15% supply recipient
  EXPLORER:     "https://robinhoodchain.blockscout.com"
};
```

Both the hero contract box, the Ansem proof block (address, copy button, explorer link) and every X button on the page
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
