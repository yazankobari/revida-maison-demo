# Revida Maison

The brand name is **Revida Maison**, with this exact casing. Both words are part of the primary logo; do not shorten the wordmark or add a full stop.

- `revida-logo.svg`: primary horizontal lockup, with the preserved perspective-frame symbol beside a two-line wordmark. The lettering uses Italiana Regular (400), the same editorial typeface as the website's large footer name. It is outlined from bundled `public/fonts/italiana.ttf`, with native kerning and equal type size on both lines. ViewBox: 524 × 184, approximately 2.85:1.
- `revida-logo.png`: transparent 1572 × 552 rendering of that SVG, used by the inspiration PDF.
- `revida-symbol.svg` and `.png`: compact symbol, reserved for space-constrained contexts where the full name is already clear.
- `revida-icon.svg` and `revida-apple-icon.png`: preserved symbol-only browser/app icons.

Use the full lockup at 44–48 px high on desktop and at least 38 px high on mobile. Keep its aspect ratio and leave clear space of at least a quarter of the symbol height. The warm stone/bronze frame colours are preserved. The standalone wordmark uses `#292824`; the inline website component inherits the surrounding text colour for light and dark surfaces.

Regenerate the SVG, matching PNG, and inline `BrandArtwork` with:

```sh
uv run --with fonttools --with uharfbuzz python scripts/generate-brand-assets.py
```

The script uses only repository assets and requires `rsvg-convert`. The logo font licence is `public/fonts/italiana-OFL.txt`. Keep Vend Sans for the website's body text and controls.
