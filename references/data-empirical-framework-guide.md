# Data & Empirical Framework — Economic-Methods Writing Guide (v2.4.0-rc2)

## Purpose and scope

**Audience:** economics, environmental/energy economics, regional economics and empirical social science. **Status:** original coordinating guidance; it does not replace discipline-specific methods, the source-data audit, the publisher's style guide, or the underlying Econ Writing Skill's authentic validator.

**Governing rule:** A Data/Empirical Framework section tells the reader **what was observed, where the data came from, how each reported measure or estimator was constructed, what the reported values mean, and what interpretation the design supports**. It is not a software manual, a source-archiving diary, a premature Results section, or a defensive catalogue of everything that might be disputed. Scientific replicability remains mandatory, using concise main-text definitions backed by technical appendices or project artifacts as appropriate.

Apply this guide when creating or substantively revising Data, Variables, Study Area, Measurement, Empirical Strategy, Empirical Framework, Model Specification, or a closely equivalent methods section. Use the existing paper's headings and journal requirements; do not force a five-subsection skeleton onto every study. In particular, a user-requested deletion of a standalone robustness subsection does **not** authorize deletion of essential robustness definitions or results.

## 1. Freeze a compact Data–Method–Meaning ledger before editing

For each important empirical object, record only what is needed to keep the manuscript and references aligned:

| Field | Question |
|---|---|
| Sample / period / unit | Which observational units, years, geographic boundary, missingness and effective number of observations? |
| Variable and terminology | What is the economic construct, displayed name, symbol, unit and price/quantity/emissions boundary? |
| Source and vintage | Which original dataset or official publication actually supplied the variable? Which specific vintage or processing decision materially changes its meaning? |
| Construction rule | Source-level measurement, aggregation, deflation/index-linking or estimation equation, and indispensable constants/reference year? |
| Model type | Descriptive statistic, exact accounting identity, index decomposition, associational estimator, causal estimator, simulation, or classification rule? |
| Interpretation | What does a larger/lower index, a factor contribution, a coefficient, a classification, or a contrast establish economically? |
| Evidence support | Correct original citation for the dataset and any nonstandard borrowed transformation/estimator; exact scope of the source's support? |
| Replication location | What appears in the main text, minimal table, appendix, source ledger, script or data documentation? |
| Downstream alignment | Are the same symbols, units, ranges, figure numbers and labels used in Results/Discussion? |

This ledger is an internal aid, **not a new JSON schema, external dependency or mandatory manuscript table**. An editorial review can be `DATA_METHODS_EXPOSITION: HOLD` for substantive omissions; it is separate from formal citation-audit status.

## 2. Write the data subsection for readers, not for the research assistant

Recommended order, when appropriate:

1. State study region, years, observation unit, panel structure and major variables in **one compact opening paragraph**.
2. Group data sources by economic object: (a) outcome/emissions or other environmental measure; (b) economic activity, especially real and nominal output; (c) population, electricity/energy and other controls. Describe a material spatial aggregation or index conversion once, with an equation **only when the definition affects interpretation or reproducibility**.
3. Give one concise Table 1 of **variables, units and source** when this satisfies the author's requested style. A role/purpose column or lengthy notes are not automatic requirements; retain them only when the table would otherwise be ambiguous or the journal requires them.
4. Provide a neutral link to one descriptive figure if it is placed here and a short, evidence-based data-quality or unusual-observation notice only when relevant to interpretation.

**Readable main text:** Use established names after first definition, e.g. *real GDP* rather than repeating *official-index-reconstructed-volume-series-on-2015-monetary-anchors* in every paragraph. Keep the needed base year, real/nominal distinction, original emissions boundary, and source genealogy **at the first definition**. Archive per-year document links, precision, historical release selection, CRS, software switches, interpolation recipes and nonessential validation history outside the prose unless they change the effective measure or conclusion. This is concision **without concealing material choices**.

