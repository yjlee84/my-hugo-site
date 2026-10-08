---
title: "Modernising the OECD Health Data Validation"
date: 2026-08-01
draft: false
summary: "Modernised an R-based pipeline to automate the validation, calculation, and processing of cross-country health care quality data."
weight: 1
---

```text
Country delegates
       │
       ▼
Prepare CSV data
       │
       ▼
Automated pipeline
       │
       ├── Standardise data
       │          │
       │          ▼
       ├── Automated validation ─────► Issues found
       │          │                         │
       │          │                         ▼
       │          │                 Validation report
       │          │                         │
       │          │                  Locate and correct
       │          │                         │
       │          ├──────────── Revalidate ◄┘
       │          │
       │          ▼
       ├── Calculate indicators
       │
       ▼
Review dashboard
       │
       ▼
Validated CSV submissions
       │
       ▼
Database-ready output
       │
       ▼
OECD Data Explorer
```

As a Consultant at the OECD, I helped strengthen health information infrastructure by modernising and integrating an automated R-based data-processing pipeline for the [Healthcare Quality and Outcomes](https://www.oecd.org/en/topics/health-care-quality-and-outcomes.html) data collection. The tool helps country delegates improve data quality before submission by standardising multi-year data and checking for structural errors, invalid entries, duplicates, missing observations, logical inconsistencies, zero denominators, and unusual year-on-year changes. When issues are detected, it generates and opens CSV validation reports identifying affected observations, making errors easier to locate and correct. The pipeline also calculates indicators and confidence intervals, produces review dashboards, and prepares validated results for database upload, reducing reliance on manual spreadsheet processing and strengthening the consistency and reproducibility of cross-country health data.

* [Data](https://data-explorer.oecd.org/vis?df%5Bag%5D=OECD.ELS.HD&df%5Bds%5D=dsDisseminateFinalDMZ&df%5Bid%5D=DSD_HCQO%40DF_HCQO&df%5Bvs%5D=2.1)
* [Slides](/pdfs/HCQO_Modernisation_Presentation.pdf)
