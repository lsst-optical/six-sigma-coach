# Black Belt Question Tree

Use this tree adaptively. Ask one question at a time, resolve dependencies before moving on, and skip questions already answered by reliable evidence.

## 0. Triage and containment

Ask first when safety, compliance, customer escape, irreversible loss, or ongoing production exposure may exist:

- Is anyone or any customer currently exposed to harm, escape, or accumulating loss?
- What temporary containment is already active, who owns it, and how is its effectiveness checked?

Containment limits damage; it is not root cause or permanent corrective action. Use 8D/CAPA governance when incident discipline is needed.

## 1. Route selection

Resolve these in order:

1. Is the capability already supposed to exist, or is it being designed for the first time?
2. Is the problem chronic/complex, urgent/escaping, flow-dominated, or local/low-risk?
3. What decision must this analysis enable, by when, and for whom?

Recommended mapping:

- Existing chronic gap + unknown cause → DMAIC.
- New capability or architecture → DFSS.
- Active serious incident → 8D/CAPA, with containment first.
- Flow/setup/waste → Lean/VSM/SMED.
- Local known problem → PDCA/A3/Kaizen.

## 2. Define

Ask only what is missing:

1. Who experiences the failure or receives the output?
2. What did they say, observe, reject, or require?
3. What measurable output `Y` represents that need?
4. Under exactly what conditions, unit, sampling point, method, and decision rule is `Y` measured?
5. What counts as one unit, one defect, and one opportunity?
6. What is the baseline, time window, target, deadline, and business consequence?
7. What guardrails must not worsen: safety, reliability, center performance, cycle time, cost, power, weight, or another CTQ?
8. Where does the process begin and end? What is explicitly out of scope?
9. Who owns the process and who can approve resources or a route change?

Recommended deliverable: a neutral problem statement with no embedded cause or solution, a CTQ operational definition, SIPOC-level boundary, and a short charter.

## 3. Measure

1. Where do data originate and can each result be traced to unit, time, batch, equipment, operator, condition, and rework state?
2. Does the sample cover startup, changeover, shifts, batches, equipment, environment, and other plausible strata?
3. What values were excluded, and was the rule set before seeing results?
4. Can the measurement system distinguish differences that matter for the decision?
5. Does MSA include the complete measurement process: fixture, setup, software, interpretation, environment, and operator?
6. Is the process stable over time? Which rational subgroup or chart type matches data collection?
7. What are the current distribution, center, spread, defect rate, and capability under the correct model?

Do not proceed to causal statistics when the measurement system or sampling frame is not fit for purpose. The next tool may be a data plan or MSA, not regression.

## 4. Analyze

1. Where and when is the problem concentrated? Where and when is it absent?
2. Are categories mutually exclusive, comparable, and normalized by opportunity where needed?
3. Which candidate causes follow from the actual process, failure mechanism, and stratified data?
4. For each leading `X`, what observation would support it and what observation would falsify it?
5. Could equipment, batch, shift, operator, time, rework, or selection create confounding?
6. What effect size and uncertainty are decision-relevant, not merely statistically significant?
7. Can changing `X` predict the direction and magnitude of `Y` and be repeated independently?
8. Why did the failure occur, why was it not detected, and why did the system allow it to persist?

Use fishbone and FMEA to organize hypotheses, not certify root causes. Use FTA for top-event logic. Use tests/regression to quantify evidence. Use designed intervention or strong mechanism evidence before causal closure.

## 5. Improve or design

1. Which verified `X` must the solution change?
2. What must-have constraints eliminate a concept before scoring?
3. Which evaluation criteria come from CTQ, risk, cost, delivery, service, and strategy? Are they non-duplicative?
4. What new failure modes or interface risks does each option introduce?
5. Is the need concept generation, factor screening, continuous optimization, robust design, tolerance design, or simple pilot confirmation?
6. What trial can distinguish alternatives while controlling nuisance variables?
7. What independent confirmation data and stop criteria are required?
8. Did the primary `Y` improve without violating guardrails?

Use TRIZ for a proven contradiction, Pugh for relative concept learning, a weighted decision matrix for mature alternatives, DOE for causal factor learning, RSM after screening near an optimum, and Taguchi methods when robustness against explicit noise factors is central.

## 6. Control and transfer

1. Which critical `X`s and `Y`s must remain visible?
2. For each, what method, frequency, sample, limit, owner, record, and reaction plan applies?
3. What exact event triggers stop, isolation, escalation, investigation, and restart?
4. Does the control plan agree with PFMEA, SOP, inspection specifications, maintenance, calibration, and training?
5. Has the operating owner demonstrated the control without the project team?
6. What 30/60/90-day evidence proves the gain persists?
7. How will financial benefit be verified and separated from volume or mix changes?
8. What lesson, design rule, baseline FMEA, or golden parameter should be reused?

The final control is a working management system, not a project team watching a dashboard forever.