**Source fidelity:** A source citation must substantiate the *exact operation claimed*. A paper using grid centroids is not evidence for area-overlap allocation; a paper that constructs historical GDP levels is not automatically evidence for city-level year-on-year chaining. If the author requests two recent examples, seek two authentic, relevant, verified examples in that window; do not impose a universal reference quota or describe a merely analogous source as an identical procedure. Cite database versions accurately.

**Real GDP illustration (conditional):** For official constant-price growth reported in percent, a transparent construction is

`Y^R_{i,t} = Y^R_{i,t-1}(1 + g^R_{i,t}/100)`, with an explicitly reported reference-year level.

This is a sample construction, not a required model across all papers. Check whether growth is a true volume rate, its reference/coverage and applicable years. Do not collapse nominal GDP, real GDP, index-linked series and growth rates into the same unit.

**Data anomalies:** Describe the *observed feature* (e.g. a large final-year change concentrated in named grid cells) and the diagnostic performed. A conspicuous value is not by itself an error. If it materially shifts inference, direct the reader to the appropriate Results/robustness analysis; avoid both burying it and speculative error attribution. A one-sentence notice in Data can be enough.

## 3. Decide where descriptive figures belong by argumentative function

- A plot directly showing the trend of variables imported/constructed from data (such as real output, emissions and intensity indexed to a base year) **may** appear after data sources to orient the reader, particularly when the author requests this. Introduce it as an **overview**, not model identification.
- Descriptive statistics are also empirical evidence; there is **no universal rule** that a raw-data-based chart must be in Data instead of Results. Place it where the economic argument benefits most and follow the journal/author's organization.
- If relocating an existing figure, preserve the actual original figure file, caption, label, number/cross-references where possible; avoid duplicate environments, reordering errors or claims that the trend is model-estimated. Results can still interpret the phenomenon and cite that figure. Keep a moved-figure reconciliation log.
- A map of influential grids, alternative measurement, leverage effects or robustness outcomes normally belongs with the substantive diagnostic evidence, **unless** the author approves a different organization. A one-sentence Data note is not a substitute for disclosing influential sensitivity.

## 4. For each empirical method: calculation → interpretation → output link

### Mathematical presentation across empirical designs

Display the defining identity, estimand or specification when its components, denominator, weights or assumptions require inspection. Short auxiliary definitions can stay inline. Group related equations with aligned lines; avoid a long one-line chain of fractions and definitions. Follow prose with the economic meaning of the terms. Number equations when useful for subsequent references, preserving existing labels and semantic targets; unnumbered displays can improve readability without changing the established equation order. Do not maximize or minimize the equation count as a quality metric.

For a panel regression, the central display may be the regression specification; for Logit, the conditional probability link; for an accounting study, an identity and allocation rule. Each retains its own inferential meaning. A readable display cannot compensate for an omitted identifying or uncertainty assumption.


The main-text method paragraph must ordinarily allow the reader to answer the following in natural economic language, without software trivia:

1. **Economic object:** Why use this measure/estimator for the research question?
2. **Formula/rule:** What is its defining equation, inputs, time interval, weighting and indispensable threshold or assumption?
3. **Interpretation:** What does a positive/negative contribution, larger/smaller dispersion, coefficient or class mean for actual economic behavior or outcomes?
4. **Output link:** Which table/figure/Results subsection reports the corresponding evidence, and what is **not** identified by this method?

Do not mechanically add an equation in every paragraph or repeat results in Methodology. Keep real estimates, comparisons and substantive findings in Results. Distinguish an **exact accounting relation** from a technology, policy, structural or causal mechanism. Describe sign and unit accurately without writing repeated stand-alone “this does not prove causation” sentences.

### 4.1 Intensity, aggregation and regional disparities — illustrative only

If `I_it = C_it/Y^R_it`, explain *fossil CO₂ per unit of real output*. When provincial `I_t = sum_i C_it / sum_i Y^R_it`, state that this is output-weighted, not the simple equal-city mean. If relative city position `r_it = I_it / mean_i(I_it)`, `r>1` is above the contemporaneous equal-city intensity mean; it is **not** a city-specific efficiency parameter or a percent of total emissions.

