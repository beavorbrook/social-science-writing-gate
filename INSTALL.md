# Install and pilot validation — v2.4.0-rc2

**Unreleased release candidate for planned v2.4.0. This is an isolated candidate, not a GitHub update or an instruction to overwrite stable v2.3.0.** Keep the existing approved manuscript and Skills untouched. The archive top-level directory is `social-science-writing-gate/` and contains `SKILL.md` and all referenced local guides.

## Safest local test

1. Record the active Skill location/version and its SHA-256 file inventory. Back up any local customizations.
2. Extract the ZIP into a separate project test folder, e.g. `skill_candidate_v2.4.0-rc2/social-science-writing-gate/`.
3. In the Codex pilot instructions, explicitly load `skill_candidate_v2.4.0-rc2/social-science-writing-gate/SKILL.md` and `references/data-empirical-framework-guide.md`. Do **not** rely on automatic discovery of a noninstalled candidate.
4. Verify all 10 Markdown files and confirm the three pre-existing `references/economic-argument-guide.md`, `references/results-economic-comparison-guide.md` and `references/introduction-literature-argument-guide.md` guides remain unchanged in content. Check all seven upstream Skills remain installed; do not reinstall or replace them.
5. Conduct a separate, protected Section 3 A/B evaluation with real Cursor ACP, preserving the stable 2.3.0 Skill, the approved manuscript and all results. Return `DATA_METHODS_EXPOSITION`, `SCIENTIFIC_INTEGRITY`, `SOURCE_METHOD_MATCH`, and genuine ACP verification; keep the formal literature validator in its independent status.
6. If the pilot loses essential definitions, sources, formulae, reproducibility or Results links, mark HOLD even when the prose becomes shorter. Do not merge or publish the candidate without author approval.

## Permanent installation after a future author decision

Only after acceptance: use a versioned backup and update the *one* intended active Skill folder. No duplicate active variants and no automatic modification of `econ-write`, other original skills or literature-validator code. Current official stable source: https://github.com/beavorbrook/social-science-writing-gate (v2.3.0).

## Rollback

The entire test lives outside the active Skill directory. Deleting the isolated candidate restores the status quo; no rollback of paper files or GitHub is needed.
