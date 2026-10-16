# Business Context

## Business Problem

The workforce directorate has access to published headcount, FTE and turnover statistics, but these are often reviewed in separate reports and at different organisational or staff-group levels. Senior leaders can see that staffing has changed, but they cannot consistently tell whether the underlying issue is recruitment, retention, workforce mix, part-time working patterns, organisational restructuring or normal short-term fluctuation.

This creates a planning problem. A large headcount can mask weak FTE capacity; high turnover may affect only certain staff groups; and organisation-level trends can be distorted by structural changes. Without one governed analytical view, workforce interventions risk being too broad or directed at the wrong problem.

The core business problem is therefore to move from descriptive workforce reporting to a repeatable evidence base that helps leadership identify where capacity pressure is persistent and what type of workforce response should be investigated.

## Required Delivery Response

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

## How the Client Will Use the Output

The finished product should be usable in a workforce planning meeting. A Workforce Director should be able to identify, for example, a staff group where headcount appears stable but FTE is falling, or an organisation where persistent turnover coincides with weak workforce growth.

The product should then help leadership decide whether the next step is deeper recruitment analysis, retention investigation, workforce redesign, or further data collection. It must not be presented as a safe-staffing or care-quality assessment.

## Client
**Confidential NHS Workforce & People Directorate**

## Current Problem
Leadership can see headline staffing totals, but workforce decisions are made across separate reports for headcount, FTE, staff group and turnover. The directorate cannot consistently identify where capacity is genuinely deteriorating, where turnover is persistent, or whether apparent shortages reflect workforce mix rather than absolute staffing levels.

## Decision Owner
**Director of Workforce**

## Senior Stakeholders
Deputy Director of Workforce Planning, Recruitment Lead, Retention Lead, Operational Planning Lead, Finance Business Partner, Data Governance Lead, Workforce Intelligence Lead

## Decision to Support
**Which workforce groups and organisations require the earliest intervention to protect service capacity, and is the evidence more consistent with recruitment pressure, retention pressure, workforce-mix change or a need for further investigation?**

## Role Responsibilities
| Role | Required contribution |
|---|---|
| Business Analyst | Produce workforce decision map, stakeholder requirements, user stories, scope and acceptance criteria. |
| Data Governance Analyst | Define workforce glossary, critical fields, organisation/staff-group reference rules, lineage and DQ controls. |
| Data Engineer | Build reproducible preparation of workforce and turnover extracts and a consistent analytical model. |
| Workforce/Data Analyst | Own FTE/headcount/turnover trend and peer-comparison analysis. |
| BI Developer | Build governed workforce sustainability reporting and drill-down. |
| Data Scientist / Forecaster | Develop simple scenario/forecast component where justified and benchmark it against a naive baseline. |
| Model Governance / Assurance Analyst | Challenge forecasting assumptions, uncertainty, subgroup effects and use boundaries. |

## Expected Organisational Outcome

The intended result is a governed, repeatable decision process. The BI product is one delivery component; it is not the project outcome by itself.

## Evidence Chain

**Requirement → governed field/definition → transformation → quality control → metric/analysis → decision insight → recommendation → UAT/acceptance**

Every major recommendation should be traceable through this chain.
