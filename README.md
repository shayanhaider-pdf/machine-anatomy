# Machine Anatomy

Interactive, browser-based mechanical explainers and pharmaceutical manufacturing process visualizations. This is an independent **Anatomy for ChatGPT** adaptation, inspired by the [Anatomy toolkit by Ryan](https://github.com/wheresryan22/anatomy) (MIT).

## Open the machines

**[Five-machine interactive gallery](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/index.html)**  
**[Combined simulator with machine selector](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/pharma/index.html)**

Each model is self-contained and can run offline once downloaded as HTML.

| Pharmaceutical machine | Run model | Source |
| --- | --- | --- |
| High-shear granulator | [Open](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/pharma/models/granulator.html) | [HTML](pharma/models/granulator.html) |
| Fluid-bed dryer | [Open](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/pharma/models/dryer.html) | [HTML](pharma/models/dryer.html) |
| IBC bin blender | [Open](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/pharma/models/blender.html) | [HTML](pharma/models/blender.html) |
| Rotary tablet press | [Open](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/pharma/models/press.html) | [HTML](pharma/models/press.html) |
| Perforated pan tablet coater | [Open](https://raw.githack.com/shayanhaider-pdf/machine-anatomy/main/pharma/models/coater.html) | [HTML](pharma/models/coater.html) |

The simulations illustrate charging, mixing, airflow and drying, blending, tablet compaction and ejection, and coating. The playback and cutaway controls are functional.

## Repository contents

- [`index.html`](index.html): start page with links to all five machines.
- [`pharma/index.html`](pharma/index.html): combined interactive simulator and controls.
- [`pharma/models/`](pharma/models): five stand-alone animated machine pages.
- [`examples/anatomy-machine-explorer.html`](examples/anatomy-machine-explorer.html): earlier interactive crank-slider/tablet-press machine explorer (includes upstream attribution in HTML).
- [`examples/tablet-press-original-demo.html`](examples/tablet-press-original-demo.html): original ChatGPT-adapted tablet press demo.
- [`examples/tablet-press-corrected.html`](examples/tablet-press-corrected.html): corrected punch-and-tablet ejection prototype.
- [`archive/2026-11-12/`](archive/2026-11-12): earlier five-model editions.
- [`skills/anatomy/SKILL.md`](skills/anatomy/SKILL.md): reusable Anatomy for ChatGPT instructions.
- [`docs/PROJECT_INSTRUCTIONS.txt`](docs/PROJECT_INSTRUCTIONS.txt): instructions for ChatGPT Project setup.
- [`docs/GETTING_STARTED.md`](docs/GETTING_STARTED.md): setup and use guide.
- [`docs/DESIGN_PRINCIPLES.md`](docs/DESIGN_PRINCIPLES.md): drawing and state-model design.
- [`docs/QA.md`](docs/QA.md): interaction and verification checklist.
- [`docs/TEST_PROMPTS.md`](docs/TEST_PROMPTS.md): prompts for future new machines.
- [`docs/ATTRIBUTION_AND_LIMITATIONS.md`](docs/ATTRIBUTION_AND_LIMITATIONS.md): attribution and scope.
- [`LICENSE`](LICENSE): MIT license.

## Use it to generate new interactive machines

1. Copy the text from [the project instructions](docs/PROJECT_INSTRUCTIONS.txt) into your ChatGPT Project instructions.
2. Add [the skill](skills/anatomy/SKILL.md), [design principles](docs/DESIGN_PRINCIPLES.md) and [QA guide](docs/QA.md) as references.
3. Describe the machine and required movement, then ask for a runnable, self-contained HTML file.
4. Test playback, all stages, and the final discharge/ejection step.

## QA and limitations

The five standalone HTML pages and the combined local simulator were loaded in Chromium at a 390px viewport without startup JavaScript exceptions on November 14, 2026. This verifies browser startup, **not** all mechanical details, live hosting or GMP compliance.

These are **educational illustrations**, not validated CAD models, equipment digital twins, production control programs or manufacturing procedures. Process parameters are schematic.

The full upstream Anatomy engine, libraries and audit scripts are in [wheresryan22/anatomy](https://github.com/wheresryan22/anatomy). This repo is an independent adaptation, not an official OpenAI or upstream release.
