# Interaction and QA checklist

These checks are appropriate for educational machine animations and do **not** replace mechanical design validation.

- [ ] Startup has no JavaScript exceptions.
- [ ] Play and Pause control actual animation.
- [ ] Next stage and phase selector reach every stage, including final discharge/ejection.
- [ ] Speed affects movement and its label reflects the selected speed.
- [ ] Reset returns mechanism and stage to the initial condition.
- [ ] Cutaway/exterior controls change visibility of internals.
- [ ] Moving components, process captions and stage readouts are synchronized.
- [ ] Tablet ejection includes **lower punch moving upward with the tablet**, not merely raising a label or stopping at compression.
- [ ] Entire mechanism fits a 390px mobile viewport; controls remain usable.
- [ ] The model renders with no network calls and continues to work offline.
- [ ] Contrast, labels and touch/keyboard interaction remain usable.
- [ ] Reduced motion is honored in implementations that support autoplay toggling.
- [ ] All actual engineering dimensions and process settings are marked unavailable or illustrative.

## Browser smoke test

Open `pharma/index.html` or a machine page, play and pause, choose each process stage, set speed to slow/fast, toggle cutaway, then reset. Watch the browser console for errors. For the tablet press, review all five stages and watch the lower punch present the tablet.

The five standalone machine HTML files and the combined simulator were locally loaded and checked for JavaScript startup errors in Chromium in November 2026. That does not certify scientific or mechanical correctness.
