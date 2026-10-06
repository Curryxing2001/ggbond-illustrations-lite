---
name: ggbond-illustrations-lite
description: Convert abstract Chinese text, concepts, essays, posts, and methodology notes into explainable 16:9 white-background hand-drawn editorial illustration prompts. Supports replaceable protagonist style.
---

# GGBond Illustrations Lite

## Purpose

This skill turns abstract ideas, long text, arguments, or methodology content into clear, interesting editorial illustration prompts.

It is designed for:
- Chinese articles
- blog posts
- Notion notes
- methodology explanations
- abstract concepts
- educational or explanatory content

It is not for:
- generic decorative images
- PPT infographics
- photorealistic rendering
- copying protected IP characters
- logos, mascots, or brand-identical character reproduction

## Core Workflow

When invoked, follow this workflow:

1. Read the user text and identify the core cognitive move.
2. Convert that idea into a visual metaphor.
3. Generate one concise image prompt.
4. Check whether the protagonist follows the user override.
5. Check whether the image explains the concept rather than merely decorating it.

## Inputs

The user may provide:

- `text`: the concept, paragraph, article excerpt, or idea to illustrate.
- `protagonist_style`: optional. A short description of the desired protagonist.
- `tone`: optional. Example: funny, calm, absurd, serious, warm, satirical.
- `output_language`: optional. Default: Chinese.
- `annotation_level`: optional. Default: minimal.

If `protagonist_style` is missing, use:

> GGBond 式原创小人：圆润、活泼、可爱、略微困惑的原创小人，适合正文配图；不使用任何可识别的受保护角色特征。

If `protagonist_style` is provided, replace the protagonist with the requested original character style while preserving the illustration logic.

## IP and Character Safety Rule

If the user asks for a specific protected IP character, famous anime character, game character, movie character, brand mascot, or celebrity likeness:

- Do not reproduce the recognizable character.
- Do not copy distinctive costume, logo, face, weapon, color arrangement, or signature visual identity.
- Convert the request into a non-infringing original character inspired by general traits.

Example:

User asks:
> 用某个知名忍者动漫角色风格

Safe interpretation:
> 一个原创热血少年冒险者，头戴简单布带，动作夸张，充满少年漫画式能量，但没有任何可识别 IP 特征。

## Visual Style

Default image style:

- 16:9 horizontal composition
- white background
- hand-drawn editorial illustration
- simple black linework
- slightly weird but understandable metaphor
- minimal red, orange, or blue annotations
- not too polished
- not photorealistic
- not a comic strip unless requested
- suitable as an inline illustration inside an article

## Illustration Logic

Focus on the idea behind the text.

Look for one of these cognitive moves:

- contrast
- trade-off
- paradox
- bottleneck
- feedback loop
- hidden assumption
- mistaken shortcut
- decision fork
- compounding effect
- abstraction becoming concrete
- system pressure
- mismatch between expectation and reality

Then map it to one visual scene.

## Output Format

Always output in this format:

### 概念动作
One sentence explaining the core cognitive move.

### 画面隐喻
One sentence describing the visual metaphor.

### 插画提示词
A concise image-generation prompt.

### 自检
- 主人公是否符合用户指定：Yes/No
- 是否避免复刻受保护 IP：Yes/No
- 是否解释概念而非装饰文本：Yes/No
- 是否 16:9 白底手绘正文配图：Yes/No

## Prompt Template

Use this template for the final image prompt:

Create a 16:9 horizontal white-background hand-drawn editorial illustration.
Main protagonist: {protagonist_style}.
Scene: {visual_metaphor}.
Style: simple black linework, slightly absurd but clear, minimal red/orange/blue handwritten annotations, article illustration, not photorealistic, not polished, no brand logos, no recognizable protected IP character.
The image should explain: {core_idea}.

## Compression Rule

Be concise. Do not write long analysis unless the user asks.

Default output should be short:
- 概念动作: 1 sentence
- 画面隐喻: 1 sentence
- 插画提示词: 1 paragraph
- 自检: 4 bullets
