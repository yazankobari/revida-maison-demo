# Revida Maison

The brand name is **Revida Maison**, with this exact casing. Both words are part of the primary logo; do not shorten the wordmark or add a full stop.

- `revida-logo.png`: primary logo (master). REVIDA in bronze serif capitals; the V is drawn as an outlined left arm and a tall solid swoosh, and MAISON runs across it in espresso capitals. Transparent, 1186 × 528 (about 2.25:1). The inspiration PDF uses it as is.
- `revida-logo.webp`: the same at 720 px wide, shown by the website.
- `revida-logo-light.webp` and `.png`: champagne-to-ivory version for dark surfaces (the studio).
- `revida-symbol.png`: the V alone, without MAISON. Use it where the full name is already clear or space is square.
- `revida-icon.png` and `revida-apple-icon.png`: the V on an ivory `#F3EBDD` tile, for the browser tab and the home screen.

Use the logo at 78 px high on desktop, easing to 64 px in the compact desktop header (901–1200 px wide), and 62 px on phones; never below 56 px, so MAISON stays legible. Keep its aspect ratio and leave clear space of at least a quarter of its height. Place the bronze logo on light ivory, stone or plaster surfaces, and the light version on dark ones.

Rebuild the derived files and the inline `BrandArtwork` component after replacing the master:

```sh
python3 scripts/generate-brand-assets.py
```

The script uses only repository files and requires Pillow with WebP.
