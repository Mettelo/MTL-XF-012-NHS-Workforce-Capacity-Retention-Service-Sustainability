# Project Brief

## 1. Business Problem

The workforce directorate has access to published headcount, FTE and turnover statistics, but these are often reviewed in separate reports and at different organisational or staff-group levels. Senior leaders can see that staffing has changed, but they cannot consistently tell whether the underlying issue is recruitment, retention, workforce mix, part-time working patterns, organisational restructuring or normal short-term fluctuation.

This creates a planning problem. A large headcount can mask weak FTE capacity; high turnover may affect only certain staff groups; and organisation-level trends can be distorted by structural changes. Without one governed analytical view, workforce interventions risk being too broad or directed at the wrong problem.

The core business problem is therefore to move from descriptive workforce reporting to a repeatable evidence base that helps leadership identify where capacity pressure is persistent and what type of workforce response should be investigated.

## What the Team Needs to Do

The team is expected to build a workforce-sustainability intelligence product that combines core workforce and turnover data at compatible grains.

The work should include:
- defining the workforce decision process and users;
- creating a workforce glossary that clearly separates headcount, FTE, turnover and staff-group measures;
- documenting organisation/staff-group codes and any continuity issues;
- building reproducible preparation of the core workforce and turnover files;
- validating joins and avoiding unsupported combinations of incompatible grains;
- analysing FTE and headcount trends separately;
- identifying persistent turnover rather than single-period movements;
- comparing staff-group and organisation trends against relevant peers or baselines;
- creating transparent workforce-pressure indicators;
- optionally developing simple scenarios/forecasts only where enough history exists;
- building management BI for organisation/staff-group drill-down;
- completing reconciliation, UAT and operational handover.

## Practical Use Case

The finished product should be usable in a workforce planning meeting. A Workforce Director should be able to identify, for example, a staff group where headcount appears stable but FTE is falling, or an organisation where persistent turnover coincides with weak workforce growth.

The product should then help leadership decide whether the next step is deeper recruitment analysis, retention investigation, workforce redesign, or further data collection. It must not be presented as a safe-staffing or care-quality assessment.

## 2. Business Decision

The team has been commissioned to provide evidence for this decision:

> **Which workforce groups and organisations require the earliest intervention to protect service capacity, and is the evidence more consistent with recruitment pressure, retention pressure, workforce-mix change or a need for further investigation?**

The project succeeds only if the final solution helps stakeholders make or structure this decision; producing charts without a decision framework is insufficient.

## 3. Agreed Objectives

1. Create a governed workforce model combining core workforce and turnover measures at an agreed organisational/staff-group grain.
2. Separate headcount, FTE and turnover concepts so leadership does not use them interchangeably.
3. Identify persistent workforce pressure by organisation and staff group using transparent comparison rules.
4. Develop scenario-based workforce sustainability indicators without presenting them as clinical safe-staffing measures.
5. Provide workforce leaders with a repeatable decision-support product and monitoring framework.

## 4. Key Business Questions

1. Where are FTE levels changing materially over time or relative to comparable organisations/staff groups?
2. Which staff groups show persistent turnover pressure rather than a one-month movement?
3. Where do headcount and FTE tell different stories about capacity?
4. Which organisations combine weak workforce growth with elevated turnover?
5. Which data/publication changes limit longitudinal comparison?
6. What indicators should trigger workforce investigation rather than automatic intervention?

## 5. Cross-Functional Delivery Model

| Role | Minimum expected output |
|---|---|
| Business Analyst | Produce workforce decision map, stakeholder requirements, user stories, scope and acceptance criteria. |
| Data Governance Analyst | Define workforce glossary, critical fields, organisation/staff-group reference rules, lineage and DQ controls. |
| Data Engineer | Build reproducible preparation of workforce and turnover extracts and a consistent analytical model. |
| Workforce/Data Analyst | Own FTE/headcount/turnover trend and peer-comparison analysis. |
| BI Developer | Build governed workforce sustainability reporting and drill-down. |
| Data Scientist / Forecaster | Develop simple scenario/forecast component where justified and benchmark it against a naive baseline. |
| Model Governance / Assurance Analyst | Challenge forecasting assumptions, uncertainty, subgroup effects and use boundaries. |

Responsibilities may be combined in a smaller team, but ownership and evidence must remain explicit.

## 6. Minimum Delivery Standard

The team must demonstrate:

- traceable requirements from stakeholder need to delivered feature/KPI;
- documented governance for critical fields and measures;
- preserved raw source data and reproducible transformations;
- explicit data-quality tests and reconciliation;
- analytical outputs that answer the commissioned questions;
- transparent decision/prioritisation logic;
- a stakeholder-facing product built from approved metrics;
- assurance/UAT evidence;
- technical and operational handover;
- GitHub evidence of genuine multidisciplinary collaboration.

## 7. Constraints and Interpretation Rules

- Published workforce statistics do not measure safe staffing, service quality or individual performance.
- Turnover does not by itself identify why people leave or whether departures are avoidable.
- Headcount and FTE must not be combined or compared without clear definition.
- Organisation restructures and code changes can distort longitudinal comparisons.
- Any forecast/scenario is planning support and must show uncertainty and assumptions.

## 8. Agreed Success Criteria

The detailed acceptance tests are in `ACCEPTANCE_CRITERIA.md`. At minimum:

- Core workforce and turnover datasets are joined only at a documented compatible grain; unsupported joins are explicitly rejected.
- Headcount and FTE are separately defined and no KPI silently mixes the two.
- At least three longitudinal validation checks reconcile derived values to published/source totals where feasible.
- Organisation/staff-group code changes or discontinuities affecting trend analysis are documented.
- If forecasting is used, a naive baseline and time-aware validation are included and uncertainty is shown.
- No output is described as a safe-staffing judgement or direct measure of care quality.

## 9. Out of Scope

Unless explicitly justified as an extension, the core engagement does not require:

- paid production infrastructure;
- confidential client data;
- automated operational decisions;
- unsupported causal inference;
- a production-grade public application.

## 10. Final Review

The Mettelo review panel may challenge source handling, definitions, reconciliation, analytical methods, thresholds, usability, governance, recommendations and whether the evidence actually supports the commissioned decision.

### Reproducibility definition

A reviewer should be able to clone the team repository, obtain the documented approved source data, execute the documented workflow and reproduce the curated analytical outputs and validation evidence without undocumented manual changes.
