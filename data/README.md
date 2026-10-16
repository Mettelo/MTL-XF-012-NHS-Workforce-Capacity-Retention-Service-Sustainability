# Data Guidance

## Approved Core Files

Use the **July 2026 NHS Workforce Statistics** release.

Official release page:
https://digital.nhs.uk/data-and-information/publications/statistical/nhs-workforce-statistics/july-2026

Core files:
1. **Trusts and core organisations — CSV data files** (~30 MB ZIP)
2. **Turnover — CSV data files** (~2 MB ZIP)

Optional:
3. **Turnover benchmarking — CSV data files** (~270 KB ZIP)
4. **Data Quality Annex** (~173 KB XLSX)

## What Goes in `data/raw/`

Prefer to keep the original downloaded ZIP files unchanged:

```text
data/raw/
├── nhs-workforce-july-2026-core.zip
├── nhs-workforce-july-2026-turnover.zip
├── nhs-workforce-july-2026-turnover-benchmarking.zip   # optional
└── nhs-workforce-july-2026-data-quality-annex.xlsx     # optional
```

Do not edit the raw ZIPs.

Extract working CSVs outside the frozen raw copy or through reproducible code.

## Recommended Analytical Scope

Do **not** attempt to analyse every workforce dimension at once.

Choose and document:
- one manageable organisation group or selected organisations;
- selected staff groups;
- the measures needed for FTE, headcount and turnover.

If historical analysis is required, add only the additional monthly/annual files needed for the agreed trend question.

## Time Guidance

The July 2026 publication is the **frozen reference release**.

For longitudinal analysis:
- use a clearly defined period;
- recommended minimum: 12 months;
- preferred: 24+ months where definitions remain comparable.

Do not silently mix months with incompatible organisation structures or definitions.

## Join Rule

Core workforce and turnover extracts may not be joinable at every possible field combination.

Before joining:
- document grain for each source;
- confirm compatible organisation/staff-group dimensions;
- reject unsupported joins.

## Practical Working Pattern

Use the raw July release for reproducibility, then build:
- organisation reference table;
- staff-group reference table;
- workforce fact table;
- turnover fact table;
- agreed analytical aggregate(s).

## Optional Extension

After the core model works, teams may automate retrieval of future workforce releases to demonstrate maintainability. The July 2026 frozen files remain the baseline for assessment.
