# Economic referee rubric, source mapping and reusable prompts

This file operationalizes original synthesized review procedures. It is **not** a verbatim copy of third-party skills or writing guides. Read for manuscript reviews and for changing a previous `Scientific PASS` into a two-axis science/economics acceptance decision.

## 1. Independent referee form (Codex -> Cursor via real ACP)

For each major section, Cursor must provide **passage location, specific claim, observed data support, economic argument quality, source proof, revision and severity**.

| Area | What to verify | Critical/Major trigger |
|---|---|---|
| Economic question | Answerable question with real economic stakes; no introduction bait-and-switch | Introduction promises channels/causal policy that cannot be addressed |
| Main findings | A clear substantive fact, magnitude and benchmark | Results reproduce statistics without an economic claim |
| Mechanism logic | Distinct mechanism and observable predictions | Local causal attribution unsupported; list of mechanisms without evidence |
| Literature depth | Full/accessible primary source; sample/outcome/mechanism match | Misattributed source or claim supported only by citation metadata |
| Heterogeneity | Economic meaning of group/city differences | An individual influential observation is called an economic cause |
| Economic implications | Actionable interpretation bounded by actual evidence | Policy effectiveness/net zero asserted from accounting or descriptive maps |
| Research contribution | New understanding, measurement, or differentiation, not just more methods | Key economic question remains unanswered with no honest boundary |
| Intro and review positioning (v2.3) | Economic question beyond identities; grounded closest-work comparison; literature synthesized by findings and scope | Method combination called novelty without comparison; unsourced gap or author–year list substitutes for synthesis |
| Hypothesis taxonomy (v2.3) | Economic propositions separated from unnumbered robustness and measurement sensitivity | Sensitivity/robustness is labeled as standalone H4/Hn or presented as independent economic finding |
| Scientific integrity | Accurate model, data, uncertainty and study boundary | Invented numbers, unsupported causal sign, false replication claim |
| Prose | Concise, fair, readable after substantive accuracy | Language polish conceals thin economic reasoning |

**Decision:** `Scientific integrity: PASS/HOLD`; `Economic interpretation: PASS/HOLD`. For final manuscript `FINAL PASS` requires both PASS. A descriptive/measurement paper **can** pass without local causal-mechanism identification if the paper is honest about its contribution, offers well-supported economic interpretation, and frames causal mechanisms as open questions.

## 2. Source-derived design choices, with original links

| Source | Relevant verified source content | Adapted rule in this skill | Scope caveat |
|---|---|---|---|
| Hanlulong, `econ-writing-skill`, core SKILL | Main result first; economic rather than only statistical magnitude; theory M → predicted X → test X for mechanisms; distinguish mediation from suggestive evidence | §§2, 4–6, 9 | Strong causal identification instructions are conditional on causal paper type; do not force on Kaya/LMDI accounting |
| `franklee16/academic-research-skills`: `paper-taste`, `references/narrative.md`, `references/evidence.md`; `good-story-main` | A few concrete claims with rigorous proof; story tension; distinguish evidence hierarchy; do not let narrative outrun source | §§2–4, 8–9 | Collection aggregates upstream skills; this package takes concepts, not their full files |
| `iik1/academic_writing_skills`: `econ-field-writing-style_SKILL.md`; `energy-economics_SKILL.md` | Introduction reports question/results; Results carry meaning, not every table entry; Discussion examines mechanisms, alternatives and implications; apply field norm first then journal-specific rule | §§3–5, 7 | Journal patterns derived partly from previews and have limited validation; current official journal author instructions override |
| Keith Head, *The Introduction Formula* | Hook, Question, Antecedents, Value Added, Road Map; end-of-paper re-evaluation of Introduction; avoid bait-and-switch | §3 | This is a narrative framework, not mandatory paragraph numbering |
| Marc Bellemare, *How to Write Applied Papers in Economics* (2020), §§6.4, 7, 8.2 and surrounding text | Investigate plausible mechanisms with the best feasible evidence, even descriptive; describe untested mechanisms honestly; keep outcomes, limitations and implications meaningful | §§5–6, 8 | Main paper often discusses causal applied micro; adapt inference requirements to descriptive studies |
| Prior seven underlying skills + 2 JMU guides | Original skills and section alignment remain mandatory | §1, §8 | This upgrade does not reinstall or relicense third-party skills |

### Direct links used for integration

