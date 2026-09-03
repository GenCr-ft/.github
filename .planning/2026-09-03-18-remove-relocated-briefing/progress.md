---
docId: ORG-PROG-WI018
title: 'WI-18 progress — remove the relocated briefing file from the public org profile'
version: 1.0.0
authors: [cerberus]
creation_date: '2026-09-03'
last_updated_date: '2026-09-03'
language: en
issue-id: GenCr-ft/.github#18
status: in_progress
summary: Phase-by-phase progress log for WI-18, the removal half of the briefing relocation.
metadata:
  lifecycle-stage: draft
  scope: studio
  domain: engineering
  doc-type: plan
  security-classification: l1_internal
  keywords: [relocation, org-profile, removal, progress]
---

# Progress — WI-18

---BEGIN PLAN DATA---

## Phase log

| # | Phase | Status | Evidence |
|---|---|---|---|
| 1 | Addition half landed in the private repo | **complete** | PR https://github.com/GenCr-ft/.github-private/pull/12, squashed as `a5edcdb` |
| 2 | Private copy verified on `origin/main` | **complete** | Fresh clone; 9994 B; sha256 `c5d88b24405005c2c377…`; identical to the public original |
| 3 | `[DESIGN]` child authored | **complete** | https://github.com/GenCr-ft/.github/issues/17 |
| 4 | `[CODE]` WI authored in this repo | **complete** | https://github.com/GenCr-ft/.github/issues/18 |
| 5 | Branch cut, ancestry proved | **complete** | `fix/issue-18-remove-relocated-briefing` on `e22b033` = `origin/main` |
| 6 | REFINE gate | **complete** | https://github.com/GenCr-ft/.github/issues/18#issuecomment-5525295266 |
| 7 | File deleted, committed | in progress | this commit |
| 8 | PR opened, CI attributed at step level | pending | |
| 9 | Merged; absence verified on a fresh `origin/main` clone | pending | |
| 10 | Credential-free AC-2 probes, with control | pending | |
| 11 | History-retrieval check, reported as observed | pending | |
| 12 | Deciding issue updated: AC-2 ticked, limits stated | pending | |

## Why a work item exists in this repository at all

The Lifecycle Gate resolves a branch's `issue-N` against **the repository being edited**. A branch
named for the deciding issue — which lives in a different repo — resolves to a nonexistent issue
here, returns `HTTP 404`, and blocks under a misleading `[AUTH]` banner. The local WI is structurally
required.

## Environmental defects met, all pre-existing and all cited rather than re-filed

| Defect | Effect here |
|---|---|
| [gcs-plt-tools#1020](https://github.com/GenCr-ft/gcs-plt-tools/issues/1020) | `gft branch create` cuts from local `HEAD` with no fetch; ancestry proved explicitly instead |
| `gft wi plan` rejects dotted repo names | This artifact is hand-authored; `--skip-plan-check` not used |
| [gcs-plt-gemop#550](https://github.com/GenCr-ft/gcs-plt-gemop/issues/550) | Raw `gh` reads return `HTTP 401`; REFINE step 2c skipped with a warning |
| [gcd-shared-actions#193](https://github.com/GenCr-ft/gcd-shared-actions/issues/193) | Blocking Gitleaks step fails at *installation*, so the SSoT linter never runs — CI carries no assurance either way |
| [gcd-shared-actions#188](https://github.com/GenCr-ft/gcd-shared-actions/issues/188) | Pre-commit traceability gate imports `yaml`; PyYAML supplied on `PATH` from a venv outside the repo, not with `--no-verify` |

## Rule 6 note

No `CHANGELOG.md` exists in this repository, so the changelog trailer rule is unsatisfiable here —
the condition tracked by
[gcs-project-management#575](https://github.com/GenCr-ft/gcs-project-management/issues/575).

---END PLAN DATA---