For multiple dispersion measures (e.g. coefficient of variation, SD of logs and log-IQR), display necessary definitions and **say which aspect of between-city differences each measures**. Do not assume all must move together. A log transform changes the comparison scale; a lower level-CV does not establish that every part of the distribution has converged. Preserve sample/population denominator and weighting conventions when they materially affect reported levels/comparisons.

**Implementation detail:** software-specific quantile/interpolation algorithms (e.g. `R type-7`) usually belong in reproducibility material rather than narrative prose, unless they cause a material numerical discrepancy, are needed to disambiguate a nonstandard statistic, or the journal mandates disclosure. Removing that sentence from the main text **does not license deleting the precise setting from code/metadata**.

### 4.2 Kaya / LMDI and supplemental identities — illustrative only

For the three-factor accounting identity `C = P × (Y/P) × (C/Y)`, name each factor, define its economic unit and explain the **algebraic identity**. If using additive LMDI, supply its essential allocation and log-mean definition once, with an original method citation where verified. Explain: positive factor contribution adds to the **accounted change** under this identity, negative contribution offsets it, and the sum reconciles to observed change. Compare direct and chained accounts if both are actually used, and avoid adding provincial factor contributions by summing municipal factors when the province is constructed aggregate-first.

For an extension such as `C = P × (Y/P) × (Q/Y) × (C/Q)`, identify it as the **study-specified supplementary accounting identity**, not an independently estimated alternative model or a standard electricity-grid emission factor. `Q/Y` describes electricity per real output; `C/Q` with **total territorial fossil CO₂** in the numerator is an emissions-to-electricity **composite accounting ratio**, not power-plant emissions per delivered kWh. A noncausal term cannot be relabelled 'technological effect' or 'fuel effect'.

**Reference attribution:** Cite the original Kaya/LMDI or factor-decomposition framework, and cite a verified genuinely relevant predecessor when claiming an externally borrowed electricity/energy extension. If predecessors use **different component definitions**, state the adaptation briefly; do not assert they use the identical four-factor formula. An algebraic factorization chosen by the authors does not acquire an external methodological provenance merely because a superficially related paper is cited. Do not fabricate two 'exact-method' sources to satisfy a quota.

### 4.3 Growth–emissions decoupling — illustrative only

Define the economic distinction *before* the elasticity formula: **relative decoupling** means emissions increase more slowly than real output; **absolute decoupling** means output increases while emissions fall. For a defined interval, `g_C=C_1/C_0−1`, `g_Y=Y^R_1/Y^R_0−1`, `epsilon=g_C/g_Y`. Explain a class in growth-rate language as well as by cutoff.

**For intervals with positive GDP growth**, a common Tapio implementation is:

- `g_C <= 0`: strong decoupling (absolute emissions are non-increasing during output growth);
- `g_C > 0` and `0 < epsilon < 0.8`: weak decoupling (emissions rise but proportionally more slowly than output);
- `0.8 <= epsilon <= 1.2`: expansive coupling (similar proportional growth);
- `epsilon > 1.2`: expansive negative decoupling (emissions rise proportionally faster than output).

State the exact boundary conventions actually used; thresholds are **classification bands**, not physical constants or economically estimated turning points. Interpret epsilon as a ratio of interval growth rates, not a structural elasticity or a causal marginal effect. Do not claim an epsilon of 0.8 is an exact policy threshold. If zero/negative GDP-growth intervals occur or the paper generalizes beyond positive growth, disclose and implement the appropriate remaining sign-dependent classes, undefined ratios and near-zero growth denominator handling; do not silently apply positive-growth rules. The entire codebook can live in technical material **only if the classifications in the paper remain interpretable**. Report annual and cumulative classifications separately; the cumulative class is not an average of annual elasticities. Cite the authentic Tapio definition, not a later paper only loosely discussing decoupling.

