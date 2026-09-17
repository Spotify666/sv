# sv

A website for **Sashi Vangapalli Couture**, a luxury pret and occasion couture
house in Banjara Hills, Hyderabad.

Single static page. No build step, no dependencies, no framework. Open
`index.html` and it runs.

## The idea

The house describes itself as known for "the evolution of silhouettes", and a
silhouette is a measured outline before it is anything else. So the site
documents the house the way you would document a system: a hairline grid,
monospaced annotations, garments presented as numbered plates, the commission
written out as a process. The warmth is carried by the typography and the space
rather than by decoration.

## What is in it

- **Six collection plates.** Each garment is a surface of revolution turned from
  a hand-authored profile, subdivided for smoothness, with folds modulated around
  the circumference so a skirt gathers the way cloth does. Lit with a diffuse key,
  ambient fill and a rim term, depth sorted, backface culled, drawn on canvas at
  30fps. Only plates on screen render.
- **Five stitch studies** in the journal: chain, running, cutdana, herringbone and
  couched coil, each drawing itself along its own curve.
- **An appointment form** with client-side validation and inline errors. Set
  `ENQUIRY_ENDPOINT` in `index.html` and it POSTs JSON; until then a valid request
  opens a pre-filled mail to the studio.
- **`ClothingStore` JSON-LD** carrying the real address, telephone, founding year
  and product lines.
- Mobile navigation, skip link, visible focus states, and a full
  `prefers-reduced-motion` path that disables every animation.
- Light and dark themes driven entirely by CSS custom properties.

## Typography

Cormorant Garamond for display, Jost for body, JetBrains Mono for the technical
labels. Loaded from Google Fonts.

## Photography

None is bundled. The plates fall back to generated garment studies until real
files exist. See `img/README.md` for the filenames and sizes expected.

There is also a control in the footer that loads photographs from the viewer's
own machine for demos. Those stay in that browser's local storage and are never
uploaded or shared. It is scaffolding: strip it, and the concept line in the
colophon, before this goes live as the house's own site.

## Before launch

- [ ] Supply `img/plate-01.jpg` through `plate-06.jpg`
- [ ] Add `img/og-cover.jpg` (1200x630) and uncomment the `og:image` tag
- [ ] Point `ENQUIRY_ENDPOINT` at a real form handler
- [ ] Remove the demo control and the colophon concept line
- [ ] Confirm the canonical URL and JSON-LD details with the house

## Status

An independent design concept, not an official Sashi Vangapalli Couture site and
not affiliated with or endorsed by the house. Brand details are drawn from the
label's own public profile and listings.
