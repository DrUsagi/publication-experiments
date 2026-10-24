# Publication Experiments

An interactive simulation laboratory for research production, journal submissions and peer review. The standalone English app reproduces the frozen models and parameter settings used in paper version 29, while allowing custom experiments and complete manuscript-trajectory replay.

## Download

**[Download the Mac Apple Silicon app — 29.2.3](https://github.com/DrUsagi/publication-experiments/releases/download/v29.2.3/V29_Simulation_English_29.2.3_macOS_AppleSilicon.zip)** · 169 MiB ZIP

[Release page and installation notes](https://github.com/DrUsagi/publication-experiments/releases/tag/v29.2.3)

Requirements: Apple Silicon Mac (M1 or later), macOS 14 or newer. Python and both original numerical environments are bundled. The app runs offline; no Python installation is needed.

## Start

1. Download and unzip the release asset above.
2. Move **V29 Simulation English.app** to Applications or another folder on your Mac.
3. Double-click the app. Its English interface opens in your default browser at a local `127.0.0.1` address.
4. Choose a paper preset, edit parameters for a custom experiment, or open **Trajectory replay** to explore the bundled original example.

The app is ad hoc signed and is not Apple-notarized. If macOS blocks the first launch, follow [Apple's instructions for opening an app from an unidentified developer](https://support.apple.com/en-us/102445). Detailed instructions, dependency licenses and test evidence are included in the ZIP.

## Features

- 111 paper configurations, 12 original seeds and three frozen simulation engines.
- Editable model inputs, including nested settings, journal arrays and policy operations.
- Automatic selection of the historical or current numerical environment corresponding to the original archive.
- Exact request export, saved results, progress reporting and safe stopping.
- Manuscript and author search, review and revision histories, timeline playback and complete-history exports.
- A complete original 5,000-author example with 83,432 manuscripts for immediate exploration.

## Verification

The release passed four original full-scale comparisons (5,000 authors, 60 journals, eight years, seed 34001001), with complete parsed worlds exactly equal to their original archives. All 111 paper configurations also passed reduced-population regression checks using 16 authors, and 33 custom scenarios matched independent original-source runs exactly. Another 32 invalid-input cases were rejected before job creation. The scientific model source and original requests remain unchanged.

Full-scale 1a and 1b were rerun in 29.2.3. Full-scale 8f and 9 were run in 29.2.1; their frozen source and numerical libraries were verified byte-identical in 29.2.3. The final release separately passed the configuration, custom, lifecycle, English-interface and standalone-distribution checks. This is not a rerun of all 1,356 historical executions. Tests were performed on one Apple Silicon Mac; the bundled report documents coverage and limitations.

## Files and results

The downloadable software is under **Releases**. GitHub's automatically generated “Source code” archives contain this repository's documentation; download the explicitly named Apple Silicon ZIP to obtain the application.

Simulation results are saved locally under `~/Library/Application Support/V29 Simulation/outputs/runs/`. Existing results are preserved, and each new run has its own request and provenance record. Keep at least 20 GiB free on the results volume and 5 GiB on the system volume, as required by the original persistence safeguards.
