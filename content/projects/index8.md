---
title: "Automating Job Discovery and Application Preparation"
date: 2026-10-01
draft: false
summary: "Built an automated Python workflow to collect and filter job listings, track applications, and prepare tailored application drafts."
weight: 2
---

```text
Career pages
       │
       ▼
Fetch and normalise job listings
       │
       ▼
Filter matching roles
       │
       ▼
Update application tracker ─────► Email alert
       │
       ▼
Generate tailored application drafts
       │
       ▼
Compile and validate one-page PDFs
```

I built an end-to-end Python workflow to reduce the repetitive work involved in finding and preparing job applications. The pipeline collects postings from configured career pages, extracts and normalises listing details, applies source-specific eligibility filters, prevents duplicate entries, and synchronises new matches with a persistent application tracker. Each run also produces a concise report and can deliver it by email.

For roles selected for review, the workflow uses the OpenAI API to analyse the job description and tailor a résumé and cover letter from existing LaTeX templates. Generation is deliberately constrained: only designated text blocks may be revised, structural checks enforce content limits, and each document must compile successfully and remain within one page. GitHub Actions coordinates the workflow, while tracker statuses keep application decisions and final review under human control.

*Python · GitHub Actions · OpenAI API · LaTeX · SMTP*