### 4.4 Other designs

For regression, spatial, panel, DID, IV, SFA, DEA, GAM, Bayesian or structural models, translate the same four questions—**estimand, specification/assumptions, coefficient/result interpretation, and scope of identification**—into the specific model's context. Do not import the above equations or the decoupling thresholds into an unrelated paper. Material standard-error/cluster/uncertainty assumptions belong in the Methods, even if their software implementation belongs in supplemental code.

## 5. Separate manuscript, replication and audit layers

|Layer|Retain here|Placement test|
|---|---|---|
|Manuscript Methods|Research object, sample/time/unit, useful original-source provenance, variable units/price basis, central formulas, material assumptions, uncertainty rules and economic interpretation|Can the reader understand and evaluate each result without decoding software? Active classification edges and causal-identification assumptions cannot be hidden.|
|Replication companion / appendix|Full source-vintage and processing ledger, exact parameter settings, software versions, complete taxonomies/edge cases, code and diagnostics|Can another researcher locate and reproduce each consequential construction? Keep a concise main-text signpost when relocating detail.|
|Author-facing audit|File hashes and paths, task/agent assignments, QA chronology, download errors, version comparisons and approval logs|Does the item establish provenance for the team rather than explain the economic method to journal readers? Avoid importing the log into prose.|

These are placement decisions, not permission to omit information. Promote a detail to main Methods, a table note or an explicit appendix reference when it changes the measure, class, estimand, identification, uncertainty or substantive conclusion. A full taxonomy may reside in a companion only when every class actually reported in the paper remains interpretable. State clustering/uncertainty and identification assumptions at the level needed for the design; moving a software command does not move away its scientific assumption. A source table number or exact construction reference can be useful concise manuscript provenance; a list of file hashes usually is not.

Use one locatable companion instead of repeated promises of unspecified records. Keep the companion with the deliverable, reconcile its source/label links, and preserve definitions when removing a standalone Methods subsection. Robustness, influence, alternate windows and measurement checks remain supporting analyses, not separate numbered hypotheses.

## 6. Anti-defensive writing: precision first, caveats when material

Bad patterns: reciting 'not causal/not verified/not a proof' after every descriptive formula; defending routine statistical choices before telling the reader what a metric means; long archives of source-vintage caveats in the GDP paragraph; narrating software routines rather than economic objects.

Preferred order: **state positively what the variable/identity/classification measures and what the finding means; retain one compact qualification exactly where a plausible consequential misunderstanding remains**. Examples:

- Prefer 'The provincial intensity is an output-weighted ratio of total emissions to total real GDP' to a paragraph of repeated disclaimers about city averages.
- Prefer 'The `C/Q` term scales total territorial emissions by city electricity use' and, where needed, 'It is not a grid emission factor' to a long speculative discussion of what this ratio might approximate.
- Prefer 'The analysis evaluates changes in observed emissions and output' to repetitive statements that a purely descriptive account does not identify every possible policy channel.

The two existing anti-defensive passes remain genuine, separate passes. **They may never erase a method, emissions boundary, missing-data rule, negative-growth classification, causal-identification assumption or material sensitivity that a reader needs.** A reviewer should reward concise accuracy, not the mere absence of caveats.

## 7. Exact, analogous and framework-level source support

Record `(claim → original source/locator → verified operation and scope → match level → verification depth → citekey)` using the existing evidence ledger. Bibliographic identity, method equivalence and full-text access are separate facts.

