---
name: social-science-writing-gate
description: Coordinate seven existing research/writing skills, two JMU guides and two anti-defensive-writing passes; enforce an economics argument gate, a Results comparison-and-magnitude gate, an Introduction question-and-contribution gate, a Literature Review synthesis gate, and claim-level source verification for proposed economic mechanisms. Use for drafting, reviewing and integrating economics and environmental-economics manuscripts with Codex and Cursor.
---

# Social Science Writing Gate — Economics-Enhanced v2.3.0

## 0. Role and precedence

This is an **orchestration and acceptance-gate skill**. It **upgrades** the earlier `social-science-writing-gate`; it does not replace or reinstall existing skills. It is intended for economics, energy/environmental economics, regional economics, and related empirical social sciences. It also works for other social sciences if the economics-specific questions are adapted.

**Core standard:** An empirically correct and well-written paper can still fail as economics if it does not identify an important economic phenomenon, offer economically grounded explanations, and say what its findings change in scholarly understanding or decision-making. This gate is **mandatory** before declaring a manuscript PASS.

Priority when rules disagree: **author-approved scope and evidence integrity > credible economic argument > source-supported interpretation > journal requirements > prose polish > token savings.** This gate never mandates new regressions, invented mechanisms, causal claims, or a change to an approved empirical model. Make substantive research changes only with the researcher's authorization.

**On every task, first identify paper type:** descriptive/measurement; accounting/decomposition; associational; causal reduced-form; structural; theory; or mixed. Apply reporting and mechanism standards appropriate to that type. Do **not** impose IV/DiD, significance stars, mediation tests, or exogenous treatment assumptions on descriptive accounting papers.

## 1. Preserve and coordinate the seven original skills

Locate the locally installed `SKILL.md` for each; read the relevant instructions instead of merely listing it. Avoid reinstalling functional dependencies.

1. **Econ Writing** — https://github.com/hanlulong/econ-writing-skill — question, economic magnitude, mechanisms, contribution, argument and editorial norms.
2. **Scientific Writing** — https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/skills/scientific-writing — evidence, accurate claims and reproducibility.
3. **Literature Review** — https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/skills/literature-review — field positioning, competing accounts, synthesis.
4. **Citation Management** — https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/skills/citation-management — verify every paper and claim, no invented citations.
5. **Anti-Defensive Writing** — https://github.com/Kiterlin/anti-defensive-writing — cut repetitive apologies/qualifiers without suppressing real limitations.
6. **Token Optimization** — https://github.com/bm629/agent-skills/tree/main/skills/token-optimization — narrow retrieval, concise ACP handoffs, reuse verified materials.
7. **Ponytail** — https://github.com/DietrichGebert/ponytail — reuse existing token-efficient workflow as applicable, never pretend a missing capability executed.

If an underlying skill is unavailable, disclose this in the audit rather than claiming it ran. Neither this upgrade nor its references copy or install any upstream full skills.

### Two original JMU guides — still mandatory for manuscript tasks

- *Empirical Research Papers: An Overview*: https://www.jmu.edu/learning/writing-center/_files/link-library/empirical/empirical_research_article_overview.pdf?jmu_redir=r_uwc
- *Introductions for Empirical Research Papers: An Overview*: https://www.jmu.edu/learning/writing-center/_files/link-library/empirical/introduction_and_lit_review_overview.pdf?jmu_redir=r_uwc

Use these for section roles, research question and evidence alignment, and the introduction/literature relationship. The second guide is primarily for Introduction/literature; do not force its structure onto Results or Discussion.

## 2. The mandatory ECONOMIC INTERPRETATION GATE

Before drafting or revising a manuscript, and again before final PASS, produce a compact **Economic Argument Matrix**, with one row per main finding:

