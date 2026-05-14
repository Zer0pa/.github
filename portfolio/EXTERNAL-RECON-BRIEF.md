# External Recon Brief — Draft

Status: Draft control brief. Do not use for final external recon until every lane has public GitHub/PyPI remediation receipts and the final falsifier returns `NO_P0_P1_FAULTS_FOUND`.

## Objective

Evaluate the Zer0pa portfolio from public remote evidence only.

Use:

- public control index: https://github.com/Zer0pa/.github/blob/main/portfolio/PORTFOLIO-INDEX.md
- machine-readable control index: https://raw.githubusercontent.com/Zer0pa/.github/main/portfolio/portfolio-index.json
- linked public GitHub repos
- linked PyPI package pages / PyPI JSON
- public GitHub releases and tags

Do not use:

- old recon documents as current authority
- local machine paths
- private handovers
- local repo clones
- status packets not present in the public repo
- website cache if it conflicts with GitHub/PyPI

## Required Per-Lane Output

For each lane, report:

- GitHub URL and current visibility
- PyPI state: connected, absent, name collision, legacy, not package-shaped, or stale pending release
- package name and version if connected
- current top authority gate
- current blocker
- what is real
- what is explicitly not claimed
- commercial product wedge
- methodology/diligence wedge
- cross-repo contamination or namespace noise
- A/B/C action classification
- exact public URLs used

## A/B/C Action Classification

- `A_ADMIN_DILIGENCE`: public metadata, README, license, release, PyPI, naming, or status drift.
- `B_PLANNED_CODING_REQUIRED`: real engineering/science work remains, such as benchmark, corpus, hardware, runtime, baseline, package separation, or validation work.
- `C_LANE_INVALIDATES_OR_AUGMENTS`: the supplied source packet is materially wrong or missing a current public fact that changes the lane.

## Handling Lab-Window Repos

These repos are a window into live research. Work-in-progress status is not a failure by itself.

Failure is:

- hiding a blocker;
- claiming a gate has passed without public receipt;
- treating a stale package or README as current;
- turning a negative result into a positive product story;
- omitting PyPI state.

## Starting Point

Use the public remediation control index as the starting point while repairs proceed:

```text
https://github.com/Zer0pa/.github/blob/main/portfolio/PORTFOLIO-INDEX.md
https://raw.githubusercontent.com/Zer0pa/.github/main/portfolio/portfolio-index.json
```

This control index is not a claim that every repo/PyPI page is already aligned. It is the map for finding current public faults without relying on stale recon documents.
