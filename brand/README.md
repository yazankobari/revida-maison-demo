# Revida Maison

The brand name is **Revida Maison**, with this exact casing. Both words are part of the primary logo; do not shorten the wordmark or add a full stop.

- `revida-logo.svg`: primary wordmark (master). Each letter of REVIDA is a piece of furniture drawn as a single line: shell-chair R, writing-desk E, side-chair V, floor-lamp I, framed D, trestle A. A bronze inlay `#9A7E5A` fills every stroke inside an espresso outline `#3A302A`; MAISON is hand-lettered with a brush pen and sits centred beneath in espresso. ViewBox: −4 0 886 × 282, approximately 3.14:1.
- `revida-logo.png`: transparent 1572 × 500 rendering of the wordmark, used by the inspiration PDF.
- `revida-symbol.svg` (master) and `.png`: the R chair, a chair whose back post, armrest, seat and front leg form the letter R. Espresso frame with a bronze seat. Use it where the full name is already clear or space is square.
- `revida-icon.svg` and `revida-apple-icon.png`: the R chair on an ivory `#F3EBDD` tile, for the browser tab and the home screen.

Use the wordmark at 56 px high on desktop, easing to 46 px in the compact desktop header (901–1200 px wide), and 44 px on phones; never below 40 px, so MAISON stays legible. Keep its aspect ratio and leave clear space of at least a quarter of its height. The colours are fixed: place the logo on light ivory, stone or plaster surfaces only.

Rebuild the PNGs, icons and the inline `BrandArtwork` component after editing either master:

```sh
python3 scripts/generate-brand-assets.py
```

The script uses only repository files and requires `rsvg-convert`.
