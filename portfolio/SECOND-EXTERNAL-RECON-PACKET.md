# Second External Recon Packet — Draft

Status: Draft control packet pending remote GitHub/PyPI remediation.

## Agent Instruction

You are evaluating the Zer0pa public portfolio as an external reviewer. You have no access to local files. Treat public GitHub and PyPI as authority.

## Use These Sources

1. Public portfolio index:
   - https://github.com/Zer0pa/.github/blob/main/portfolio/PORTFOLIO-INDEX.md
   - https://raw.githubusercontent.com/Zer0pa/.github/main/portfolio/portfolio-index.json
2. The 32 public GitHub repositories linked from the index.
3. The PyPI project pages or absence/name-collision states linked from the index.
4. Public GitHub releases/tags.

## Do Not Use These Sources As Current Authority

- historical recon documents;
- local file paths;
- private handovers;
- old website cache;
- package names inferred from repo names without PyPI confirmation;
- previous agent conclusions without URL receipts.

## Core Questions

For each lane:

1. Does the GitHub repo exist and is it public?
2. Is the PyPI package connected, absent, legacy, name-collided, or not package-shaped?
3. Do README, GitHub metadata, release/tag, and PyPI agree?
4. What is the current authority gate?
5. What is the current blocker?
6. What does the repo explicitly not claim?
7. What commercial wedge, if any, is supported by public remote evidence?
8. What methodology/diligence wedge, if any, is supported by public remote evidence?
9. Is there cross-repo contamination, stale namespace language, multimodal subtree drift, or marker collision?
10. What is the A/B/C action classification?

## Output Format

Return one report per lane:

```text
Lane:
GitHub Receipt:
PyPI Receipt:
Repo/PyPI Agreement:
Current Authority Gate:
Current Blocker:
What Is Real:
What Is Not Claimed:
Commercial Product Wedge:
Methodology/Diligence Wedge:
Cross-Repo Contamination:
A/B/C Classification:
Required Fixes:
Public URLs:
```

## Acceptance Gate

The second external recon passes only if all 32 lane reports cite public URLs and no lane omits PyPI treatment.

Do not treat this draft packet as final approval to score the portfolio as repaired. If a lane's status packet URL returns 404, or if PyPI still says stale `PRIVATE`, `INTERNAL`, wrong license, wrong blocker, or no-PyPI language, report that as a public-source fault.