- https://github.com/hanlulong/econ-writing-skill/blob/main/.agents/skills/econ-write/SKILL.md
- https://raw.githubusercontent.com/franklee16/academic-research-skills/master/paper-writing/paper-taste/SKILL.md
- https://raw.githubusercontent.com/franklee16/academic-research-skills/master/paper-writing/paper-taste/references/narrative.md
- https://raw.githubusercontent.com/franklee16/academic-research-skills/master/paper-writing/paper-taste/references/evidence.md
- https://raw.githubusercontent.com/franklee16/academic-research-skills/master/paper-writing/good-story-main/SKILL.md
- https://github.com/iik1/academic_writing_skills
- https://raw.githubusercontent.com/iik1/academic_writing_skills/main/skills/fields/econ-field-writing-style_SKILL.md
- https://raw.githubusercontent.com/iik1/academic_writing_skills/main/skills/economics/energy-economics_SKILL.md
- https://blogs.ubc.ca/khead/research/research-advice/formula
- https://marcfbellemare.com/wordpress/wp-content/uploads/2020/09/BellemareHowToPaperSeptember2020.pdf

The `ft50-empirical-writing` material in `franklee16` was considered for the high-level question → theory → evidence → implication flow, but its causal-identification-first instruction was intentionally **not** imposed on descriptive environmental economics papers. Source: https://raw.githubusercontent.com/franklee16/academic-research-skills/master/paper-writing/ft50-empirical-writing-main/SKILL.md

**Copyright / scope:** This package consists of new instructions derived from the listed sources, paraphrased and attributed; it does not include third-party repository files, full books, full journal manuals, or copied Skill bodies. Links are for optional upstream consultation.

## 3. Minimal handoff prompt — drafting or major revision

> Read `.agents/skills/social-science-writing-gate/SKILL.md`. Classify paper type, lock the approved data/model, and first prepare the Economic Argument Matrix with phenomenon, economic stakes, candidate mechanisms, prediction, study evidence, external source, competing explanation, policy boundary. Identify any economic-interpretation HOLD before drafting. Write results as meaningful economic facts, Discussion as evidence-calibrated economic explanation, and Conclusion as an answer to Introduction. Apply underlying seven skills/two JMU guides, run anti-defensive passes on two distinct drafts, and obtain real independent Cursor ACP referee review. Keep versions separate. Do not change the approved models or invent causal mechanisms. Return scientific and economic PASS/HOLD separately.

## 4. Minimal handoff prompt — independent Cursor review

> Independently read the current manuscript sections, actual final tables and mechanism references. Apply `social-science-writing-gate` and focus on ECONOMIC INTERPRETATION: does Results identify economically substantive patterns? Does Discussion explain what could cause these patterns, contrast source-backed explanations, disclose what cannot be tested, and derive conditional implications? Check Introduction bait-and-switch, accounting vs causal claims, units, source fit and numerical consistency. Return paragraph-location Critical/Major/Minor findings and dual gate decision. Do not automatically approve because calculations/citations/English are correct.

## 5. Prompt for a Zhejiang-v1.5-style paper

> For each substantive economic hypothesis (e.g., H1–H3), make a finding/economic-puzzle/mechanism/literature/evidence matrix. Prioritize why eleven Zhejiang city intensities fell while ranks/disparities differed; which sector/energy/innovation/urban structure theories could rationalize the observation; why positive output growth can coexist with rising absolute CO2 despite lower intensity; what different annual versus endpoint decoupling implies; and which *unnumbered robustness checks* actually change economic assessment. Use Luo et al. (2025) only after checking its original mechanism claims and comparing outcome boundaries. Do **not** claim the city panel identifies sector mix, technology or carbon-neutrality policy effects unless such evidence is separately established. Audit first; seek author approval before adding new variables/tests or rewriting approved text.


## 6. v2.1 — independent citation-to-mechanism review

For **each central mechanism claim in Discussion** (and any nontrivial external claim in Results):

