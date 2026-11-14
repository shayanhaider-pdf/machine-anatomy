# Visual and mechanical design principles

Adapted from the Anatomy for ChatGPT project kit; inspiration and upstream credit: [Ryan's Anatomy](https://github.com/wheresryan22/anatomy) (MIT).

## Object first

A machine explainer should look like its named machine at a glance, with enough context to understand function. Show frame, tooling, drives, interfaces, guards/housings, inlets and outlets. Avoid generic rectangles, disconnected parts, unsupported pipe ends and labels blocking components.

## Camera and cutaway

Use a consistent isometric-style or cutaway camera. Shading should show depth: light top, medium front, darker side, fine outlines. Allow moving parts enough room at **all** operating extremes. Label cutaway and schematic geometry honestly; this is not CAD.

## Mechanisms

A single state model should control every moving part and every descriptive readout. Do not independently animate objects that have a dependent relationship. For punches, the tablet cannot float or remain behind during lower-punch ejection. For crank-slider and reciprocating machines, derive connected-rod and slider positions from the same crank angle.

## Presentation

Use restrained colors with one accent for moving/active mechanisms, explanatory legends, responsive panels and accessible controls. Capture the entire mechanism at mobile widths, not only on desktop.

## Packaging

Prefer a self-contained `.html` with embedded JS/CSS and no network dependencies. The finished example should run offline after downloading. Link out to source references separately.

## Accuracy

Never invent pharmaceutical process setpoints, product tolerances, safety limits or equipment specifications. All models here are illustrative educational visualizations.
