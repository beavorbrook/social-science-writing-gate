# Results Economic Magnitude & Comparison Guide (v2.2)

This is a **Results-only**, transferable writing and review guide. Read when drafting/revising empirical Results, not automatically for Discussion. It consolidates the existing `social-science-writing-gate` principles rather than installing or copying a new Skill.

## 1. Why this exists

Reporting all values accurately is necessary but not sufficient. A useful empirical Results section **selects the most revealing comparable magnitudes** and turns them into clear facts about an economy. In the Zhejiang v2.0 manuscript, the agent reported Quzhou's and Shaoxing's intensity levels and percentage reductions but omitted the easily verified **between-city intensity ratio**, an especially intuitive illustration of persistent level differences. The absence is a communication gap, **not a failed calculation or an identified economic mechanism**.

## 2. Pre-draft comparison candidates (short ledger)

Use existing *approved* tables, figures, validated scripts and numeric sources. For each main Results subsection, record a few candidate comparisons (there is no fixed minimum), then choose those most likely to change the reader's substantive understanding:

| Claim / economic phenomenon | Source cells or validated output | Candidate economic contrast | Calculation / common units / rounding | Representativeness and alternative cases | Economic interpretation and evidence boundary | Keep? reason |
|---|---|---|---|---|---|---|

Selection priorities, in order:

1. **Research-question relevance:** Does the comparison illuminate the stated economic puzzle, not merely dramatize a number?
2. **Valid denominators and matching objects:** Same units, period, real/nominal convention, geography, emissions scope, and population at risk where applicable. Check nonzero/stable denominators, percentage versus percentage-point conventions, log versus level distinctions.
3. **Economically interpretable scale:** e.g., how many times larger, how many percentage points apart, level gap, initial-to-final distance, output increase versus emissions increase, share of aggregate change, effect-size relative to a sensible benchmark.
4. **Non-cherry-picked heterogeneity:** Set any selected two units in the all-unit distribution; identify whether they are endpoints, typical, outliers or a contrasting pair. Show conflicting patterns when important.
5. **Parsimony:** One lucid comparison may be better than six statistics. A missing useful contrast should be supplied; a trivial or unstable derived figure should not.

For every new descriptive computation, preserve a one-line provenance record: `input source → expression → unrounded result → presentation rounding → sample/period/units`. An approved source file and standard calculator/spreadsheet are enough; no extra panel model is authorized by this guide.

## 3. Results paragraph architecture (non-mechanical)

- **Lead:** Economically meaningful finding in ordinary field language.
- **Magnitude:** Verified size with units and reference period.
- **Diagnostic comparison:** Most informative matched before/after, between-unit, between-group, or continuous-versus-category contrast.
- **Economic meaning:** What this observation does/does not establish (within-unit change ≠ convergence; lower intensity ≠ absolute reduction; LMDI term ≠ technology effect).
- **Evidence link:** Point to the actual table, map or figure; do not narrate everything displayed.
- **Handoff:** Pose the *specific* economic origin or implication explored in Discussion, without making an unsupported claim now.

Paragraph lengths and ordering can vary; not every subsection needs every move or two cases. **A reader should understand the economic takeaway without memorizing the statistical estimator.**

## 4. Worked Zhejiang examples — illustration ONLY; verify again against approved final data

### 4.2 City-level carbon intensity: a useful contrast

Verified table values used by the v2.0 manuscript:

| City | 2015 | 2024 | Reduction |
|---|---:|---:|---:|
| Quzhou | 23,423.52 | 13,266.79 | 43.36% |
| Shaoxing | 3,874.44 | 2,379.13 | 38.59% |

Unit: tonnes fossil CO2 per 100 million RMB of 2015-anchored real GDP.

Descriptive ratio: `Quzhou_2015 / Shaoxing_2015 ≈ 6.05`; `Quzhou_2024 / Shaoxing_2024 ≈ 5.58`. The ratio decreased, but a large endpoint gap remained. **This is a two-city comparison, not a test or sufficient statistic for all-city disparity**. Report alongside the actual 11-city distributional results: CV falls, while log-SD and log-IQR rise.

**Under-informative yet valid:** “Quzhou's larger proportional improvement did not eliminate its much higher starting level.”

**More informative (when space allows):** “Quzhou's intensity remained about 5.58 times Shaoxing's in 2024, compared with about 6.05 times in 2015: the two-city proportional gap narrowed but stayed large.”

The second version uses an understandable quantitative *comparison*. Neither statement proves why the cities differ in industrial composition, technology or energy use. Those mechanisms belong in Discussion with verified evidence.

