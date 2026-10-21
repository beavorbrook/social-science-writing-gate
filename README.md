# Social Science Writing Gate — Economics-Enhanced v2.2

An orchestration **Codex Skill** for empirical economics, environmental/energy economics, regional economics, and social-science writing. It coordinates established research Skills instead of copying all their code or documentation.

## What v2.2 adds

- **Results Economic Magnitude and Comparison Gate:** Begin results with an economic phenomenon, select an informative *verified* comparison, explain its size and significance, and distinguish representative evidence from extreme cases.
- **Results exposition check:** Independent Codex–Cursor review reports `RESULTS_EXPOSITION: PASS/HOLD`, with numerical traceability and protection against cherry-picked contrasts.
- **Results guide:** [results-economic-comparison-guide.md](references/results-economic-comparison-guide.md) covers regional disparities, LMDI decompositions, decoupling, and measurement sensitivity.

## Retained from v2.1

- **Economic Interpretation Gate:** Connect results to economic puzzles, candidate mechanisms, evidence levels, competing explanations, and bounded policy implications.
- **Mechanism citations:** Usually one or two directly supporting papers per important claim, or one to three complementary sources for a mechanism cluster. These are not citation quotas.
- **Independent reviewing:** Scientific integrity, economic interpretation, and mechanism citation support are separate final acceptance gates. Cursor's ACP review must be real, not simulated.
- **Seven original Skills, two JMU guides, and two Anti-Defensive-Writing passes**, with token-efficient, selective source loading. Upstream Skills are not bundled.

## Install

Clone or download the repository into a folder named `social-science-writing-gate` under your project's `.agents/skills/` directory. The entry point is [`SKILL.md`](SKILL.md). See the Chinese [INSTALL.md](INSTALL.md) for safe backup, update, validation, and rollback.

## Files

- [SKILL.md](SKILL.md): Coordinating Skill and quality gates
- [REFERENCES_AND_SKILLS.md](REFERENCES_AND_SKILLS.md): Seven original Skills and economic-writing sources
- [references/results-economic-comparison-guide.md](references/results-economic-comparison-guide.md): v2.2 Results drafting and reviewer checklist
- [references/economic-argument-guide.md](references/economic-argument-guide.md): Economic argument guidance
- [references/referee-and-source-checklist.md](references/referee-and-source-checklist.md): Independent referee and citation audit
- [INSTALL.md](INSTALL.md), [CHANGELOG.md](CHANGELOG.md): Installation and version history

## Attribution

Writing guidance is synthesized and adapted from sources acknowledged in [`REFERENCES_AND_SKILLS.md`](REFERENCES_AND_SKILLS.md). This repository does **not** bundle upstream Skills or copyrighted books. Scientific claims and references should be independently verified.

**Version: 2.2.0**