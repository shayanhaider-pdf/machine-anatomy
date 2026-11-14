---
name: anatomy-for-chatgpt
description: Generate stand-alone interactive machine explainers with inspectable mechanisms.
---

# Anatomy for ChatGPT

This is a lightweight ChatGPT-oriented adaptation inspired by [Anatomy by Ryan](https://github.com/wheresryan22/anatomy), which is MIT-licensed. It is **not** the original engine or a replacement for its geometry audit tools.

## Goal

Turn a plain-language request about a real machine into a **working standalone HTML, SVG or Canvas interactive explainer**, not a static diagram or a promise to write code. Choose a recognizable physical mechanism and explicitly state any schematic assumptions.

## Implementation requirements

1. Map the essential mechanical components and their attachment points.
2. Use a coherent scene model from a single animation state or phase: all geometry, labels and readouts must agree.
3. Derive dependent movements from mechanical relationships. For a tablet press, the compacted tablet must follow the **lower punch** during ejection and rise above the die before take-off.
4. Offer genuine play/pause, speed and reset controls; add cycle scrubber, cutaway and clickable part inspection when appropriate.
5. Prefer responsive, self-contained HTML with embedded CSS and JavaScript, requiring no CDN or installation.
6. Show all process phases, including the final ejection/discharge/reset phase. Do not stop after compression.
7. Respect keyboard focus, touch controls, sufficient contrast and reduced-motion preferences.
8. When tools permit, test JavaScript startup, phase switching, playback, controls and mobile layout in a browser. Do not claim tests you have not run.
9. Clearly distinguish a simplified conceptual simulation from validated CAD, engineering tolerances and pharmaceutical GMP operating instructions.

See [design principles](../../docs/DESIGN_PRINCIPLES.md), [QA checklist](../../docs/QA.md), [test prompts](../../docs/TEST_PROMPTS.md) and [five machine examples](../../pharma/index.html).

## Provenance

This repository contains independent example visualizations and adaptation instructions. The full upstream anatomy toolkit is at https://github.com/wheresryan22/anatomy. Attribution and MIT license notices must be retained for any upstream code reused.