| Field | What the agent must actually answer |
|---|---|
| Economic phenomenon | What happened in the economy, to whom/where/when, in substantive units? |
| Puzzle / research question | Why does it matter, and what needs explanation beyond the arithmetic? |
| Main result and magnitude | What is directly established by this study (sample, years, outcome, quantitative size)? |
| Most informative economic comparison | What source-verified pair, group, benchmark, time comparison, or scale makes the result intelligible? Is it representative of the full sample? |
| Candidate economic mechanism(s) | Which *specific* economic forces could account for it: structural composition, energy mix, technology, prices/incentives, demand, urbanization, firm behavior, regulation, etc.? Why, in economic terms? |
| Observable predictions | If mechanism M operated, which **distinctive** observable X would differ from a competing mechanism? |
| Evidence in this study | Which variables, comparisons, tables or figures support/challenge X? Distinguish accounting identity from mechanism testing. |
| Verified external evidence | Which relevant papers report findings on M/X, and with what geography, emissions boundary, method and identification? |
| Evidence status | Label: demonstrated in this study / descriptively consistent in this study / established only in external literature / plausible but untested / contradicted or unsupported. |
| Economic meaning | What follows for understanding adjustment, distribution, growth, constraints or trade-offs? |
| Implication and boundary | Which conditional assessment/policy implication follows? What would require new data or causal identification? |

**Blocking rule:** An empirical section that repeats indexes, coefficients, sensitivity directions or statistical definitions but cannot name the **economic meaning** of its headline findings receives `ECONOMIC_INTERPRETATION_HOLD`. A Discussion that lists many plausible mechanisms with no mechanism-specific literature or evidence also fails. Resolve with sourced interpretation, a bounded additional test **only with authorization**, or explicitly identify the unresolved economic question rather than fabricating an answer.

### Evidence-level language discipline

- **Directly established:** “In the observed panel, ...”; report actual scope, magnitude and uncertainty/type of comparison.
- **Study-level descriptive consistency:** “The pattern is consistent with ..., but the available variables do not isolate this channel.”
- **External literature only:** “Study X links A to B in context Y; this offers a possible explanation, not a mechanism identified here.”
- **Untested hypothesis:** “One possible account is ...; distinguishing it would require sectoral output and fuel data.”
- **Causally identified:** reserve “causes/impact/effect of policy X” for a design and assumptions that justify them.

Never turn a Kaya/LMDI term into a measured technology, policy or industrial-composition effect merely by renaming the residual. Avoid giving significance tests to accounting identities or treating descriptive spatial patterns as spillover effects.

**Narrative integrity:** A persuasive economic explanation does not mean a positive finding, predetermined hypothesis support or a tidy causal story. Preserve contradictory outcomes and alternative explanations.

## 3. Economic question and paper spine (Introduction gate)

**v2.3 Introduction Question & Contribution Check (mandatory for substantial Introduction writing or revision):** Freeze a short, evidence-bound question–answer–contribution map before drafting. Separate (a) the economic phenomenon and its stakes, (b) the genuinely unresolved empirical question, (c) the answer the approved Results can supply, and (d) the marginal understanding added relative to the closest verified studies. Do not use an accounting identity, a definitional coexistence (e.g., growing output alongside falling emissions intensity), or the combination of established methods as the entire research puzzle or as independent scholarly novelty. If the question is descriptive or accounting-based, make the substantive variation, magnitude, heterogeneity, or duration that remains unknown explicit. Do not promise policy causality or mechanisms beyond the available design. The Introduction's contribution must compare both sides: specific prior work and the paper's specific new evidence. A within-region common observation base can be an honest contribution **when it reveals a consequential comparison or assessment**, but the words 'integrated framework' alone are not a sufficient contribution claim.

**Concrete opening and proportionate findings preview (v2.3.0):** Lead with a specific economic outcome, observable tension, or credible stylized fact wherever possible. Do not let a generic label such as “the aggregate and distributional dimensions of adjustment” substitute for stating what happened in the economy. It may follow a concrete opening as conceptual framing. Preview only the one or two headline facts essential to understanding the main answer and contribution; do not compress every main result, robustness variant, classification count, or number into the Introduction's closing paragraph. This is a relevance rule, not a numerical quota: keep an additional magnitude if omitting it would obscure the answer.

Apply Keith Head's *Introduction Formula* as a **logic**, not a rigid paragraph count:

