---
title: "Automating Job Alerts, Tracking, and Drafting"
date: 2026-10-01
draft: false
summary: "Built an automated Python workflow to collect and filter job listings, track applications, and prepare tailored application drafts."
weight: 3
---

{{< job-alert >}}

I built an end-to-end Python workflow to reduce the repetitive work involved in job discovery and application preparation, automating the process from computer login onward. A local startup process triggers GitHub Actions, which collects postings from configured career pages, normalises their details, applies source-specific eligibility filters, prevents duplicates, and updates a persistent application tracker in a single CSV containing each role's full description, status, and application details. The workflow sends a job alert by email, generates a Markdown report, and synchronises the latest files back to the local computer. For roles marked for review, it uses the OpenAI API to analyse the job description and tailor résumé and cover-letter drafts from existing LaTeX templates. Generation is deliberately constrained to designated text blocks, and the workflow compiles and validates each one-page PDF before storing the application package. I then review the prepared drafts, apply, and manage the process by updating statuses in the tracker, keeping final review under human control.

*Python · GitHub Actions · OpenAI API · LaTeX · SMTP*

* [Code](https://github.com/yjlee84/job-alerts)