- Quote or identify the exact manuscript **sentence** and the **citation immediately supporting it**.
- Identify the original paper's title, DOI/URL, outcome, sample, method, variables and **actual findings**. Read its original relevant sections where available; mark `abstract-only` if that is all that can be checked.
- Verify the paper truly supports the **specific channel**, not just the general subject of carbon emissions. Do not use a study about data inventory quality as proof of industrial composition or technology effects.
- Check relevance and differences in territorial vs consumption emissions, CO2 vs all greenhouse gases, city vs province, study years, nominal vs real output, correlation vs causality.
- For each independent important economic judgment, ordinarily expect 1–2 directly supporting studies; for one connected mechanism cluster, typically 1–3 complementary works. **Never enforce a citation count mechanically.** One decisive source can suffice. Weak or conflicting literatures require explicit qualification rather than citation padding.
- Check that a source validating a general mechanism is **not** used to claim the mechanism actually operated in the current city's data.
- Find unsupported leaps, cumulative citations at a paragraph's end, fabricated references, missing DOI/author-year integrity and one-sided literature selection.
- Report `MECHANISM_CITATION: PASS/HOLD` with claim IDs, offending sentences, source-grounded corrections and whether a local test would be required.

Suggested concise Cursor review task:

> Review each distinct major economic-mechanism sentence in Discussion. Make a claim/source/evidence-level ledger; verify 1–2 direct source papers per independent claim or 1–3 complementary papers for each mechanism cluster when appropriate. Check exact source findings and place citations near propositions. Reject generic end-of-paragraph citation stacks, literature-based local causal attributions, fabricated or mismatched sources. Report Major/Critical issues and `MECHANISM_CITATION: PASS/HOLD` separately. Preserve the approved empirical results.

## 7. v2.2 Results exposition and comparison review

For work that revises Results, load only the final Results sections, key approved tables and `results-economic-comparison-guide.md`. Independently re-check selected derived ratios and compare the draft against the evidence ledger. Mark `RESULTS_EXPOSITION: PASS/HOLD` separately in the review; map material HOLD to the existing overall `Economic interpretation: HOLD`. Do not require new ratios when no useful validated benchmark is available.

**Required separate question:** What economically instructive comparison was available in the approved outputs but omitted from the written paragraph? Name its inputs and why it changes the reader's understanding. Do not privilege the most dramatic unit if it is not representative.


## 8. v2.3 Introduction, Literature Synthesis and Hypothesis Referee (real Cursor ACP)

Load `references/introduction-literature-argument-guide.md` when checking Introduction, Literature Review, or hypothesis framing. Independently read the *actual current* manuscript question, Results, Discussion, closest cited sources (to their available depth), and the candidate's compact question–answer–contribution and literature relation matrices. Do not judge from the matrices alone.

**Introduction:** Identify the exact question; state what remains economically uncertain beyond a definition/identity. Name the most relevant existing study/studies and what specifically the manuscript adds, supported by the real Results. If the only novelty is a method combination, return `INTRODUCTION_ARGUMENT: HOLD` for substantive repositioning. **Check the first sentence for a concrete economic phenomenon rather than an unexplained aggregate/distributional label; flag an abstract opening when it hides the stakes. Check that the concluding preview selects indispensable findings without listing every number, city outcome or robustness case.** Judge natural English and appropriate scope; do not enforce a four-paragraph quota or numeric limit.

**Literature Review:** For each main stream, cite at least one *actual relationship* among verified study findings or explain why no meaningful contrast is supportable. Flag source-outcome mismatch, convergence/dispersion conflation, empty 'research gap', unreferenced substantive empirical propositions, and method definitions occupying the literature synthesis. Do **not** invent a study disagreement or impose a citation count. If the review is an author–year list or fails to show the paper's marginal position, return `LITERATURE_SYNTHESIS: HOLD`.

**Hypotheses:** Explicitly inspect every proposed numbered `Hn`. Confirm that each refers to a substantive, answerable economic proposition or labeled descriptive expectation; test, robustness, measurement sensitivity, alternative inventory/price definitions, sample omissions, and model diagnostic checks belong in Methods/Robustness without `Hn` numbering. Return `HYPOTHESIS_TAXONOMY: HOLD` for a new candidate that contains a sensitivity H4/Hn. For approved legacy text, report the issue and exact dependent cross-references and request author-scoped migration approval; never silently edit protected text. There need not be a fixed number of hypotheses.

Return passage-level `Critical/Major/Minor`, source citation/locator where available, a bounded correction, and separate **diagnostic sub-gates**: `INTRODUCTION_ARGUMENT: PASS/HOLD`, `LITERATURE_SYNTHESIS: PASS/HOLD`, `HYPOTHESIS_TAXONOMY: PASS/HOLD`. They are editorial sub-checks of the existing economic-interpretation decision, **not** a new validator, JSON schema, or substitute for upstream citation QA. Keep scientific and citation-integrity statuses separate. Genuine ACP assignment/results only; never forge independence.