# Obsidian Capture

Use only after the user explicitly approves saving the completed analysis.

## Vault

Primary vault: `G:\obsidian\六西格玛思维`

Search existing Markdown notes before creating a new one. Prefer updating the relevant problem, decision, case, or tool note over making a duplicate.

## Capture destinations

- Active analyses and decisions: `07 问题分析`
- Reusable completed cases: `06 案例`
- New professional calibration: `05 校准与边界`
- Tool improvements: update the matching note in `04 工具卡`
- Unclassified approved material: `00 Inbox`

## Required preview

Before writing, show:

- proposed title and target path;
- whether the action creates or updates;
- problem statement, route, phase, facts, hypotheses, evidence gaps, tool plan and next gate;
- any sensitive project identifiers that will be retained.

Ask exactly one confirmation question. Do not write on ambiguous assent to the analysis itself; the confirmation must clearly authorize saving.

## Frontmatter

Use Dataview-friendly YAML where applicable:

```yaml
---
type: six_sigma_analysis
status: active
framework: DMAIC
phase: Define
project: ""
created: YYYY-MM-DD
updated: YYYY-MM-DD
tags:
  - 六西格玛
  - 问题分析
---
```

Use `status: active`, `blocked`, `validated`, or `closed` according to evidence. Do not mark a hypothesis validated without supporting evidence.

## Body structure

1. Decision and current gate
2. Neutral problem statement
3. Customer/VOC and operational Y
4. Scope, baseline, target and guardrails
5. Facts, inferences, hypotheses and decisions
6. Evidence gaps and measurement plan
7. Tools now/later/not yet
8. Actions, owners, due evidence and next gate
9. Risks and limitations
10. Sources and related wikilinks

Use `[[wikilinks]]`. Keep source-derived claims separate from `专业校准`. Link to the matching framework, phase, tool cards, and optical note when applicable.

