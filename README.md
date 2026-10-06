# GGBond Illustrations Lite

A lightweight Codex Skill for converting abstract Chinese text, concepts, essays, posts, and methodology notes into explainable 16:9 white-background hand-drawn editorial illustration prompts.

## Quick Start

Invoke the skill with a `text` input:

> $ggbond-illustrations-lite text="..." protagonist_style="..." tone="..."

## Key Features

- **Extract the cognitive move** behind any text, then map it to one visual scene.
- **Replaceable protagonist**: default is a "GGBond 式原创小人" (round, lively, cute, slightly puzzled), or set your own via `protagonist_style`.
- **IP-safe**: protects against reproducing recognizable characters from protected IPs.
- **Low-token output**: concise concept analysis + one-prompt generation.
- **Designed for editorial use**: 16:9, white background, hand-drawn linework, minimal annotations.

## Input Parameters

| Parameter | Required | Default | Description |
|-----------|----------|---------|-------------|
| `text` | Yes | — | The concept, paragraph, or idea to illustrate |
| `protagonist_style` | No | GGBond 式原创小人 | Short description of the desired protagonist character |
| `tone` | No | — | Mood: funny, calm, absurd, serious, warm, satirical |
| `output_language` | No | Chinese | Language for the output sections |
| `annotation_level` | No | minimal | How many annotations in the illustration |

## Output Sections

- **概念动作** — the cognitive move (1 sentence)
- **画面隐喻** — the visual metaphor (1 sentence)
- **插画提示词** — the image prompt (1 paragraph)
- **自检** — self-check with 4 Yes/No items

## Why Lite

This is the **lite** version of the GGBond Illustrations skill family. It keeps no long case libraries, no image databases, and no lengthy examples — just the logic, template, and safety rules.

## License

Released under the [MIT License](LICENSE).
