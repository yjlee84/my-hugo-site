---
title: "Automating Job Alerts, Tracking, and Drafting"
date: 2026-10-01
draft: false
summary: "Built an automated Python workflow to collect and filter job listings, track applications, and prepare tailored application drafts."
weight: 2
---

{{< job-alert >}}

I built an end-to-end Python workflow that automates job discovery and application preparation from computer login onward. A local startup process triggers GitHub Actions, which collects and normalises new postings, applies source-specific eligibility filters, prevents duplicates, and updates a single CSV tracker containing each role's full description, status, and application details. The workflow sends a job alert by email, generates a Markdown report, and synchronises the latest files back to the local computer. For roles marked for review, it uses the OpenAI API to tailor résumé and cover-letter drafts from existing LaTeX templates, compiles and validates the one-page PDFs, and stores the resulting application package by job. I then use the prepared drafts to apply and manage the entire process by updating statuses in one tracker.

*Python · GitHub Actions · OpenAI API · LaTeX · SMTP*