**Hook (important/puzzling economic fact) → Answerable Question → Critical Antecedents → Specific Value Added → Short Roadmap.**

Add a **closed-loop check**: the principal question explicitly promised in the introduction must be substantially answered by the Results, interpreted economically in Discussion, and answered in Conclusions. Flag a **bait-and-switch** if the paper promises causes or how to solve an economic problem but offers only descriptive indices. Either strengthen the evidence with approval or narrow the promise truthfully.

Before approval, the lead agent must be able to write:

- **One-sentence economic puzzle:** an actual tension, not “few studies have examined X.”
- **One-sentence answer:** what the study has demonstrably learned.
- **One-sentence value added:** what a reader can now distinguish, understand, measure or evaluate that was previously unclear.

The paper should have **one main intellectual spine and roughly one to three coordinated claims**. Several hypotheses need not become unrelated papers; place technical robustness and reporting details in service of the central economic question. Do not invent causal novelty or require the literature review to be merged into the Introduction when the researcher has an approved separate section or a target journal expects one.

**Mandatory cross-paper hypothesis rule (v2.3; all future articles):** Do **not** frame robustness, measurement sensitivity, source-vintage differences, sample omissions, alternative statistical definitions, influential cases, or model-diagnostic checks as a standalone numbered research hypothesis, **including 'H4: Measurement Sensitivity'** or any equivalent `Hn`. These are supporting credibility/robustness analyses, not substantive economic hypotheses merely because their outcome can vary. Retain them in Data/Methods, Robustness/Results, and limitations as applicable, without assigning hypothesis numbering or claiming 'H4 supported'. Reserve numbered hypotheses for substantive, evidence-answerable economic propositions; even these should be called *descriptive expectations* where their design warrants rather than misrepresenting confirmatory causal tests. If an approved legacy manuscript contains a sensitivity H4, flag it for author-approved cross-section migration (Section 2, Methods, Results, Discussion, Conclusions, and references); **do not silently remove it or change protected text**. This rule generalizes across papers and does not presume there must be exactly three substantive hypotheses.

## 4. Literature used to EXPLAIN economics, not decorate Results

**v2.3 Literature Synthesis & Contribution Positioning Check (mandatory for substantive Literature Review):** Organize around the paper's answerable economic questions and the few closest literature streams. Before prose, make a compact relation matrix for each central study: actual economic finding; unit/period/outcome/design; relationship to other findings (agreement, divergence, different objects/assumptions); limit of transfer; unresolved substantive issue; marginal contribution the present evidence can establish. Every principal subsection should synthesize *relationships among findings*, not merely list author–year summaries; explain apparent disagreement by differing geography, outcomes, identification, periods, or definitions **only when supported**. Explicitly distinguish city dispersion, formal convergence, and accounting identities when relevant; do not manufacture conflicts or claim novelty from a missing citation. Place extended equations, indicator definitions, source-inventory comparisons and technical sensitivity catalogues primarily in Data/Methods or robustness, unless they are themselves central to a genuine measurement-research question. Do not impose citations on mathematical definitions or the paper's own results; do verify each nontrivial external empirical proposition. Full instructions and transferable examples: `references/introduction-literature-argument-guide.md`.

For each pivotal external work, extract: exact citation/DOI; question; sample/period; outcome and economic unit; method; proposed/tested mechanisms; actual result; applicable scope; fit/mismatch with the current study. Prefer reading full text for mechanism claims. An abstract may support a limited claim **only if the abstract actually says it**; otherwise flag source-depth limits and obtain the paper.

Use literature for four jobs: **theory/prediction, empirical mechanism evidence, comparison with the current finding, and implication/boundary**. Never assume that finding the same sign establishes the same economic channel across incompatible emissions scopes, periods or cities.

At least one paragraph in Discussion should compare a **mechanism or economically meaningful interpretation** from relevant literature with the new study—not merely say that dispersion rose/fell similarly. Competing explanations are valuable; do not cite five papers merely to build a one-sided story.

