---
docId: ORG-PLAN-WI018
title: 'WI-18 — remove the relocated briefing file from the public org profile'
version: 1.0.0
authors: [cerberus]
creation_date: '2026-09-03'
last_updated_date: '2026-09-03'
language: en
issue-id: GenCr-ft/.github#18
status: in_progress
summary: >-
  Plan for the removal half of a two-PR relocation: delete profile/executive_briefing.md from this
  public repository's default branch after the private copy has been landed and verified.
metadata:
  lifecycle-stage: draft
  scope: studio
  domain: engineering
  doc-type: plan
  security-classification: l1_internal
  keywords: [relocation, org-profile, removal, disclosure]
---

# WI-18 — remove the relocated briefing file from the public org profile

Work item: https://github.com/GenCr-ft/.github/issues/18
Design: https://github.com/GenCr-ft/.github/issues/17

This artifact is **hand-authored**. `gft wi plan` rejects this repository's name —
`invalid repo '.github': must match [a-zA-Z0-9-]+` — so no generated planning document is obtainable
for either org-config repo. It is written to the generator's shape rather than waived with
`--skip-plan-check`, because waiving a traceability check in order to satisfy a traceability rule
would be circular. Recorded on
[gcs-plt-tools#1020](https://github.com/GenCr-ft/gcs-plt-tools/issues/1020).

---BEGIN PLAN DATA---

## Objective

Remove `profile/executive_briefing.md` from this repository's default branch. The document has been
relocated to a private studio repository.

The deciding issue is private (`GenCr-ft/gcs-security-core#62`, AC-2). Its contents are deliberately
not restated here — **this repository is public**. This plan describes only *what* moved.

## Why the removal is safe to perform now

The addition half is merged and verified, so deleting the public copy can no longer lose the
document:

| Location | Ref | Digest | Size |
|---|---|---|---|
| Public original | `GenCr-ft/.github@e22b033` | `c5d88b24405005c2c377…` | 9994 B |
| Private copy | `GenCr-ft/.github-private@a5edcdb` | `c5d88b24405005c2c377…` | 9994 B |

Both digests were taken from fresh clones of `origin/main`, not inferred from a merge API response.

## Steps

1. Branch `fix/issue-18-remove-relocated-briefing` from `origin/main`, ancestry proved with
   `git merge-base --is-ancestor`. **Done** — rooted on `e22b033`, which is `origin/main` exactly.
2. REFINE gate on #18. **Done** — full tier, one non-blocking `HTTP 401` warning on the GDD concept
   scan (gcs-plt-gemop#550).
3. Delete the file. Nothing else in the diff except this planning artifact.
4. Open the PR; attribute its red CI at **step level** against a `main` run; do not claim green.
5. Merge, verify absence on a fresh clone of `origin/main`, then run the credential-free AC-2 probes.
6. Record on the deciding issue what the 404 proves **and what it does not**.

## The limit of this remediation — stated up front, not discovered later

Removing a file from `main` does not remove it from git history. After this merges the raw URL for
`main` will 404, but the blob may remain reachable in this public repository's history. That is
verified empirically and unauthenticated in step 6 and reported as observed.

**History rewriting is out of scope**: destructive on a public repo, breaks every clone and fork,
and requires org-level coordination. It is the repository owner's decision. If retrieval from history
still succeeds it is raised as an open question, not acted on.

## Out of scope

- Any rewrite of this repository's history.
- Any edit to the document's text; it moved byte-identically.
- `profile/README.md` and `profile/banner.svg`, both retained.
- Fixing the fleet-wide Gitleaks installation failure
  ([gcd-shared-actions#193](https://github.com/GenCr-ft/gcd-shared-actions/issues/193)).

---END PLAN DATA---
