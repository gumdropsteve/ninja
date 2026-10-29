# $NINJA

No Income. No Job. No Assets. Not a loan. A legend.

Launch site for $NINJA, launched on Baum on Robinhood Chain. One static file, `index.html`, with no build step.

## What's on the page

- **Hero**: the 2006 loan file, stamped APPROVED, with the contract address and buy links.
- **Live stats**: price, market cap, liquidity, 24h volume and change, from GeckoTerminal.
- **Lore**: the NINJA loan from 2004 to the 2026 launch.
- **Underwrite**: a 30-second game. Approve the true NINJAs, deny anyone who could pay.
- **Mask Desk**: a profile-picture maker. Photos stay in the browser.
- **Chart & Buy**: a 24h price chart and how to buy through Baum.

## At launch

Set the contract address at the top of the script in `index.html`:

```js
const CA = "0x…";
```

That fills in the address and copy button, points the chart links at DexScreener, and turns on the live stats and chart. Until then those show dashes and a flat placeholder line.

Check `NETWORK` (currently `"robinhood"`) against GeckoTerminal's network id for Robinhood Chain once the pool is indexed. If it's wrong, the stats stay as dashes.

## Run locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Hosting

Any static host works. For GitHub Pages: Settings → Pages → Deploy from branch → `master`, root.
