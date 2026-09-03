---
name: tactile-paper-product-studio
description: Transform white-background jewelry and small-accessory photos into tactile editorial product images built from handmade paper, folded fabric, and a dark outer surface, automatically choosing a restrained scene palette from the product colors while preserving the real product. Use for bracelets, necklaces, jewelry, and small accessories; do not use for model try-ons, plain catalog cutouts, or inventing unseen product angles.
---

# Tactile Paper Product Studio

Create a brand-consistent product photograph from a user-supplied white-background product image. Keep the style grammar stable while adapting the paper, textile, and outer-background colors to the product.

## Inputs and authority

- Treat the clearest white-background product image as the authoritative product reference.
- When several real photos exist, label one as the primary angle and use the others only to verify structure or material details.
- When the user supplies a scene reference, use it only for scene, palette family, texture, lighting, and composition. Never copy its jewelry or product components.
- When no scene reference is supplied, follow the built-in style grammar below.

## Non-negotiable product preservation

Preserve the source product's exact:

- silhouette and strand count;
- component count, order, spacing, relative scale, and connection path;
- colors, stone patterns, inclusions, transparency, polish, and faceting;
- metal color, clasp type, rings, spacers, charms, cord, and other hardware.

Do not add, delete, duplicate, fuse, reshape, recolor, beautify, symmetrize, or substitute product parts. Do not turn smooth beads into faceted beads or regularize natural stone patterns.

A single view does not authorize a new viewpoint. If the user requests an oblique, side, rear, clasp, or macro view, require a real photo of that angle and use it as the primary product reference. With only one top-down photo, make only the matching top-down scene or safe crops from that view.

## Style grammar

Keep these elements stable across the series:

- tactile oatmeal or stone-toned handmade paper beneath the product;
- one folded, low-saturation textile layer framing the paper;
- a deep smoky neutral outer surface visible near the edges;
- soft directional side light, controlled highlights, and realistic contact shadows;
- restrained editorial product photography with natural texture and no glossy catalog look;
- generous negative space, no decorative clutter, no text, logo, watermark, or extra props unless requested.

The textile color is dynamic. Select it from the product colors using [references/palette-system.md](references/palette-system.md). Briefly tell the user the chosen paper, textile, and outer-background color before generation, but proceed without waiting unless the user asked to approve the palette first.

## Default composition

When the user supplies one complete white-background image and does not request another layout:

- create a 3:4 vertical hero image;
- use an approximately 90-degree overhead camera matching the source view;
- place the complete product on a centered or slightly offset handmade-paper rectangle;
- rotate the textile layer subtly beneath it and reveal the dark outer surface only at the margins;
- keep the product comfortably inside frame with about 15-25% breathing room;
- keep the whole product sharply resolved.

For a real supplied detail angle, preserve that angle and crop instead of forcing the product into the default hero layout.

## Workflow

1. Inspect every supplied product image. Identify the authoritative view, product structure, dominant and accent colors, material finish, transparency, and metal tone.
2. Write a compact invariant checklist before generating. Include exact counts for distinctive large beads, charms, strands, and clasp parts when visible.
3. Choose the scene palette with the palette reference. Favor product-background separation and low saturation over literal color matching.
4. Use the built-in image generation/editing workflow. Label inputs explicitly:
   - primary product image: structure and angle authority;
   - supporting real photos: detail verification only;
   - style reference: scene, palette family, texture, lighting, and composition only.
5. In the image prompt, repeat that only the scene and matched lighting may change. List both invariants and forbidden changes.
6. Inspect the result against the primary source. Check component count, order, clasp geometry, strand routing, main-stone shapes, surface finish, sharpness, and whether the product appears to float.
7. If one localized error remains, make one targeted correction and lock every already-correct region. Do not repeatedly regenerate the entire design to fix a small structural mistake.
8. Save accepted project outputs into the current workspace using a versioned descriptive filename. Do not overwrite earlier accepted versions.

## Acceptance criteria

Accept the result only when:

- the product is recognizably the same physical item at the supplied angle;
- every distinctive visible part has the correct count, position, shape, and material;
- the paper, textile, and outer surface form a coherent low-saturation palette that separates the product;
- the product is crisp at intended viewing size and its shadows make physical contact with the paper;
- the image contains no invented props, text, logos, watermarks, extra jewelry, or unintended UI elements.

When exact preservation cannot be verified from the available source photos, state that limitation and ask for the missing angle or detail rather than inventing it.

## Delivery

Return the image, final saved path, selected palette with a one-sentence rationale, a compact final-prompt summary, and whether the built-in or fallback image workflow was used.
