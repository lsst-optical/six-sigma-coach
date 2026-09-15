# Six Sigma Tool Router

Choose tools by the question they answer. A stage is a common home, not an exclusive boundary.

## Define

| Tool | Use when | Required input | Decision output |
|---|---|---|---|
| Project Charter | value, authority, goal, and governance are unclear | business case, baseline, target, sponsor | approved problem, objective, team, milestone |
| Scope Statement | the project may expand or ownership is disputed | start/stop, product/process boundary | in-scope and out-of-scope boundary |
| WBS | a defined outcome must become manageable deliverables | scope and deliverables | work packages and acceptance criteria |
| Gantt | dependencies and timing must be coordinated | WBS, durations, predecessors, resources | milestones and critical-path view |
| SIPOC | the end-to-end process and customers are unclear | high-level process | suppliers, inputs, 5–7 steps, outputs, customers |
| Kano | investment among customer needs is unclear | paired customer survey evidence | must-be, performance, attractive, indifferent, reverse needs |
| CTQ Tree | VOC is subjective or not measurable | customer language and need drivers | operational CTQs and specification intent |
| QFD / House of Quality | needs must be translated and prioritized across functions | WHATs, importance, HOWs, evidence | relationships, technical priorities, conflicts, targets |

Do not use QFD to fabricate customer priorities or write engineering solutions as VOC.

## Measure

| Tool | Use when | Required input | Decision output |
|---|---|---|---|
| Data Collection Plan | data provenance or sampling is uncertain | decision question, variables, process strata | definitions, source, sample, owner, exclusions |
| Run Chart | time behavior is hidden by aggregate statistics | ordered observations | trend, shift, oscillation, mixture hypotheses |
| MSA / GRR | measurement error may mask product/process differences | representative parts, appraisers, repeats, method | repeatability, reproducibility, bias/linearity/stability fitness |
| Normality / Distribution Diagnosis | a model depends materially on distribution | ordered and stratified continuous data | plausible model, mixture/outlier questions, method choice |
| Control Chart / SPC | process stability or change detection matters | rational time order/subgroups | common vs special-cause signals |
| Process Capability | a stable process must be compared with specifications | valid MSA, stable data, specs, correct distribution | capability/performance indices and tail risk |

Use stability before capability. Do not delete “outliers” until their process meaning is understood.

## Analyze

| Tool | Use when | Required input | Decision output |
|---|---|---|---|
| Pareto | limited effort needs priority among comparable categories | mutually exclusive counts/cost/rates | vital categories and drill-down plan |
| Fishbone | the team needs a broad hypothesis set | precise effect and cross-functional process knowledge | structured, testable cause hypotheses |
| Is / Is Not | contrasts can narrow a search | verified where/when/what/extent facts | discriminating differences and tests |
| 5 Why | a supported causal path needs deeper system causes | one evidence-backed path | occurrence, escape, and systemic causes |
| Chi-square / exact test | association between categorical variables matters | contingency counts and adequate design | effect/association with uncertainty |
| Hypothesis test / ANOVA | group or condition differences must be quantified | independent/paired data and assumptions | effect, interval, p-value, practical decision |
| Regression | a quantitative relationship or prediction is needed | paired data, plausible model, confounders | effect model, interval, diagnostics, prediction range |
| FTA | a severe top event has multiple AND/OR paths | system architecture and failure logic | cut sets, single-point vulnerabilities, safeguards |
| FMEA | future or existing functions/processes need preventive risk action | structure, function, failure chain, controls | severity-aware/AP actions and residual risk |
| Eight Wastes | flow hides non-value work | direct observation and customer value | waste inventory and improvement targets |

Pareto locates concentration; fishbone expands hypotheses; tests quantify evidence; intervention and mechanism support cause.

## Improve and DFSS optimization

| Tool | Use when | Required input | Decision output |
|---|---|---|---|
| TRIZ | a verified technical/physical contradiction blocks progress | improving/worsening parameters or separation need | concept directions, not final proof |
| Transfer Function `Y=f(X)` | inputs must be linked quantitatively to outputs | physics, simulation, regression or DOE evidence | sensitivity, prediction, tolerance relationship |
| Full/Factorial DOE | effects and interactions must be estimated | controllable factors, response, range, MSA | causal effects, interactions, model |
| Fractional/PB Screening | many factors require economical screening | sparsity assumption and alias plan | shortlist of important factors |
| Taguchi Robust Design | performance must resist explicit noise factors | control/noise factors and loss/response definition | robust parameter combination and confirmation plan |
| RSM | significant continuous factors are near an optimum with curvature | screened factors and local region | quadratic surface and operating window |
| Pugh Matrix | concepts need relative learning against a datum | alternatives and positive criteria | strengths, weaknesses, hybrids, next concepts |
| Weighted Solution Matrix | mature options need a traceable decision | must-have gates, weights, anchored scores, evidence | score, sensitivity, uncertainty, decision record |
| System Design / DFX | functions, interfaces, manufacturability, testability, reliability, cost, or service need design-in control | requirements, architecture, process capability | architecture, ICD, design rules, verification needs |
| Design Scorecard | CTQ capability and risk must be tracked before release | model/simulation/test evidence and specs | CTQ readiness, gap, evidence maturity |
| Poka-Yoke | human or sequence errors should be prevented at source | error mechanism and process step | prevention/interlock/detection concept |

Use independent confirmation. Optimization inside the fitted data is not confirmation.

## Control and organizational learning

| Tool | Use when | Required input | Decision output |
|---|---|---|---|
| SPC | stable operation requires early warning | rational sampling and stable baseline | signals and response triggers |
| Control Plan | critical characteristics need operational ownership | PFMEA, specs, process flow, key X/Y | method, frequency, owner, limit, reaction |
| SOP / Standard Work | repeatable execution must be taught and audited | proven method, images, parameter windows | controlled work instruction |
| Poka-Yoke | recurrence depends on human attention | known error opportunity | prevention or automatic stop |
| 5S | abnormality and wasted motion are hidden by workplace disorder | direct observation | visual location, cleaning-as-inspection, sustain rules |
| Visual Management / Andon | status or abnormality must be understood at a glance | live operational state and escalation | visible normal/abnormal condition and response |
| SMED | changeover limits flexibility or capacity | timed setup steps/video | internal/external separation and reduced downtime |
| Kaizen | many local frictions need rapid ownership | frontline observations | small tested changes and recognition |
| PDCA | a short iterative control/learning loop is sufficient | problem, countermeasure, check method | next standard or next cycle |
| Process Audit | documented controls may differ from practice | process, control plan, evidence | conformity, gaps, CAPA verification |
| Handoff and Benefit Tracking | gains may decay after project closure | owner, baseline, benefit method, controls | signed ownership and sustained benefit |
| Knowledge Base / Lessons Learned | insight should prevent repeat work | validated result and context | reusable rule, case, baseline FMEA, golden setting |

## Fast selection rules

- Subjective customer language → VOC/Kano/CTQ; cross-functional translation → QFD.
- “Our data disagree” → operational definition and MSA before arguing about the process.
- “The average looks fine” → time order/SPC and distribution/stratification.
- “There are many causes” → Pareto/Is–Is Not to focus, fishbone/FTA/FMEA to structure, tests/DOE to verify.
- “We tried changing one factor at a time” → DOE if interaction and causality matter.
- “Two requirements fight each other” → QFD roof to expose, TRIZ to generate, DOE/analysis to verify.
- “The fix worked once” → independent confirmation and pilot before control.
- “People must be more careful” → system cause, standard work, Poka-Yoke, and control-plan reaction.