**If authors/report/data lack mechanism evidence:** state that and identify which additional observations would be discriminating. Do not fabricate local industrial structure or infer factory behavior from gridded emissions alone.

### 4.1 Mandatory claim-level mechanism citation gate (v2.1)

**Default scholarly rule:** **Each distinct, important economic interpretation or proposed explanatory mechanism in Discussion should be supported by approximately one or two directly relevant, verified studies.** For a connected cluster of claims about the **same mechanism**, **one to three complementary, nonredundant studies** usually suffice. These are evidence-quality heuristics, **not mechanical minimum counts, citation quotas, or an instruction to cite every sentence**. Prefer one authoritative study that directly establishes a claim to multiple superficial citations. A pivotal or contested claim may require more thorough triangulation or explicit discussion of disagreement.

**Claim proximity and exact fit:** Put the citation close to the economic proposition it actually supports. Identify what the source studied (outcome, mechanisms/variables, population, geography, period, design) and what it actually found. Do not attach a stack of author–years to the end of a paragraph containing several unsupported mechanisms, or use a broad review article to attribute a specific empirical estimate it did not report. Two sources testing the same claim may reinforce it; evidence from different settings or methods should be framed as complementary rather than identical.

**Citation ledger required for each major mechanism claim:**

| Claim ID & exact sentence | Mechanism / predicted observation | Direct source and locator (DOI/URL + section/page/table when available) | Verified original finding and research design | Relevance / scope difference | Evidence level S1–S5 | Draft citation placement | Cursor verdict |
|---|---|---|---|---|---|---|---|

1. Extract the proposed **economic** claim and separate a source-backed mechanism, a theoretical possibility, and a locally established fact. A paper supporting the *importance of sectoral emissions decomposition* does not automatically establish that a city's *sector mix caused* its observed intensity gap.
2. Verify cited sources at **claim level**, using original full-text Results/Discussion or documented abstract-only evidence. Resolve DOI, author and year; make sure the cited article actually evaluates or explicitly develops that mechanism. Check for sign, heterogeneity, time coverage, sector and emission-boundary incompatibilities.
3. For each independent key mechanism (e.g., production specialization; energy/fuel requirements and efficiency; technology diffusion; land use and demographics), seek approximately **1–2 direct supporting studies** where available. For an integrated paragraph or cluster about one channel, **1–3 complementary studies** is generally appropriate. Add more only for a genuine controversy or distinct additional claim, never to meet a quota.
4. State **what the source supports** and **what it does not establish for the present sample**. External evidence can motivate an economic interpretation but cannot be treated as identified effects in an untested local panel. If source evidence is weak or absent, downgrade the claim to a labeled hypothesis or omit it; **do not add invented or loosely related citations**.
5. Seek contrary or competing evidence when available. Mechanisms should not become a one-sided sequence of convenient positive findings.
6. Make the narrative flow **local observed result → proposed economic channel → specific source-based evidence → what is/not verified here → conditional implication**. A brief transition may combine links; avoid repetitive templates and citation dumping.

**Which passages need outside citations?** The manuscript's **own computed findings** are supported by its verified tables/figures and normally do not need external citations for each sentence; mathematical definitions and a clearly marked author's inference are not automatically citation-required. Claims about **external empirical findings, specific economic channels, institutional settings, policy effectiveness, industry characteristics or contested theories** need appropriately matched support. In Results, prioritize study data and cite external literature only when making a substantive external claim; in Discussion, actively compare mechanisms with verified studies.

**Independent referee failure conditions:** `MECHANISM_CITATION_HOLD` for (a) a central explanation with no relevant source or no evidence-status label, (b) a citation that does not support the adjoining proposition, (c) unverified/fabricated references, (d) a stack of unrelated sources disguising an unsupported statement, or (e) external correlation presented as proof of this study's city-specific mechanism. The reviewer must propose a concrete correction: verify/replace the source, narrow the claim, label an open explanation, or seek author-approved additional evidence. This is a component of the broader `ECONOMIC_INTERPRETATION_HOLD`; noncritical incomplete supporting citations should be explicitly logged for remediation, not automatically concealed as PASS.

