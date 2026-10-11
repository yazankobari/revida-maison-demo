# Revida Maison

The brand name is **Revida Maison**, with this exact casing. Both words are part of the primary logo; do not shorten the wordmark or add a full stop.

- `revida-logo.png`: primary logo (master). REVIDA in bronze serif capitals; the V is drawn as an outlined left arm and a tall solid swoosh, and MAISON runs across it in espresso capitals. Transparent, 1186 × 528 (about 2.25:1). The inspiration PDF uses it as is.
- `revida-logo.webp`: the same at 720 px wide, shown by the website.
- `revida-logo-light.webp` and `.png`: champagne-to-ivory version for dark surfaces (the studio).
- `revida-symbol.png`: the V alone, without MAISON. Use it where the full name is already clear or space is square.
- `revida-icon.png` and `revida-apple-icon.png`: the V on an ivory `#F3EBDD` tile, for the browser tab and the home screen.

Use the logo at 78 px high on desktop, easing to 64 px in the compact desktop header (901–1200 px wide), and 62 px on phones; never below 56 px, so MAISON stays legible. Keep its aspect ratio and leave clear space of at least a quarter of its height. On the website it casts a shadow like metal letters fixed a little off a plaster wall, lit from the top left (`svg[data-revida-logo]` in `globals.css`). Place the bronze logo on light ivory, stone or plaster surfaces, and the light version on dark ones.

Rebuild the derived files and the inline `BrandArtwork` component after replacing the master:

```sh
python3 scripts/generate-brand-assets.py
```

The script uses only repository files and requires Pillow with WebP.

## The home page opening

`public/brand/opening/` holds what the opening on the home page is made of (`src/components/OpeningCurtain.tsx`):

- `bronze-light.webp` and `maison-light.webp`: the light logo split into REVIDA and MAISON (it sits on the dark curtains), made by `scripts/generate-opening-assets.py`, which also traces the letters for the line drawing (`src/components/opening-trace.ts`).
- `curtain-velvet.webp`: a photograph of closed espresso velvet curtains, generated with Ideogram 4.5 (2560 x 1440, high quality, magic prompt off; image 3 of seed 1356440896) and prepared by `scripts/prepare-curtain-photos.py` (floor trimmed; graded from rust to espresso). The prompt: "Photorealistic interior photograph, perfectly straight-on and symmetrical: a pair of closed floor-to-ceiling heavy espresso brown velvet curtains that meet exactly in the vertical centre of the frame and fill the entire frame from edge to edge and from the top edge to the bottom edge. Deep, soft, natural vertical folds, rich dark shadows in the folds and a soft warm velvet sheen on the fold crests, lit by soft light from the upper left, the fabric just touching the floor. Deep espresso, chocolate and warm bronze-brown colours, a luxury residence. No curtain rod, no window, no wall, no furniture, no people, no text, no logo. Ultra realistic velvet pile texture, sharp focus, 50mm lens, soft diffused light."
