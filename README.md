# FreshTrace Bio — Final Prototype

A full static prototype for the FreshTrace Bio smart food freshness monitoring platform.

## Included
- Premium dark biotech UI inspired by the provided Home and Analytical references
- Consistent UI across Home, Dashboard, Register, Packages, QR, Scan, Analytical, Research and public freshness report
- Product-specific QR with package ID + batch + company/product metadata in the report URL
- QR generator with download, print and copy-link actions
- Public `/scan/<packageId>` hash route for direct freshness reports
- Demo packages: Fresh / Early Spoilage / Moderate Spoilage
- pH, temperature, gas index, food condition, sticker colour and expected expiry
- Animated Home biosensor panel that changes colour, pH and temperature
- Analytical page with shelf-life, TVB-N, microbial growth and pH trend visuals
- Demo sensor simulation on package details
- LocalStorage persistence

## Run locally

From this folder:

```bash
python -m http.server 8000
```

Open:

`http://localhost:8000/index.html#home`

## Routes
- `#home`
- `#dashboard`
- `#register`
- `#packages`
- `#qr`
- `#scan`
- `#analytics`
- `#research`
- `#settings`
- `#scan/PKG-2026-00001`
- `#packages/PKG-2026-00001`

## QR / mobile camera note
For a normal phone camera to open the QR destination, deploy the site to a public HTTPS URL. Then set the **Public Base URL** in Settings to that deployed URL before generating printed QR labels.

## Scientific note
The pH, temperature, gas and freshness values in demo mode are interface calibration examples, not validated food-safety thresholds. Replace them with experimentally measured and validated data for research or competition claims.