## 5. Section-specific writing requirements

### Introduction — important economic problem

Start with a **concrete economic outcome or tension**, rather than an unexplained abstract “dimension” label. State a question answerable by the available design, specify study scope and high-level approach, give **a proportionate preview of only the decisive findings**, place them relative to closest predecessors, and explain **why they matter economically**. Avoid listing every result or numerical magnitude in the final Introduction paragraph. Use a tailored roadmap only when helpful to the journal and reader.

### Literature Review & hypotheses — theory with observable implications

Synthesize verified *findings and relationships* among prior studies, not an author-year list, unsupported opinions or several paragraphs describing statistics. Explain what is known, what differs across research settings/designs, what remains empirically unresolved, and what this manuscript can genuinely add. Each **substantive economic hypothesis or descriptive proposition** should contain: **economic intuition, expected observable pattern, evidence criterion, and interpretation boundary**. Distinguish causal hypotheses from descriptive analytical expectations. Do not present sensitivity/robustness checks as numbered hypotheses (see Section 3); keep them as supporting analyses. Include sector, geography and price-content comparability when relevant.

### Data & empirical framework — identify the object, not just the tools

Explain what economic behavior or outcome each variable measures, and why its definition fits the question. Distinguish nominal/real output; territorial/consumption emissions; absolute emissions/intensity; GDP-weighted aggregate/equal-city dispersion. State whether an analysis is an identity, a descriptive statistic, an association, or a causal estimator. Equations belong here or in an appendix; do not crowd Discussion with their algebra.

### Results — phenomenon → verified magnitude → informative comparison → meaning (v2.2)

**Results is evidence-driven economic storytelling, not a table-by-table readout.** State the economically substantive finding first, quantify it, choose an informative contrast, refer to its source table/figure, explain exactly what the observed evidence establishes, then transition to the mechanism question for Discussion. Vary paragraph structure naturally; do not fill a rigid six-sentence template.

**Mandatory pre-draft step: the Substantive Economic Magnitude and Comparison Gate.** Before writing a substantial Results subsection, inspect the approved result table(s) and identify candidate reader-relevant comparisons, such as: a high-versus-low level, before-versus-after ratio, absolute versus proportional change, within-unit versus between-unit movement, group/sector contrasts, observed versus benchmark magnitude, classification versus underlying continuous changes, or a sensitivity case that changes a substantive conclusion. Select the *smallest set* that explains the important economic phenomenon, normally one primary comparison plus a complementary or contrasting case **when supported**. Never fabricate a contrast to satisfy a quota; never present an extreme pair as the entire regional distribution.

**Derived economic magnitude, only when legitimate.** Calculate informative ratios, gaps, percentage-point changes, units, and offsets from verified source numbers using a reproducible check. Confirm numerator/denominator units, time periods, price base, sample and emissions boundary are comparable; guard against unstable near-zero denominators, mechanically linked quantities and misleading averages. Record formula, inputs, source table and rounding. A derived magnitude is a transparent description, **not a new econometric result or causal mechanism**. When no reliable comparison is possible, say so; do not invent it.

**Two-part disclosure:** (a) what a typical reader should learn about the economy; (b) why this comparison—not merely the value or statistical definition—matters for the paper's research question. Explain how the finding modifies the substantive claim: persistence versus catch-up, relative progress versus absolute pressure, balanced versus concentrated contribution, heterogeneous growth configurations, or sensitivity of an economically relevant classification. Preserve genuine counterexamples and uncertainty rather than selecting only dramatic pairs.

**Placement:** Results prioritize the study's own verified tables/figures and economical explanation of observed facts; keep untested production, energy, demographic and policy *mechanisms* for Discussion (with literature). Avoid repeating every equation, table row, map color, or technical robustness check. Explain a map's relevant economic geography only if the mapped variable supports it; maps alone do not demonstrate structural specialization or spatial spillovers. End with **one specific unanswered economic explanation**, without repeating it in several transitions.

