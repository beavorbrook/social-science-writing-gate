# Social Science Writing Gate — Economics-Enhanced v2.4.0-rc2

An orchestration **Codex Skill** for empirical economics, environmental/energy economics, regional economics, and social-science writing. It coordinates established research Skills instead of copying all their code or documentation.

## What v2.4.0-rc2 refines (unreleased release candidate)

- Separate journal Methods, a locatable replication companion and author-facing QA logs.
- Display central formulas without needless equation renumbering.
- Distinguish exact, analogous and framework-level source support at its actual verification depth.
- Apply the same principles to a non-carbon econometric brief without importing accounting formulas or cutoffs.

The planned stable version is v2.4.0. No stable release, installation or publication is represented by this candidate.

- **Data/Empirical Framework Exposition Check:** Put data provenance, essential equations, valid classification rules and clear economic meaning before implementation minutiae.
- **New original guide:** [data-empirical-framework-guide.md](references/data-empirical-framework-guide.md) covers variables and units, concise data sources, Figure/Table 1 placement, source-method matching, LMDI and author-specified identities, decoupling interpretation and reproducibility boundaries.
- **Independent Cursor review:** `DATA_METHODS_EXPOSITION: PASS/HOLD` is a writing-quality sub-check only, not an executable formal literature validator.
- **Transferability:** Do not impose the pilot paper's Section 3 numbering, Kaya/LMDI/Tapio choices, two-reference preference or figure moves on unrelated empirical papers.

## Retained v2.3.0 Introduction/Literature/Hypothesis improvements

- Concrete answerable economic research questions and contribution positioning; synthesis of verified literature findings.
- No H4 or other numbered hypothesis for sensitivity, robustness or software diagnostics.
- Concrete Introduction opening and proportionate results preview.

## Retained v2.2 Results improvements

- **Results Economic Magnitude and Comparison Gate:** Begin results with an economic phenomenon, select an informative *verified* comparison, explain its size and significance, and distinguish representative evidence from extreme cases.
- **Results exposition check:** Independent Codex–Cursor review reports `RESULTS_EXPOSITION: PASS/HOLD`, with numerical traceability and protection against cherry-picked contrasts.
- **Results guide:** [results-economic-comparison-guide.md](references/results-economic-comparison-guide.md) covers regional disparities, LMDI decompositions, decoupling, and measurement sensitivity.

## Retained from v2.1 and v2.2

- **Economic Interpretation Gate:** Connect results to economic puzzles, candidate mechanisms, evidence levels, competing explanations, and bounded policy implications.
- **Mechanism citations:** Usually one or two directly supporting papers per important claim, or one to three complementary sources for a mechanism cluster. These are not citation quotas.
- **Independent reviewing:** Scientific integrity, economic interpretation, and mechanism citation support are separate final acceptance gates. Cursor's ACP review must be real, not simulated.
- **Seven original Skills, two JMU guides, and two Anti-Defensive-Writing passes**, with token-efficient, selective source loading. Upstream Skills are not bundled.

## Install

**Pilot only:** Install this archive in an isolated, explicitly addressed directory; the active stable v2.3.0 installation and GitHub `main` must remain unchanged. See [INSTALL.md](INSTALL.md) for the reversible test. Do not create duplicate active installations.

## Files

- [SKILL.md](SKILL.md): Coordinating Skill and quality gates
- [REFERENCES_AND_SKILLS.md](REFERENCES_AND_SKILLS.md): Seven original Skills and economic-writing sources
- [references/data-empirical-framework-guide.md](references/data-empirical-framework-guide.md): v2.4 Data/Empirical Framework guide
- [references/introduction-literature-argument-guide.md](references/introduction-literature-argument-guide.md): v2.3 Introduction/Literature/Hypotheses guide
- [references/results-economic-comparison-guide.md](references/results-economic-comparison-guide.md): v2.2 Results drafting and reviewer checklist
- [references/economic-argument-guide.md](references/economic-argument-guide.md): Economic argument guidance
- [references/referee-and-source-checklist.md](references/referee-and-source-checklist.md): Independent referee and citation audit
- [INSTALL.md](INSTALL.md), [CHANGELOG.md](CHANGELOG.md): Installation and version history

## Attribution

Writing guidance is synthesized and adapted from sources acknowledged in [`REFERENCES_AND_SKILLS.md`](REFERENCES_AND_SKILLS.md). This repository does **not** bundle upstream Skills or copyrighted books. Scientific claims and references should be independently verified.

**Version: 2.4.0-rc2 (unreleased candidate for planned v2.4.0; active stable remains v2.3.0)**
