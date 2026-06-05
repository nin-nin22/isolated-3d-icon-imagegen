---
name: isolated-3d-icon-imagegen
description: Generate or plan prompts for isolated isometric 3D icon images using the bundled samples. Use for アイソレ画像, isometric icons, 3D isolated objects, smooth soft 3D commercial icons with slight clay-art softness, or sample-matched icon images from a theme or object.
---

# Isolated 3D Icon Imagegen

## Overview

Use this skill to create isolated isometric 3D icon images or the prompts for them. The target style is defined by the approved images in `samples/`: white or very light gray background, one isolated object or compact group, three-quarter top-down perspective, rounded simplified forms, smooth soft 3D model surfaces, slight clay-art softness, soft studio lighting, and subtle contact shadows.

This skill controls style and prompt quality. Use the available image generation workflow/tool for actual image creation.

## Trigger

Use this skill when the user asks for:

- `アイソレ画像`
- `isometric icon`, `isometric 3D icon`, or `3D isolated object`
- A soft 3D icon/image for a product, person, animal, food, gadget, ecommerce, logistics, home, office, SNS, or marketing concept
- An image that should match the bundled `samples/` style

## Workflow

1. Identify subject, count, relationship between objects, required colors, background, and aspect ratio.
2. Inspect only the closest `samples/` image(s) when visual matching matters:
   - Baseline object/material: `pencil.png`, `stainless-tumbler.png`, `knife-cutting-board.png`
   - Gadgets/devices: `mx-master4-mouse.png`, `keyboard-mouse.png`, `mechanical-keyboard-black.png`, `open-silver-laptop.png`, `black-smartphone-screen-on.png`
   - Furniture/interior objects: `office-chair-black.png`, `standing-desk-white.png`, `wooden-side-table-natural.png`, `black-floor-lamp.png`
   - People/groups: `construction-worker.png`, `mother-kindergarten-boy.png`, `business-person-suit-male.png`, `casual-woman-tshirt-jeans.png`, `young-man-casual-waving.png`
   - Animals/plants/food: `seated-shiba-inu.png`, `standing-black-cat.png`, `sansevieria-potted-plant.png`, `pizza-cola.png`, `simple-white-coffee-cup.png`
3. Choose a compact composition: single centered object by default; related subjects become one compact isolated group; use grids only for explicit sets.
4. Write the final prompt in English. Preserve Japanese text only when the user explicitly requests visible text.
5. Generate with the image tool, then revise using the QA checklist if needed.
6. If the result is project-bound, copy the final image into the requested project folder.

## Core Style

Always include:

- White or very light gray background, no room or real scene.
- Isolated object or compact group with generous whitespace.
- Three-quarter top-down isometric view.
- Rounded simplified geometry that remains recognizable.
- Smooth soft 3D display-model material with slight clay-art softness, not handmade clay.
- Soft ambient studio lighting and subtle contact shadow.
- Clean commercial app/marketing icon quality.

Materials:

- Plastic/shells: smooth soft plastic, broad soft highlights, low surface noise.
- Metal: flat satin, low contrast, broad soft highlights; no chrome, mirror reflection, sparkle, or noisy brushed streaks.
- Wood: warm simplified wood, subtle smooth grain only when recognition needs it.
- Glass/liquid/screens: simplified translucency or soft glow; no photorealistic reflections or detailed UI.
- Fabric/fur/mesh: simplify into broad soft forms or shallow rounded grooves; avoid noisy fine texture.

## Subject Rules

- Detailed objects: keep only the few defining features, then make them slightly larger, rounder, and cleaner so they read at thumbnail size.
- People: use blank rounded faces by default: no eyes, nose, mouth, or expression. Show role through clothing, tools, colors, silhouette, and pose.
- Human pairs/groups: show relationship through scale, spacing, posture, and gesture; avoid narrative scene details.
- Animals: unlike people, small simplified eyes/nose are allowed when needed for species recognition; avoid realistic fur.
- Gadgets: prefer soft graphite, warm gray, off-white, light silver, muted blue-gray, and restrained pale accents. Avoid stark black-heavy or cold realistic hardware palettes unless exact color matching matters.
- Keyboards/button grids: decide the intended layout in the prompt. Use blank simplified keys/buttons and explicitly prevent stray keys, duplicate buttons, symbols, or floating parts.
- Food/drinks: use warm rounded forms, simplified toppings, soft melted shapes, and brand-free containers.
- Related multi-object compositions: arrange as one balanced compact cluster, not a desk, table, street, room, or lifestyle scene.

Avoid:

- Photorealistic real-world scenes, busy backgrounds, rooms, landscapes, desk setups, or environmental props.
- Harsh shadows, dramatic lighting, neon glow, grunge, heavy outlines, or noisy texture.
- Overt handmade clay, fingerprints, lumpy modeling clay, or rough clay sculpture styling.
- Extra text, logos, watermarks, unreadable labels, brand marks, accidental duplicated parts, or layout-breaking details.
- Flat 2D vector art unless explicitly requested.

## Palette Guide

- Ecommerce/delivery: white, blue, cardboard tan, coral accents.
- Devices/gadgets: soft graphite, warm gray, off-white, light silver, muted blue-gray, restrained pale accents.
- SNS/marketing: pink, purple, yellow, mint, teal, playful accents.
- Business/security: blue, green, white, muted gray.
- Food/home: warm natural colors, off-white, tan, muted greens, pale wood, soft charcoal accents.

## Prompt Template

```text
Create a clean isolated isometric 3D icon of [subject].
Represent it as [single object / compact related group] with [key defining features], simplified but recognizable.
Use rounded geometry, smooth soft 3D display-model materials, and a very subtle clay-art softness.
Use a [palette] color palette: [colors].
[Subject-specific rule: blank rounded faces / blank keys / flat satin metal / subtle wood grain / simplified animal features / rounded food details.]
Place it centered on a white or very light gray background with generous whitespace.
Use a three-quarter top-down isometric view, soft ambient studio lighting, and a subtle contact shadow.
Clean commercial app icon style, crisp readable details, no real scene, no clutter, no text, no logos, no watermark.
```

For multiple related subjects:

```text
Arrange [subjects] as one compact isolated group with balanced spacing, consistent scale, and clear separation. Make the relationship readable through pose, proximity, overlap, or shared orientation, without adding a real environment.
```

For generated sets:

```text
Create [count] separate isolated isometric 3D icons with consistent scale, perspective, material, lighting, and palette. Use a grid only for a requested collection; otherwise generate each asset separately.
```

## QA Checklist

Before returning an image or prompt, verify:

- Background is white or very light gray.
- Subject is isolated and not part of a real scene.
- View reads as isometric or three-quarter top-down.
- Forms are rounded, soft, and simplified without becoming unclear.
- Lighting is soft with only subtle contact shadows.
- Subject is recognizable at thumbnail size.
- Important features survive simplification without becoming sharp, noisy, or photorealistic.
- Materials read as simplified soft-icon materials.
- People use blank rounded faces unless the user asked otherwise.
- Groups read as compact icon compositions, not lifestyle scenes.
- Gadgets and grids have no stray keys, buttons, symbols, logos, or duplicate details.
- Food, animals, plants, and furniture are readable but still clean, rounded, and brand-free.
- Palette matches the subject domain and the `samples/` style.
