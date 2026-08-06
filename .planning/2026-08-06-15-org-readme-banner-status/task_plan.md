---
docId: GOV-PLAN-15
title: "[CODE] fix(profile): banner, mission, status; delete dead onboarding path"
version: 1.0.0
authors:
  - Claude
creation_date: '2026-08-06'
last_updated_date: '2026-08-06'
language: en
summary: Planning context for issue #15 — org profile README advertises the dead pre-ADR-088 onboarding path and the wrong workspace taxonomy
status: in_progress
issue-id: GenCr-ft/.github#15
metadata:
  lifecycle-stage: draft
  scope: project-aethel
  domain: engineering
  doc-type: specification
  security-classification: l2_confidential
  keywords:
    - planning
    - org-readme-banner-status
---

# [CODE] fix(profile): banner, mission, status; delete dead onboarding path

## Problem

`profile/README.md` is the first thing anyone sees at github.com/GenCr-ft. It
currently publishes a broken onboarding path, a workspace taxonomy the tooling
rejects, and no statement of mission or status.

1. **The "Fast Path" is a supply-chain regression.** It instructs newcomers to
   `curl` a tarball of a **moving branch** and run `bash gft-onboarding.sh
   --quickstart`. That is the pre-ENG-ADR-088 orchestrator, which the supported
   entry point no longer invokes at all, and tarballing a branch deliberately
   bypasses the pinned-tag trust anchor that ENG-ADR-087/088 established as the
   sole integrity guarantee between the public shim and the tooling. It is
   **deleted**, not updated.
2. **Wrong workspace taxonomy.** The README claims "five bounded workspaces" and
   names `evai-platform`, `agent-factory`, `workspace-ops`, `studio-gencraft`.
   The tooling enforces exactly four canonical ids — `aethel`, `gft-platform`,
   `onboarding`, `agent-ecosystem` — and `is_canonical_workspace()` hard-rejects
   anything else, so a newcomer following the README picks an id the tool
   refuses. These are two genuinely different taxonomies; `cli.py` already notes
   `WORKSPACE_REPOS` is "the marker-aligned authority; deliberately NOT
   `BOUNDED_WORKSPACES`, which has a different taxonomy".
3. **No banner link.** The link to gencr-ft.github.io exists but is buried in
   prose.
4. **No mission or status.**

## Approach

Add a self-hosted SVG banner (studio palette, no external image dependency)
linked to the public homepage, plus a prominent "Start here" callout, a mission
statement, and a status table.

Status content is kept deliberately **durable rather than sprint-level**:
`gcs-project-management/workspaces/aethel/STATUS.md` was last updated
2026-06-21 and is ~7 weeks stale, so propagating it onto the org front page
would publish stale claims. The table describes what exists and what is live,
and points at the project boards for day-to-day detail.

Relative links resolve from `profile/` (i.e. `../CONTRIBUTING.md`), since the
community-health files live in the repository root.

## Relations

Parent: #15 · keystone gcs-project-management#535 · ADR ENG-ADR-087/088 ·
sibling gencr-ft.github.io#49.
