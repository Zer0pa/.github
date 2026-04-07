# Zer0pa

**Deterministic compression for structured signals. One geometric architecture, eleven applied domains.**

Zer0pa builds codecs that compress domain-specific data — sensor telemetry, hand-pose streams, robot motion, geospatial trajectories, financial time-series, neural signals, biosignals, motion capture, speech prosody, digital ink, and multimodal content — using a unified set of eight geometric primitives.

Every codec guarantees **bit-exact deterministic replay**. No GPU required. No neural network. No probabilistic reconstruction. What you encode is exactly what you decode, every time.

### The Repos

| Package | Domain | Headline |
|---------|--------|----------|
| [`zpe-iot`](https://github.com/Zer0pa/ZPE-IoT) | IoT / Sensors | 17× compression on real sensor datasets, edge-deployable (Rust + Python) |
| [`zpe-xr`](https://github.com/Zer0pa/ZPE-XR) | XR / Hand Tracking | 56× compression, sub-mm pose fidelity, 0.025ms latency |
| [`zpe-robotics`](https://github.com/Zer0pa/ZPE-Robotics) | Robotics / Motion | 187× compression on LeRobot data, wire-format replay |
| [`zpe-geo`](https://github.com/Zer0pa/ZPE-Geo) | Geospatial | Trajectory codec, sub-metre fidelity, zero dependencies |
| [`zpe-ft`](https://github.com/Zer0pa/ZPE-FT) | Financial Data | OHLCV + tick-stream codec, ≥13× on synthetic benchmarks |
| [`zpe-neuro`](https://github.com/Zer0pa/ZPE-Neuro) | Neural Signals | Extracellular spike-train codec, DANDI-validated |
| [`zpe-bio`](https://github.com/Zer0pa/ZPE-Bio) | Biosignals | ECG + EEG codec in Rust and Python, embedded reference path |
| [`zpe-mocap`](https://github.com/Zer0pa/ZPE-Mocap) | Motion Capture | Joint-angle compression, search-without-decode |
| [`zpe-prosody`](https://github.com/Zer0pa/ZPE-Prosody) | Speech Prosody | Pitch/rhythm/stress codec, 4/6 gates verified |
| [`zpe-ink`](https://github.com/Zer0pa/ZPE-Ink) | Digital Ink | `.zpink` stylus codec, >5× vs raw float32 |
| [`zpe-imc`](https://github.com/Zer0pa/ZPE-IMC) | Multimodal Platform | 10 modality lanes, 276.8k IMC words/s, integration layer |

### License

All repos are source-available under [SAL v6.0](https://github.com/Zer0pa/ZPE-License-Commercial). **Free below USD 100M annual gross revenue.** Commercial, hosted, or legal-interpretation questions: [architects@zer0pa.ai](mailto:architects@zer0pa.ai).

### Who This Is For

- **Developers** building on constrained devices, real-time pipelines, or audit-grade data infrastructure
- **Investors and evaluators** conducting technical due diligence on codec IP
- **Grant reviewers** assessing computational physics or information-theory research
- **Deep tech engineers** who want deterministic, verifiable compression — not black-box approximation

### Where to Start

Pick the domain repo closest to your signal type. Each repo has a quickstart, proof artifacts, and benchmark data. [ZPE-IMC](https://github.com/Zer0pa/ZPE-IMC) ties the architecture together across domains.
