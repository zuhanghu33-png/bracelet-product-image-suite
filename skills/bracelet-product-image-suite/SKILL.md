---
name: bracelet-product-image-suite
description: "Turn one white-background bracelet product photo into a coordinated four-image set by orchestrating Tactile Paper Product Studio and Bracelet Material Board: one complete warm-paper product image, two source-faithful detail images, then one material-board cover built from the accepted complete image. Use for a repeatable one-upload bracelet product-image workflow; do not invent unseen viewpoints or materials."
---

# Bracelet Product Image Suite

Create exactly four accepted vertical 3:4 PNGs from one clear, complete white-background bracelet product photo:

1. warm-paper complete product image;
2. warm-paper detail A;
3. warm-paper detail B;
4. Bracelet Material Board cover using image 1 as its unchanged left print.

Before generating, load and follow `$tactile-paper-product-studio`, its palette reference, `$bracelet-material-board`, and the installed image-generation workflow. If either product skill is unavailable, stop and identify the missing skill.

## Input and authority

- Require one clear white-background photo showing the complete bracelet. Ask for one only when it is missing or the product is materially cut off.
- Treat the white-background photo as the product identity and structure authority for all four outputs.
- If the user supplies more real angles or close-ups, use them only for the corresponding visible angle or detail.
- Treat accepted generated images as composition inputs, never as authority for hidden product structure.
- Do not ask for a material list by default. When names are absent, use neutral visible descriptions and never invent gemstone identity, origin, grade, treatment, or metal purity.

A single photo does not authorize a new camera viewpoint. Detail images are close crops from visible, source-supported regions at the supplied viewpoint, not invented side, rear, oblique, or macro views.

## Run the workflow

Briefly state that the run uses four image edits and has a checkpoint after the three warm-paper images. Proceed without waiting unless the user asks to approve the palette or pause at the checkpoint.

### 1. Lock the product and palette

Inspect the white-background photo and record a compact invariant checklist: overall form, strand count, visible component sequence, distinctive beads, spacers, charms, clasp, cord or wire, colours, transparency, finish, and natural marks. Count distinctive large or unique parts when visible.

Choose the paper, textile, and outer-surface palette once with the Tactile Paper Product Studio palette system. Reuse it unchanged across images 1-3. State the chosen palette in one line before generation.

### 2. Generate the three warm-paper images

Generate each image from the original white-background photo as the primary product reference. Use the accepted complete image only as a palette, lighting, and scene-consistency reference for the detail images.

- **Image 1 — complete:** Follow the Tactile Paper Product Studio default complete-product composition. Keep the entire bracelet visible with about 15-25% breathing room.
- **Image 2 — detail A:** Make a safe close crop of the most distinctive visible focal region, such as a signature bead, charm, central motif, or unusual material transition. Keep enough surrounding sequence to verify its location.
- **Image 3 — detail B:** Make a different, non-duplicative safe close crop of visible construction or hardware, such as the clasp, knot, spacer sequence, cord or wire connection. If no such feature is visible, use the second most informative source-supported component region.

Keep all three at the supplied camera viewpoint and in the same 3:4 warm-paper visual family. Do not add text, props, logos, watermarks, extra jewelry, or unseen microtexture. Do not enlarge a crop beyond what the source can support without inventing detail.

After each image, compare it with the white-background authority. Reject changes to component count, order, geometry, colour, surface, clasp, cord routing, or strand structure. Use at most one targeted correction for a localized error; lock already-correct regions and avoid full regeneration for a small defect.

### 3. Checkpoint

Accept the warm-paper set only when image 1 shows the complete product and images 2-3 show two distinct, source-supported regions with consistent palette and lighting. Continue automatically to the cover unless the user requested a pause.

### 4. Generate the Material Board cover

Run `$bracelet-material-board` with:

- **primary display input:** accepted image 1, placed unchanged as the complete left physical print;
- **verification input:** the original white-background photo, used only to check bracelet structure and visible component truth;
- **right-side samples:** only components visible in the source or explicitly named by the user.

Keep the cover vertical 3:4. Preserve image 1's complete pixels and crop inside the left print; only uniformly scale it and add the permitted paper border, tape, and mild whole-print integration. When no material list was supplied, use short neutral appearance labels or omit a label that would require guessing. Never infer a named mineral from appearance alone.

Verify that the cover retains the accepted complete warm-paper image at left and that every right-side sample corresponds to a real visible bracelet component. Do not let labels, tape, or samples cover the product.

## Save and deliver

Save accepted files in the current workspace, never only in the generated-image cache. Use one product-specific folder and these ordered names:

```text
output/bracelet-product-image-suite/<product-name>/
  01-warm-paper-complete-v1.png
  02-warm-paper-detail-a-v1.png
  03-warm-paper-detail-b-v1.png
  04-material-board-cover-v1.png
```

Do not overwrite accepted versions; increment the version suffix. Return all four images together with their saved paths, the shared palette, any source limitation, and whether a targeted correction was used.

## Acceptance contract

- Exactly four final images are delivered in the required order.
- All outputs depict the same physical bracelet and preserve source-supported structure.
- Images 1-3 share one palette and visual system; image 1 is complete and images 2-3 are distinct truthful details.
- Image 4 uses accepted image 1 unchanged as the left print and does not invent material claims.
- A single source view never becomes a fabricated new viewpoint.

