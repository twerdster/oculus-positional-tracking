# Updated browser example

Added 17 November 2026 as a new, project-specific interaction. It is separate from the recovered software and is not the students' implementation.

## What runs

Play a generated head trajectory and vary noise, sample delay and exponential smoothing; export the synthetic samples.

Time is counted in generated samples, not hardware timestamps or output rates. Delay is applied to the generated trajectory before deterministic noise is added; the filter computes pₜ = αsₜ + (1 − α)pₜ₋₁, where sₜ is the delayed, noisy sample and pₜ the filtered estimate. Smoothing reduces rapid variation and introduces lag. It does not establish how the original tracking providers performed.

## Run

Open https://twerdster.github.io/oculus-positional-tracking/ or serve the repository's `docs/` directory with any static HTTP server. For example, from the repository root:

```sh
python3 -m http.server 8000 --directory docs
```

Open `http://localhost:8000`. The demo uses standard Canvas 2D and local browser controls. No additional demo packages, SDKs or credentials are required. Downloads are generated JSON files. No camera permission is requested.

## Implementation

`docs/index.html` contains the controls and factual scope labels; `docs/demo.js` implements the interaction; `docs/demo.css` contains the responsive layout. All generated images/data are illustrative. It uses no KinectFusion or Vicon recordings and runs none of the original code.

## Recorded checks

[VALIDATION.json](VALIDATION.json) records 11 passed browser assertions on the new interaction, JSON export where present, local-only requests, error-free JavaScript and a 390-pixel responsive layout. These are interaction assertions on generated/local examples, not accuracy or compatibility benchmarks. Original native application/hardware coverage is unchanged; see [historical recovery notes](../docs/RECOVERY.md).

## Attribution and terms

Original project: [Dor Goldbaum](https://www.linkedin.com/in/dorgold/), [Vlady Ostrovski](https://www.linkedin.com/in/vladislav-ostrovski-b99619121/). Supervision: Aaron Wetzler. The new browser example was prepared with Codex assistance in November 2026; Claude reviewed the README wording and factual scope. The new files have a [scoped MIT license](../docs/DEMO-LICENSE.txt); it does not relicense historical code, images, slides, reports or third-party dependencies.
