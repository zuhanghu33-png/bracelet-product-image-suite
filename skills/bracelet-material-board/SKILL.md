---
name: bracelet-material-board
description: Transform a user-supplied bracelet product photo into a tactile editorial material board with the unchanged full product image at left and physical bead, spacer, charm, and cord samples at right. Use for bracelet material stories, bead reference boards, jewelry concept presentations, and handcrafted product-content images; do not use for fashion outfits or generic jewelry catalog layouts.
---

# Bracelet Material Board

Create a vertical, photographed physical archive board that preserves the supplied bracelet product photo as a printed image at left and presents the bracelet's real component materials as tactile samples at right. Keep the warm paper, torn tape, handwritten studio-note, and restrained editorial character of a hand-assembled material board. Do not reinterpret it as a fashion board, ecommerce infographic, or jewelry tray.

## Require product references

Require at least one user-supplied bracelet product photo before generating.

- If no product photo is available, ask: `请先上传一张完整、清晰的手链产品拍摄图。`
- Prefer a photo showing the complete bracelet. Preserve a partial crop when that is all the user supplied; never invent the hidden portion.
- If multiple photos are supplied, choose the clearest complete product photo for the left print and use additional close-ups only to understand component appearance.
- Treat style references as layout guidance only. Ignore phone status bars, player controls, black margins, watermarks, and other screenshot UI.

Exact gemstone or material identity cannot be established reliably from appearance alone. Use user-provided material names as the source of truth. If the user requests named labels but has not supplied the materials and the image is ambiguous, ask for the bead and hardware material list. If they do not know it, use neutral visual labels such as `translucent tea-brown stone` instead of inventing a mineral, treatment, origin, grade, or certification.

## Lock the bracelet and source photo

The left image is the user's actual product photograph placed as a physical print, not loose inspiration for a new bracelet render.

- Preserve the bracelet's exact overall form, bead count, sequence, bead shapes, diameters and relative scale.
- Preserve bead colour, translucency, lustre, polish, banding, grain, pores, inclusions, cracks, carving, holes, and other source-supported marks.
- Preserve every spacer, cap, charm, pendant, clasp, knot, elastic, cord, tassel, logo, and their exact positions.
- Preserve the source camera angle, perspective, crop, lighting, background relationship, shadows, and colour balance.
- Do not add, remove, duplicate, reorder, resize, recolour, replace, clean up, or redesign any product component.
- Do not retouch away natural variation or make all beads artificially identical.
- Limit treatment of the embedded photo to uniform scaling, non-destructive placement, a paper border, subtle print sheen, and very mild whole-photo tonal integration.
- Keep tape, notes, samples, and shadows outside the bracelet and its important details.

Before handoff, compare the embedded print against the source. If the bracelet structure or any identifying component changed, correct the image before presenting it.

## Build the board

Default to one vertical 3:4 board unless the user requests another ratio.

1. Use a warm ivory or off-white wall or tabletop with soft natural side light and restrained contrast.
2. Allocate about 40% of the width to the left product print and 60% to the right material sheet. Keep both elements fully visible with breathing room.
3. Print the complete bracelet photo on warm-white matte paper. Attach it with two small torn strips of aged cream masking tape at the paper edges.
4. Place a separate cream, uncoated, deckle-edged paper sheet at right.
5. Arrange 4-6 physical component groups derived only from the actual bracelet. Use one to three loose beads per group, a short source-supported bead sequence, or one real spacer, charm, or cord sample. Samples rest on the paper with believable contact shadows; they never float.
6. Make the primary bead group largest near the upper right. Place secondary beads through the middle and hardware, charm, cord, or knot details near the lower right. Allow restrained overlap without obscuring material features.
7. Add sparse, small dark-brown or black handwritten workshop labels. Default to short English labels because image models render short text more reliably; use another language only when the user asks.

## Render material truthfully

Describe each component as `verified material or neutral identity + colour + transparency + surface + internal or structural feature`.

Show only source-supported properties:

- Stone or glass: translucency, colour bands, clouds, inclusions, fractures, internal highlights, polish, and edge glow.
- Wood or seed beads: pores, vessels, grain, pits, uneven skin, carving, and patina.
- Metal: colour, engraving, hammer marks, oxidation, plating, brushed or polished finish, and softened reflections.
- Cord or elastic: fibre twist, weave, thickness, knot construction, and matte or waxed finish.
- Ceramic, shell, resin, or composite materials: glaze, nacre, mould lines, grain, embedded particles, and surface wear only when visible or verified.

Do not imply rarity, healing effects, authenticity, origin, treatment, grade, or precious-metal purity without user-provided evidence.

## Visual language

- Near-overhead tactile flat-lay photography, vertical 3:4.
- Warm daylight, gentle cast shadows, quiet cream, grey, brown, and product-derived accent colours.
- Matte paper fibres, torn tape ends, slight wrinkles, deckle edges, minor curl, and imperfect hand placement.
- Real three-dimensional beads and hardware with scale cues and contact shadows, never flat circular colour chips.
- Restrained 1990s-2000s editorial archive sensibility: minimal, tactile, calm, and premium without glossy advertising polish.
- Handwritten notes remain secondary and may be softly imperfect. Never let text dominate the board.

## Generation brief

For raster creation or editing, follow the installed image-generation workflow and use the product photo as the primary reference image. Build the generation instruction in this order:

```text
Edit the supplied bracelet product reference into a realistic editorial bead-material archive board photographed from above. Use the original product photo as the unchanged printed image at left. Preserve the exact bracelet form, bead count and order, bead sizes, shapes, colours, translucency, natural marks, holes, spacers, charms, knots, cord, camera angle, crop, lighting, and shadows; do not redraw or redesign the product.

Generate only the surrounding hand-assembled flat lay: a warm ivory ground, matte product print fixed with two small torn cream masking-tape strips, and a deckle-edged cream material sheet at right. Arrange 4-6 real three-dimensional component groups at right using only these verified materials or neutral visual descriptions: [USER MATERIAL LIST]. Show one to three beads or one source-supported hardware or cord sample per group, realistic scale, tactile microtexture, natural contact shadows, restrained overlap, sparse small handwritten workshop labels, soft side daylight, muted archival jewelry styling, vertical 3:4.

No clothing, fabric swatches, model, jewelry box, display tray, grid, catalogue, exploded diagram, ecommerce infographic, logo, price, large typography, invented material names, extra beads, altered product components, phone UI, player controls, or black screenshot borders.
```

If the user supplied exact annotation text, use it. Otherwise derive concise labels from verified materials or neutral visible descriptions. Keep labels to roughly two to five words.

## Final checks

Verify before returning the image:

- The left print retains the supplied product photo and complete bracelet identity.
- Bead count, order, proportions, spacers, charms, knots, and cord remain unchanged.
- Every right-side sample corresponds to an actual component or user-verified material.
- Unknown materials use neutral descriptions rather than confident gemstone claims.
- Samples are physical beads or components, not fabric squares or flat colour chips.
- The board reads as a tactile handmade archive, not a digital collage or product listing.
- No screenshot interface, excessive props, large text, or invented brand content appears.

