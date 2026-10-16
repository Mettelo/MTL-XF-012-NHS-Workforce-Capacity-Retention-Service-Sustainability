# Project Brief

## Engagement Details

| Field | Detail |
|---|---|
| Project ID | MTL-XF-012 |
| Project Title | NHS Workforce Capacity, Retention & Service Sustainability Intelligence |
| Client | Confidential NHS Workforce & People Directorate |
| Sector | NHS / Workforce / Service Planning |
| Duration | 8 weeks |
| Recommended Team Size | 6–8 |
| Primary Sponsor | Director of Workforce |
| Senior Stakeholders | Deputy Director of Workforce Planning, Recruitment Lead, Retention Lead, Operational Planning Lead, Finance Business Partner, Data Governance Lead, Workforce Intelligence Lead |
| Primary Dataset | NHS HCHS Workforce Statistics — July 2026 core workforce and turnover extracts |

## 1. Client Situation

Leadership can see headline staffing totals, but workforce decisions are made across separate reports for headcount, FTE, staff group and turnover. The directorate cannot consistently identify where capacity is genuinely deteriorating, where turnover is persistent, or whether apparent shortages reflect workforce mix rather than absolute staffing levels.

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
