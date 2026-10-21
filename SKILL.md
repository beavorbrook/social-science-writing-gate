---
name: social-science-writing-gate
description: Coordinate seven existing research/writing skills, two JMU guides and two anti-defensive-writing passes; enforce an economics argument gate and claim-level, source-verified literature support for key economic mechanisms in Results and Discussion. Use for drafting, reviewing and integrating economics and environmental-economics manuscripts with Codex and Cursor.
---

# Social Science Writing Gate — Economics-Enhanced v2.1

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

Apply Keith Head's *Introduction Formula* as a **logic**, not a rigid paragraph count:

**Hook (important/puzzling economic fact) → Answerable Question → Critical Antecedents → Specific Value Added → Short Roadmap.**

Add a **closed-loop check**: the principal question explicitly promised in the introduction must be substantially answered by the Results, interpreted economically in Discussion, and answered in Conclusions. Flag a **bait-and-switch** if the paper promises causes or how to solve an economic problem but offers only descriptive indices. Either strengthen the evidence with approval or narrow the promise truthfully.

Before approval, the lead agent must be able to write:

- **One-sentence economic puzzle:** an actual tension, not “few studies have examined X.”
- **One-sentence answer:** what the study has demonstrably learned.
- **One-sentence value added:** what a reader can now distinguish, understand, measure or evaluate that was previously unclear.

The paper should have **one main intellectual spine and roughly one to three coordinated claims**. Four empirical hypotheses need not become four unrelated papers; place technical robustness and reporting details in service of the central economic question. Do not invent causal novelty or require the literature review to be merged into the Introduction when the researcher has an approved separate section or a target journal expects one.

## 4. Literature used to EXPLAIN economics, not decorate Results

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

Start with a consequential outcome, tension, or stylized fact. State a question answerable by the available design, specify study scope and high-level approach, give the main concrete finding, place it relative to closest predecessors, and explain **why the finding matters economically**. Finish with a tailored roadmap. Avoid promising causal channels or carbon neutrality pathways when only territorial fossil-CO2 comparisons are measured. Revisit the Introduction after Results and Discussion are settled.

### Literature Review & hypotheses — theory with observable implications

Synthesize prior studies around competing explanations, not an author-year list. Each hypothesis or descriptive proposition should contain: **economic intuition, expected observable pattern, evidence criterion, and interpretation boundary**. Distinguish a formal testable causal hypothesis from a descriptive analytical expectation. Include sector, geography and price-content comparability when relevant.

### Data & empirical framework — identify the object, not just the tools

Explain what economic behavior or outcome each variable measures, and why its definition fits the question. Distinguish nominal/real output; territorial/consumption emissions; absolute emissions/intensity; GDP-weighted aggregate/equal-city dispersion. State whether an analysis is an identity, a descriptive statistic, an association, or a causal estimator. Equations belong here or in an appendix; do not crowd Discussion with their algebra.

### Results — phenomenon → magnitude → meaning

**Required order for each main subsection**: (1) state the economically substantive observed fact, (2) report an intuitive size and benchmark, (3) refer to the relevant table/figure, (4) give a brief interpretation tied to the question, (5) explain heterogeneity/robustness only insofar as it changes a substantive conclusion, (6) point forward to a mechanism/implication question addressed later. Report unsupported mechanisms as open, not as verified findings.

Results must not end at “CV changes sign under city omission.” Also explain which substantive inter-city comparison depends on that city and **why it matters for the reader's assessment**; reserve extended method diagnostics for an appendix when appropriate. In descriptive work, “economic significance” means magnitude, distribution, real-world benchmark and consequences—**not necessarily a p-value or regression coefficient**.

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
2. **Economic argument map FIRST:** Map each finding to phenomenon, theoretical possibilities, actual evidence, sources, competing explanations and bounded implications (Section 2). Mark holes; do not hide them with fluent prose.
3. **Evidence/source verification:** Build the v2.1 claim-to-source ledger for **each important Discussion mechanism**, verify original passages and final calculation tables, assess direct relevance and scope, and avoid reusing citations copied from earlier LLM output without checking.
4. **Draft or targeted revision:** Write around the research question; preserve approved empirical conclusions unless the researcher authorizes a scientific revision.
5. **Economics + literature gate — Lead check:** Does each key Results/Discussion segment explain substantive meaning, not only method and numerical sensitivity? Does every important Discussion mechanism have suitably placed, verified direct evidence (normally 1–2 per distinct claim or 1–3 complementary works per channel cluster), or an explicitly downgraded evidence status? If not, revise or HOLD **before language polishing**.
6. **Anti-Defensive-Writing Pass 1:** Revise the current full draft and log actual changes; preserve limitations and epistemic labels.
7. **Independent Cursor economics referee via REAL ACP:** Cursor reads relevant source, Results, Discussion and mechanism evidence. Must raise specific `ECONOMIC_INTERPRETATION`, `MECHANISM_CITATION`, `COMPETING_MECHANISMS`, `LITERATURE_FIT`, `POLICY_PROPORTIONALITY` concerns alongside numeric, causal, and prose checks. Require concrete paragraph locations and verification coverage. Do not fabricate independent work.
8. **Codex adjudication:** Resolve Critical/Major issues with evidence and tracked actual changes. Disagreement persists as a documented limitation or HOLD, not automatic PASS.
9. **Anti-Defensive-Writing Pass 2:** Review the *revised* manuscript, independently from Pass 1; cut repeated cautions and mechanical prose without weakening scientific boundaries.
10. **Final dual gate:** Report **Scientific integrity status** and **Economic interpretation status** separately. Only `FINAL PASS` when both pass, claim-level mechanism citation support passes, source/citation consistency passes, and real ACP evidence exists. Otherwise `PASS WITH DISCLOSED LIMITATIONS` when nonblocking issues remain, or `HOLD` for material gaps.

