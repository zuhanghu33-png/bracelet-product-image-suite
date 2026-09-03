# Product-led palette system

Choose three coordinated scene colors:

1. **Paper** — the light support plane under the product.
2. **Textile** — the main adaptive color and largest visual accent.
3. **Outer surface** — the deepest quiet neutral at the frame edges.

The goal is product separation and a handcrafted editorial mood, not exact color matching.

## Decision rules

- Read the product's dominant hue, secondary accent, average lightness, saturation, transparency, and metal tone.
- Keep the paper warm-neutral and lighter than most of the product. For very pale, clear, or silver products, darken the paper slightly to retain edge definition.
- Choose a low-saturation textile that either gently complements the dominant hue or echoes a small accent color. Never use a brighter or more saturated version of the product's main color.
- Keep the outer surface deeper and quieter than the textile. It should frame the scene, not become a fourth focal color.
- Maintain obvious value separation between the product and the paper. If the product disappears into the paper, adjust the paper first, then the textile.
- For multicolor products, use a neutral textile derived from the darkest or least dominant color rather than trying to repeat every hue.
- Transparent stones need darker adjacent tones and controlled highlights; opaque dark products need a lighter paper and a warmer midtone textile.

## Starting palettes

Hex values are starting points, not fixed output requirements. Preserve the hue family and low saturation while adapting to the actual source.

| Product family | Paper | Textile | Outer surface | Intent |
|---|---|---|---|---|
| Deep blue, navy, cool black | warm stone `#C6B9A3` | tobacco/cognac brown `#6C4A3A` | smoky brown-gray `#3F3B38` | Warm-cool contrast; let blue remain premium and clear |
| Burgundy, red, pink | warm oatmeal `#CEBCA8` | muted rust/tobacco red `#75402F` | deep cocoa `#3A2F2A` | Echo the red family without becoming monochrome |
| Green, teal | warm greige `#C9BDAA` | smoked clay or muted plum-brown `#76534A` | charcoal brown `#383431` | Quiet complementary warmth |
| Purple, violet | stone beige `#C7BAA4` | muted olive-brown `#625C46` | dark mushroom `#37332F` | Balance violet with an earthy opposite |
| Yellow, amber, orange, gold | sand-beige `#C7B9A0` | smoky blue-green or charcoal taupe `#505957` | deep neutral brown `#302F2D` | Cool restraint around warm product colors |
| White, clear crystal, silver | mid stone `#B9AA94` | oxblood brown or deep cocoa `#5A3B33` | near-charcoal warm gray `#2F2C2A` | Increase edge and transparency definition |
| Black, graphite, gunmetal | light oatmeal `#D0C2AA` | camel/tobacco `#80604A` | warm charcoal `#3A3430` | Strong value separation without stark white |
| Mixed bright colors | neutral stone `#C5B9A7` | warm taupe `#665448` | quiet charcoal brown `#34312F` | Prevent the scene from competing with the product |

## Metal adjustments

- **Silver metal:** favor warmer paper and textile tones so silver reads clean rather than blue-gray.
- **Yellow gold:** avoid strong orange cloth; use smoked olive, charcoal taupe, or subdued blue-green.
- **Rose gold:** use mushroom taupe, muted cocoa, or smoked plum rather than saturated pink.
- **Mixed metal:** make the textile neutral and let the paper carry the warmth.

## Avoid

- pure white paper behind clear or silver products;
- pure black outer backgrounds with crushed shadows;
- bright orange, bright red, or saturated complementary cloth;
- matching the textile exactly to the dominant product color;
- more than one strong textile color in the same image;
- color casts that alter the product's true material color.

## Palette statement format

Before generation, state the decision in one line:

`布料：<颜色/近似色>；纸张：<颜色/近似色>；外背景：<颜色/近似色>。理由：<产品分离或呼应关系>。`
