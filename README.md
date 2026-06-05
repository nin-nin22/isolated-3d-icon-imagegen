# isolated-3d-icon-imagegen

[日本語版](README.ja.md)

A Codex / ChatGPT skill for creating cute, loosely deformed 3D icon-style isolated images with image generation.

It uses the bundled `samples/` as style references and helps turn everyday objects, gadgets, food, plants, animals, people, and small concepts into clean isolated 3D icon images.

## What It Does

This skill helps you generate:

- isolated 3D icon-style images
- softly rounded and simplified objects
- compact product, app, ecommerce, and marketing visuals
- image generation prompts that match the sample style

## Use Cases

- product icons
- ecommerce assets
- app illustrations
- SNS and marketing visuals
- office, gadget, food, animal, plant, and character-like isolated objects

## Repository Structure

```text
.
├── SKILL.md          # Skill instructions
├── agents/
│   └── openai.yaml   # Agent metadata
└── samples/          # Reference images that define the target style
```

## Example Usage

```text
Use $isolated-3d-icon-imagegen to generate a cute isolated 3D icon of a small delivery box with a smartphone.
```

```text
Use $isolated-3d-icon-imagegen to generate a loosely deformed 3D icon-style isolated image of a potted plant and two stacked books.
```

## Notes

This repository contains the skill instructions and reference samples. Actual images are generated with the image generation tool available in the Codex / ChatGPT environment.
