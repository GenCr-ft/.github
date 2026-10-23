---
docId: GOV-PLAN-022
title: '[CODE] WI-22.1 — move the SSoT linter caller to @v1 and drop the explicit version pins'
issue-id: GenCr-ft/.github#22
status: in_progress
version: 1.0.0
authors: [loigallain]
creation_date: '2026-10-23'
last_updated_date: '2026-10-23'
language: en
summary: The SSoT linter caller moves from @v1.5.0 to the moving @v1 alias and drops both version
  inputs, so it inherits the measured canonical pair (v1.6.1, v5.0.1). This is AC-5 of
  GenCr-ft/gcd-shared-actions#303 and supersedes #21.
metadata:
  lifecycle-stage: draft
  scope: studio
  domain: devops
  doc-type: backlog
  security-classification: l2_confidential
  keywords: [ssot-linter, version-pins, v1-alias, cve]
---

# [CODE] WI-22.1 — SSoT caller to @v1

Tier: `wi:lightweight`, set by loigallain. The REFINE-LIGHTWEIGHT:PASS comment is on #22.

| Step | Status |
|---|---|
| Change `uses:` from `@v1.5.0` to `@v1` and drop both version inputs | done |
| Keep posture `continue-on-error: false` and `secrets:` unchanged | done |
| Verify the change structurally: parse the YAML and assert the job block | done |
| Check the CI oracle | **none**: this repo's SSoT workflow has never dispatched (GenCr-ft/gcd-shared-actions#241) |