**Mandatory Result subsection test:** Could a reader without the formulas answer (i) *what happened?*, (ii) *how large was it compared with what?*, (iii) *which units or periods differed, and is the example representative?*, (iv) *why does it change the economic assessment?*, and (v) *what does the paper not establish?* If a material answer is missing despite available data, assign `RESULTS_EXPOSITION_HOLD` and repair before polishing. This is a named sub-gate of `Economic interpretation: PASS/HOLD`; it does **not** change the existing three final status fields.

For full drafting logic, anti-patterns and transferable examples, read **`references/results-economic-comparison-guide.md`** when revising Results. Read it selectively; it is not a new external Skill.

### Discussion — explain WHY; compare; distinguish; infer proportionately

Every substantive Discussion subsection should contain the following argumentative steps in coherent prose (not repetitive labeled mini-lists):

1. **Economic interpretation:** What economic reality does the result illuminate or complicate?
2. **Mechanism candidates:** Specify one or two theoretically meaningful pathways and their distinctive predictions.
3. **Evidence confrontation:** Compare verified external evidence and any relevant study data. Say which pathways remain speculative.
4. **Competing interpretations / trade-offs:** What else could produce the same pattern? What is the relevant economic constraint, distributional trade-off or growth–emissions tension?
5. **Practical meaning:** What follows for performance assessment, institutional decision making, or **conditional** policy choice? What does not follow?

Do not substitute a long description of trimming, mapping, price revisions or outlier removal for economic interpretation. Robustness/measurement sensitivities matter most when they change an economic conclusion or policy ranking; technical details may be moved to appendices **without concealing material sensitivity**. Avoid generic recommendations (“encourage innovation”) unless linked to an actual mechanism, implementation condition, or evidence gap.

For discussions of climate and carbon-neutrality objectives, distinguish **carbon intensity improvement**, **absolute territorial fossil-CO2 reductions**, and **economy-wide net zero**. The latter additionally involves scope, other greenhouse gases, sinks and future trajectories not necessarily measured here.

### Conclusions — answer, synthesize, qualify, finish

Answer the Introduction's central question in plain economic language. State the one to three decisive findings and why they matter, offer evidence-proportionate implications and a specific next research question. Do not repeat an extensive statistical audit or write a wish list of untested policy prescriptions. Keep the limitations accurate but not defensive.

### Abstract/title/figures

The title and abstract should convey the economic phenomenon and real contribution rather than only a method inventory. Figures and tables should each support a claim: put the substantive finding before long display-by-display narration; keep units, baselines, and spatial boundaries explicit.

## 6. Mechanism pathway: practical but scientifically restrained

Following Bellemare's pragmatic mechanisms discussion, apply **the strongest feasible evidence level**, never an automatic requirement to identify causal mediation:

1. **Theoretically plausible channel**: show the economic logic and what would be observed.
2. **Descriptive test (when available/approved)**: sector shares, output/emissions intensities, fuel mix, R&D, urbanization, or credible comparisons. Label descriptive evidence as such. One well-designed discriminating comparison beats numerous ad hoc regressions.
3. **Competing mechanism check**: document at least one alternative that could also explain the same pattern.
4. **Unverifiable with present data**: make the data need concrete; do not infer a specific industry's contribution from aggregate city carbon intensity.
5. **Formal causal mechanism**: only with adequate design, data and assumptions, and explicit researcher approval.

**Researcher gate for new analysis:** If stronger explanation requires new city variables, panel models, sectoral decomposition or mechanism tests, write a bounded proposal with expected contribution, source, feasibility, validity and potential sensitivity. Stop and seek approval. Do **not** run exploratory specifications until a favorable result emerges.

## 7. Journal style and generalizability

Borrow from `iik1/academic_writing_skills` the **field baseline first, target-journal layer later** principle. Use a neutral economics/energy-economics voice unless the author names a target journal. Treat claims about particular journals' usual lengths, causal-identification preferences, and published style as **descriptive summaries**, not binding policies. Check the target journal's current official author instructions for actual limits, submission format and data-sharing rules. Do not blindly transplant FT50 causal-identification templates or finance-specific standards into a descriptive environmental accounting paper.