**Non-writing tasks:** Pure data/source audits do not need the two prose passes; apply numerical/source integrity requirements and record why writing requirements are inapplicable.

## 9. Mandatory independent economics-referee questions

Cursor must answer, with passage references:

- What is the one-sentence economic question and what does the article establish?
- Does the Introduction promise a causal/policy answer not delivered by the actual design?
- Which central result is merely a change in a metric, and how has it been translated into a substantive economic fact?
- For observed regional differences, what plausible **economic** explanations are distinguished? Which have local evidence, which only literature support, and which are unresolved?
- Where does the paper interpret a composition/technology/policy channel without measuring it?
- For every important economic mechanism, are the closest one or two (or one to three complementary studies per mechanism cluster) directly relevant, verified and cited alongside the proposition? Does each citation actually study/support the attributed channel, and is it comparable to the current emission boundary and period?
- What competing explanation would remain even if the preferred mechanism were true?
- What economically relevant implications survive the spatial, price, sample and time-window sensitivity checks?
- Are proposed interventions feasible/evidenced, or are they generic slogans or claims about carbon neutrality unsupported by the data?
- Would an environmental economist reading only Introduction, core Results, Discussion and Conclusions learn a meaningful new fact about the economy, or only about the analysis method?

A missing answer to a *core* question is a **Major** item; a central unsupported mechanism, misattributed source or causal/policy conclusion is **Critical**. Do not label the result final simply because the text is concise, properly cited and numerically correct.

## 10. Task-scaled outputs and reference loading

Minimum for a substantial draft/revision: final manuscript section, **Economic Argument Matrix**, claim-to-original-source ledger with mechanism-by-mechanism citation adequacy and placement check, actual Cursor referee report, Codex adjudication, separate pass-1/pass-2 logs, and final **dual-gate** memo. Version-lock files; preserve original until approval. In a small prose-polish task, a concise inline matrix and brief log suffice.

For nuanced instructions and examples, read **only when relevant**:

- `references/economic-argument-guide.md` — practical argument structure and the descriptive-mechanism ladder; results/discussion paragraph pattern and Zhejiang illustration.
- `references/referee-and-source-checklist.md` — economics referee rubric, claim-level mechanism citation audit, source limits, and copy-ready prompts.
- `REFERENCES_AND_SKILLS.md` — exact seven upstream Skills, both JMU guides, supplementary economic-writing sources, and dependency versus inspiration distinctions.

These are **original synthesized rules based on cited sources** (see provenance notes); they are not verbatim replacements for third-party skills. Source consultation and user-approved evidence always take precedence.

## 11. Token discipline and final decision

Load the latest manuscript and only the original results/sources needed to evaluate the paragraph. Send Cursor small file paths and explicit claims to check. Use the seven skills already installed; do not paste entire upstream manuals. The 2-stage economics + prose audit is worth more than extra speculative literature hunting.

**Final acceptance statement must report the two existing fields plus an explicit third field `Mechanism citation support: PASS/HOLD/NOT_APPLICABLE`:** `Scientific integrity: PASS/HOLD` and `Economic interpretation: PASS/HOLD`. A missing mechanism test need not block a *descriptive* paper if the argument accurately distinguishes observed economic patterns from unresolved causes and provides an evidence-grounded interpretation. Unsupported answers to why/how or hollow policy claims **do** block publication-ready writing.