# Bracelet Product Image Suite

A source-faithful, three-skill workflow for turning one white-background bracelet photo into a coordinated four-image product set.

一个以真实产品结构为最高优先级的 Codex 三-Skill 开源套件：用一张完整白底手串图，生成统一风格的暖纸产品图、细节图与材质档案板。

## Included skills

| Skill | Purpose |
| --- | --- |
| `bracelet-product-image-suite` | Orchestrates the complete four-image workflow. |
| `tactile-paper-product-studio` | Creates warm handmade-paper editorial product images. |
| `bracelet-material-board` | Creates a tactile component/material archive board. |

The suite produces, in order:

1. one complete warm-paper product image;
2. two source-supported detail images;
3. one material-board cover using the accepted complete image.

## Design principles

- The supplied product photo is the authority for structure, color, material appearance, and camera angle.
- A single source view never authorizes an invented side, rear, or oblique view.
- Bead count, order, spacers, clasp, cord or wire routing, and natural marks must remain unchanged.
- Material names come from the user. Ambiguous materials receive neutral visual descriptions.
- Generated images must be visually checked against the source before acceptance.

## Requirements

- Codex with image generation/editing available.
- One clear, complete white-background bracelet photograph.
- All three skill folders installed together.

## Install

Clone the repository, then copy the three folders under `skills/` into your Codex skills directory.

PowerShell:

```powershell
git clone https://github.com/zuhanghu33-png/bracelet-product-image-suite.git
Copy-Item -Recurse -Force .\bracelet-product-image-suite\skills\* "$env:USERPROFILE\.codex\skills\"
```

macOS or Linux:

```bash
git clone https://github.com/zuhanghu33-png/bracelet-product-image-suite.git
cp -R bracelet-product-image-suite/skills/* ~/.codex/skills/
```

Restart or refresh Codex after installation so the skills are discovered.

## Use

Upload one complete white-background bracelet image and invoke:

```text
Use $bracelet-product-image-suite to create the complete four-image product set.
Materials: main bead ..., secondary bead ..., body beads ..., spacers ..., cord/wire ...
```

The material list is optional. When omitted, the workflow uses neutral appearance labels instead of guessing gemstone identity.

You may also invoke either supporting skill directly:

```text
Use $tactile-paper-product-studio to create a warm-paper hero image from this product photo.
```

```text
Use $bracelet-material-board to turn this product photo into a tactile material archive board.
```

## Repository layout

```text
skills/
  bracelet-product-image-suite/
  tactile-paper-product-studio/
  bracelet-material-board/
```

No private product photographs, generated customer images, or third-party style-reference images are included. Users provide their own product and optional style references at runtime.

## License

MIT License. Copyright (c) 2026 zuhanghu33-png.