## 8. Codex–Cursor workflow with TWO distinct quality gates

1. **Scope and version lock:** Find latest approved manuscript/data; classify paper type and protected content; confirm language, requested section, output and no-change boundaries.
2. **Economic argument map FIRST:** Map each finding to phenomenon, **the most informative comparable magnitudes**, theoretical possibilities, actual evidence, sources, competing explanations and bounded implications (Section 2). For Results, create a short candidate-comparison ledger from approved tables before drafting. Mark holes; do not hide them with fluent prose.
3. **Evidence/source verification:** Build the v2.1 claim-to-source ledger for **each important Discussion mechanism**, verify original passages and final calculation tables, assess direct relevance and scope, and avoid reusing citations copied from earlier LLM output without checking.
4. **Draft or targeted revision:** Write around the research question; preserve approved empirical conclusions unless the researcher authorizes a scientific revision. For Introduction/Literature Review work, apply the question–answer–contribution map and literature relation matrix from `references/introduction-literature-argument-guide.md`; identify legacy robustness-as-hypothesis issues without silently modifying approved downstream sections.
5. **Economics + literature gate — Lead check:** For Introduction, does the question go beyond identities/method lists, and does the verified contribution answer it? For Literature Review, are major studies compared on findings, study objects and limitations, with a justified marginal contribution? Are robustness and sensitivity checks unnumbered and subordinate rather than treated as independent hypotheses? For Results, did the agent select and validate a representative, informative economic comparison (or document why none applies), rather than merely enumerate statistics? Does each key Results/Discussion segment explain substantive meaning, not only method and numerical sensitivity? Does every important Discussion mechanism have suitably placed, verified direct evidence (normally 1–2 per distinct claim or 1–3 complementary works per channel cluster), or an explicitly downgraded evidence status? If not, revise or HOLD **before language polishing**.
6. **Anti-Defensive-Writing Pass 1:** Revise the current full draft and log actual changes; preserve limitations and epistemic labels.
7. **Independent Cursor economics referee via REAL ACP:** For Introduction/Literature work, Cursor must inspect the actual frozen Results/Discussion (not only the abstract), the closest source studies, and the question–answer–contribution and literature matrices; independently judge whether the contribution is incremental rather than a list of methods, whether literature synthesizes findings, and whether sensitivity is incorrectly numbered as a hypothesis. Cursor also reads relevant source, Results, **the candidate-comparison ledger and its raw-input arithmetic**, Discussion and mechanism evidence. Must raise specific `ECONOMIC_INTERPRETATION`, `MECHANISM_CITATION`, `COMPETING_MECHANISMS`, `LITERATURE_FIT`, `POLICY_PROPORTIONALITY` concerns alongside numeric, causal, and prose checks. Require concrete paragraph locations and verification coverage. Do not fabricate independent work.
8. **Codex adjudication:** Resolve Critical/Major issues with evidence and tracked actual changes. Disagreement persists as a documented limitation or HOLD, not automatic PASS.
9. **Anti-Defensive-Writing Pass 2:** Review the *revised* manuscript, independently from Pass 1; cut repeated cautions and mechanical prose without weakening scientific boundaries.
10. **Final dual gate:** Report **Scientific integrity status** and **Economic interpretation status** separately. Only `FINAL PASS` when both pass, claim-level mechanism citation support passes, source/citation consistency passes, and real ACP evidence exists. Otherwise `PASS WITH DISCLOSED LIMITATIONS` when nonblocking issues remain, or `HOLD` for material gaps.

**Non-writing tasks:** Pure data/source audits do not need the two prose passes; apply numerical/source integrity requirements and record why writing requirements are inapplicable.

## 9. Mandatory independent economics-referee questions

Cursor must answer, with passage references:

- What is the one-sentence economic question and what does the article establish? Which meaningful uncertainty remains after accounting definitions or indicator arithmetic are known?
- Does the Introduction promise a causal/policy answer not delivered by the actual design? Is 'using several methods on a common dataset' claimed as novelty without naming the new economic insight compared with closest research?
- Does each Literature Review stream state actual prior findings, agreements/differences and design/geography limits, then show the specific question the current evidence can address? Are methodological definitions wrongly substituting for literature synthesis?
- Are robustness/sensitivity checks (including any historical 'H4 Measurement Sensitivity') incorrectly given standalone `Hn` status? If legacy, is there a bounded migration proposal rather than silent removal?
- Which central result is merely a change in a metric, and how has it been translated into a substantive economic fact? For each Results subsection, was the most reader-informative *valid* ratio, gap, change or contrast considered and accurately reported? If an obvious benchmark was omitted, why?
- For observed regional differences, what plausible **economic** explanations are distinguished? Which have local evidence, which only literature support, and which are unresolved?
- Where does the paper interpret a composition/technology/policy channel without measuring it?
- For every important economic mechanism, are the closest one or two (or one to three complementary studies per mechanism cluster) directly relevant, verified and cited alongside the proposition? Does each citation actually study/support the attributed channel, and is it comparable to the current emission boundary and period?
- What competing explanation would remain even if the preferred mechanism were true?
- What economically relevant implications survive the spatial, price, sample and time-window sensitivity checks?
- Are proposed interventions feasible/evidenced, or are they generic slogans or claims about carbon neutrality unsupported by the data?
- Would an environmental economist reading only Introduction, core Results, Discussion and Conclusions learn a meaningful new fact about the economy, or only about the analysis method?

A missing answer to a *core* question is a **Major** item; a central unsupported mechanism, misattributed source or causal/policy conclusion is **Critical**. Do not label the result final simply because the text is concise, properly cited and numerically correct.

## 10. Task-scaled outputs and reference loading

Minimum for a substantial draft/revision: final manuscript section, **the Results comparison-and-magnitude ledger when Results are revised**, **Economic Argument Matrix**, claim-to-original-source ledger with mechanism-by-mechanism citation adequacy and placement check, actual Cursor referee report, Codex adjudication, separate pass-1/pass-2 logs, and final **dual-gate** memo. Version-lock files; preserve original until approval. In a small prose-polish task, a concise inline matrix and brief log suffice.

For nuanced instructions and examples, read **only when relevant**:

- `references/introduction-literature-argument-guide.md` — **v2.3 Introduction/Literature-only** research-question validity, prior-work contribution positioning, literature synthesis, hypothesis taxonomy, and independent Cursor test.
- `references/results-economic-comparison-guide.md` — **v2.2 Results-only (retained unchanged)** source-to-claim comparison selection, magnitude verification, examples and independent review rubric.
- `references/economic-argument-guide.md` — practical argument structure and the descriptive-mechanism ladder; results/discussion paragraph pattern and Zhejiang illustration.
- `references/referee-and-source-checklist.md` — economics referee rubric, claim-level mechanism citation audit, source limits, and copy-ready prompts.
- `REFERENCES_AND_SKILLS.md` — exact seven upstream Skills, both JMU guides, supplementary economic-writing sources, and dependency versus inspiration distinctions.

These are **original synthesized rules based on cited sources** (see provenance notes); they are not verbatim replacements for third-party skills. Source consultation and user-approved evidence always take precedence.

## 11. Token discipline and final decision

Load the latest manuscript and only the original results/sources needed to evaluate the paragraph. Send Cursor small file paths and explicit claims to check. Use the seven skills already installed; do not paste entire upstream manuals. For Results work, read the narrow comparison guide and reuse existing verified result tables. The 2-stage economics + prose audit is worth more than extra speculative literature hunting.

**Final acceptance statement must report the two existing fields plus an explicit third field `Mechanism citation support: PASS/HOLD/NOT_APPLICABLE`:** `Scientific integrity: PASS/HOLD` and `Economic interpretation: PASS/HOLD`. A missing mechanism test need not block a *descriptive* paper if the argument accurately distinguishes observed economic patterns from unresolved causes and provides an evidence-grounded interpretation. Unsupported answers to why/how or hollow policy claims **do** block publication-ready writing.