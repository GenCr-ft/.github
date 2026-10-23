---
docId: GOV-PLAN-025
title: '[CODE] WI-25.1 — remove the SSoT linter callsite and record the exemption'
issue-id: GenCr-ft/.github#25
status: in_progress
version: 1.0.0
authors: [loigallain]
creation_date: '2026-10-23'
last_updated_date: '2026-10-23'
language: en
summary: This repository must stay public, and a public repository cannot call the private
  gcd-shared-actions reusable workflow, so its SSoT gate can never run. It would also scan 0
  files. The callsite is removed and the exemption is documented in AGENTS.md, as the Studio Lead
  decided on 2026-10-23 (GenCr-ft/gcd-shared-actions#241).
metadata:
  lifecycle-stage: draft
  scope: studio
  domain: devops
  doc-type: backlog
  security-classification: l2_confidential
  keywords: [ssot-linter, exemption, public-repo, reusable-workflow-visibility]
---

# [CODE] WI-25.1 — remove the SSoT callsite

Tier: `wi:lightweight`, set by loigallain. The REFINE-LIGHTWEIGHT:PASS on #25 is the latest such comment.

| Step | AC | Status |
|---|---|---|
| Delete `.github/workflows/ssot-compliance.yml`; confirm no other `reusable-ssot-linter` reference | AC-1 | done |
| Add the `## SSoT Gate Exemption` section to `AGENTS.md`: two reasons, link #241, revisit trigger | AC-2 | done |
| A PR opened after merge shows no `SSoT Compliance Check` run | AC-3 | pending |