|Match level|What the source supports|Appropriate manuscript treatment|
|---|---|---|
|Exact operation within verified scope|The relevant transformation/estimator and its consequential definitions, units, weighting, interval and assumptions actually match|Attribute that operation and state any restricted years or scope. A shared model name alone is insufficient.|
|Analogous operation|A related operation differs in data unit, benchmark, weighting, outcome or model structure|Say what is adapted and what differs. Do not call the current algorithm identical or imply that the external paper validates local data.|
|General framework|Principles or an allocation/estimation framework, without the same operational construction|Cite the framework for that purpose and identify the study-specified identity or specification separately.|
|Unresolved operational match|Only metadata, an abstract or indexed passages, or missing decisive details|Restrict the claim to inspected evidence; record its actual depth. Do not promote an index extract to full-text verification or invent a matching formula.|

An abstract may directly support a narrow statement appearing there, but it does not establish unseen equation details or author-stated limitations. Even full-text access does not make an analogous method exact. If essential data provenance or the method claimed in the manuscript is unsupported, retain the applicable HOLD and withhold that assertion. Bounded nonessential precedents can remain PARTIAL or be omitted from manuscript claims. A numerical citation quota cannot create equivalence. Preserve the existing claim-level mechanism and formal literature-validator requirements; editorial acceptance does not close those gates.

## 8. Independent Cursor referee: `DATA_METHODS_EXPOSITION: PASS/HOLD`

Require real ACP independent examination of the **actual model equations and data definitions**, the current manuscript, frozen Results and available source documents. Ask Cursor to:

1. Check **sample, units, terms and symbols** against Table 1, formulae, figures and downstream tables; spot conflicts across real/nominal GDP and output-weighted/equal-city measures.
2. Check **source fidelity**: does every data/method citation support the described operation, rather than an unrelated similar method? Record verification depth.
3. Check **calculation + economic meaning**: can a non-programmer economist interpret a lower intensity, a disparity index, a factor contribution and a decoupling class? Are these consistent with the actual equations?
4. Check **classification edges**: threshold inclusions, zero or negative denominators, observation intervals, and any special small-denominator rule actually used.
5. Check **extension semantics**: supplementary identities are transparently specified, `C/Q` boundaries aren't misread, and accounting effects aren't made causal.
6. Check **method-data continuity**: diagram/figure placement, labels, role of descriptive versus estimated findings, retained material sensitivity, and absence of stale cross-references after method-subsection removal.
7. Check **prose economy**: software-only details and repeated source-discovery narration removed or relocated; scientifically necessary definitions, boundaries and diagnostics still available.
8. Check **change protection**: no modifications to the approved model, results, references, data, figures or source-vintage choices without permission.

Return passage-level `Critical/Major/Minor`, a concrete bounded patch, a short model–meaning–source ledger, and `DATA_METHODS_EXPOSITION: PASS/HOLD`, plus separate `SCIENTIFIC_INTEGRITY` and `SOURCE_METHOD_MATCH` statuses when applicable. This is an **editorial sub-gate** under the existing framework, not a new executable validator or a substitute for an upstream formal literature/citation workflow.

## 9. Conditional examples and transferability

**Regional accounting illustration:** The Zhejiang pilot uses territorial fossil emissions, official-growth-linked GDP, distributional measures, LMDI and growth classifications. Its source-vintage caveat, uniform-within-cell assumption, author-specified four-factor identity and zero/negative-growth codebook illustrate consequential details. They do not prescribe emissions data, provincial weights, 2015 anchors, Tapio cutoffs, a Figure1 move or removal of Section3.6 for another paper.

**Non-carbon econometric illustration:** A firm-panel association study would define the firm-year sample, original financial/employment measures and units, display the fixed-effects specification, state firm/time effects and the declared cluster correction, and interpret the coefficient as a within-firm conditional association in the relevant units. A Logit study would instead define the binary outcome and link, distinguish log-odds coefficients from probability changes, and report any marginal-effect construction actually used. A causal design must retain its identifying variation and assumptions; an associational brief cannot acquire causality from polished wording.

Test the guidance on a clearly labelled synthetic writing brief without pretending that its data, coefficients or citations are real. The test is whether it chooses the right definitions, display and interpretation for that design. A shorter paragraph that loses a consequential assumption is a failure; a different paragraph is not automatically an improvement.