### 4.1 Output and fossil emissions: relative versus absolute

Use the approved aggregate: real output +73.33%, fossil CO2 +11.71%, intensity −35.55%. The important contrast is that **lower emissions per output did not reduce absolute emissions**. Avoid calling intensity decline absolute decarbonization. Give total emissions change in Mt when established and useful.

### 4.3 LMDI: partial offsets

Approved direct three-factor aggregate account: output per resident +165.5214 Mt, composite intensity −164.6155 Mt and population +40.5945 Mt; net +41.5004 Mt. The informative comparison is the near-cancellation of the two large terms, **not** a causal attribution to technology or regulation. Source and aggregation definitions matter; retain direct-versus-chained information when material.

### 4.4 Decoupling: continuous magnitudes versus classifications

Three city economies exhibit cumulative strong decoupling while eight are weakly decoupled, despite all lowering intensity. Cite underlying GDP and emissions changes for contrasting cities; Zhoushan real GDP +112.97% and emissions +63.39% illustrates why weak decoupling can coexist with rising absolute emissions. Quzhou's −0.25% emissions change is near the sign boundary; do not interpret its classification as a stable net-zero trajectory.

### 4.5 Robustness: test an economic claim

Instead of listing every numerical sensitivity scenario, ask whether the change reverses a meaningful comparison or category. Example: excluding Quzhou reverses the endpoint direction of CV change; grid-center allocation reverses the log-SD direction, but the basic coexistence of aggregate intensity decline and rising fossil emissions remains. Report a significant classification change; put low-value implementation detail elsewhere without hiding material uncertainty.

## 5. Other empirical papers: adaptable comparison choices

- **Panel/regression:** Interpret effect in natural units and over a credible change in X; use confidence bounds and actual identification limits. Never equate statistical significance with economic importance; never invent a standard deviation or reference group.
- **Treatment/policy evaluation:** Give both baseline and intervention comparison, specify treated population and absolute or relative effect, justify causal language by design. Do not conflate coefficients with total welfare effects.
- **Efficiency/frontier studies:** State measured efficiency gap and meaningful peer/period contrasts; distinguish estimated frontier distance from a verified mechanism or policy gain.
- **Heterogeneity:** Compare substantive effect sizes across prespecified groups; note precision and composition. A strong claim of between-group difference requires a supported direct comparison, not separate significant/insignificant estimates.
- **Distributional/inequality analysis:** Pair global dispersion measures with interpretable relative positions or distributional segments; a selected city pair cannot establish distributional convergence.
- **Accounting/decomposition:** Contrast the terms that matter for net economic change; do not relabel identities as structural causal effects.
- **Spatial maps:** Describe meaningful geographic variation only when directly supported by mapped outcomes; maps alone cannot demonstrate causes or spillovers.

## 6. The Cursor Results exposition referee: independent, focused

Before approving Results, Cursor should inspect draft paragraph(s), approved final tables and the candidate-comparison ledger, *not merely the whole PDF*. Ask:

1. **Finding:** Can a reader state a concrete economic phenomenon in one sentence?
2. **Magnitude:** Is its size quantified in interpretable units, and are the baselines/denominators correct?
3. **Comparison:** Has an important, valid and available magnitude/ratio/benchmark been omitted? If none is suitable, record that fact without manufacturing one.
4. **Sample context:** Do city/group examples illuminate rather than replace full-sample evidence? Are counterexamples and edge cases retained?
5. **Meaning:** Does the text explain what the empirical result means economically, without inferring a causal mechanism it did not test?
6. **Display economy:** Is the table/figure used to support a finding rather than mechanically narrated, and does the subsection end with one useful handoff to Discussion?

Report exact passage, source table/cells, revised wording and Critical/Major/Minor severity. If the text is numerically correct but omits a reader-critical available comparison, return `RESULTS_EXPOSITION_HOLD` for substantive rewrite, nested under `Economic interpretation: HOLD`. Do not hold a draft merely because it lacks a decorative ratio. A concise, complete Results subsection is acceptable.

## 7. Reviewer prompt (copy ready)

> Independently audit Section 4 against `references/results-economic-comparison-guide.md`. For each subsection, read its final approved source tables and identify the 1–2 most informative *valid* economic contrasts. Check whether the draft selects and quantifies them, explains what they mean for the research question, and distinguishes illustrative cases from the full sample. Verify every newly derived ratio or gap and its price base, time, units and denominator. Report paragraph-level Critical/Major/Minor issues and `RESULTS_EXPOSITION: PASS/HOLD`. Do not add new models, literature mechanisms or fabricated comparisons. Preserve numerical results and original sources.
