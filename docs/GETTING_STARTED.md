# Getting started

## Run the demos

Open [the machine gallery](../index.html) in any browser using a hosted URL, then choose a machine. For a combined interface that switches machines without navigating, open [the pharma simulator](../pharma/index.html).

Direct HTML files are in [pharma/models](../pharma/models). Every file is self-contained and works offline after saving it.

Controls vary by example, but include playback, phase/stage selection, speed and a cutaway or external view. Tablet press stages must include tablet ejection and reset.

## Use it with ChatGPT

Copy [PROJECT_INSTRUCTIONS.txt](PROJECT_INSTRUCTIONS.txt) into a ChatGPT Project's instructions. Attach [SKILL.md](../skills/anatomy/SKILL.md), [design principles](DESIGN_PRINCIPLES.md) and [QA reference](QA.md) as supporting knowledge if desired.

Example request:

> Create a stand-alone interactive cutaway of a tablet press. Show die filling, compaction, upper punch withdrawal, lower punch ejection and reset. Provide real play/pause, scrub, stage selection and speed controls. Test that ejection works.

For advanced geometry features and the full original engine, use the upstream [Anatomy project](https://github.com/wheresryan22/anatomy). These local demos do not include the complete original skill engine.

## Development and publishing

The site is plain HTML and requires no build. A hosted static server can serve the repository root. GitHub Pages can be configured in repository Settings > Pages, or the HTML files can be viewed through a trusted static HTML preview service. GitHub's `blob` code pages display source rather than running the animation.

Do not treat the visualizations as validated pharma equipment simulators or manufacturing SOPs.
