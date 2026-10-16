# Data Guidance

## Approved Core Release

Use the **July 2026 NHS Workforce Statistics** release.

Official release page:
https://digital.nhs.uk/data-and-information/publications/statistical/nhs-workforce-statistics/july-2026

Core files:
1. **Trusts and core organisations — CSV data files** (~30 MB ZIP)
2. **Turnover — CSV data files** (~2 MB ZIP)

Optional supporting files:
3. **Turnover benchmarking — CSV data files** (~270 KB ZIP)
4. **Data Quality Annex** (~173 KB XLSX)

## What to Put in `data/raw/`

Prefer to keep the original downloaded files unchanged:

```text
data/raw/
├── nhs-workforce-july-2026-core.zip
├── nhs-workforce-july-2026-turnover.zip
├── nhs-workforce-july-2026-turnover-benchmarking.zip   # optional
└── nhs-workforce-july-2026-data-quality-annex.xlsx     # optional
```

Do not edit the raw ZIP files. Extract working CSVs through reproducible code or into a working/processed area.

## Recommended Analytical Scope

Do **not** try to analyse every workforce dimension at once.

Agree and document:
- selected organisation(s) or organisation group;
- selected staff groups;
- the measures needed for FTE, headcount and turnover.

## Time Guidance

The July 2026 release is the frozen reference point.

For trend analysis:
- minimum recommended history: **12 months**;
- preferred: **24 months or more** where definitions remain comparable.

Only add historical releases needed for the agreed business question.

## Join Rule

Core workforce and turnover extracts are not automatically compatible at every dimension.

Before joining:
- document the grain of each source;
- confirm compatible organisation/staff-group fields;
- reject unsupported joins.

## Recommended Model

Build separate:
- organisation reference table;
- staff-group reference table;
- workforce fact table;
- turnover fact table;
- agreed analytical aggregate(s).

## Optional Extension

After the core solution works, teams may automate future NHS workforce releases. The July 2026 files remain the frozen assessment baseline.
