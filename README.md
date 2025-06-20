---
docId: GC-GHUB-README-IDX-001 # GenCr@ft - GitHub Org - README - IndeX
title: GenCr@ft Studio - Organization-wide GitHub Files - README
version: 1.0.0
status: Active
authors:
  - "DevOps Team"
  - "Community Management Team"
knowledgeGuardian(s):
  - "Lead DevOps Engineer"
relatedDocuments:
  - docId: GCS-DEVOPS-GITHUB-STD-IDX-001 # Assumed link to GitHub standards in DevOps
    description: "Gencraft Studio DevOps Standards for GitHub"
  - docId: GCS-H016 # Link to SSoT Documentation Principles
    description: "SSoT Documentation Principles"
audience:
  - "All Contributors"
  - "Community Members"
  - "DevOps Team"
  - "AI Agents (Gems)"
keywords:
  - "github"
  - "community"
  - "contributing"
  - "code of conduct"
  - "issue templates"
  - "pull request templates"
  - "organization defaults"
ssot_path: ".github/README.md"
reviewers:
  - "Head of Engineering"
creation_date: "2024-07-25" # Example date
language: "en"
summary: "This README.md serves as the entry point for the .github special repository. This repository contains default community health files and configuration that apply to public repositories within the GenCr@ft Studio GitHub organization, unless overridden at the individual repository level."
tags:
  - "github"
  - "community-health"
  - "organization-profile"
  - "index"
last_updated_date: "2024-07-25" # Example date
---

# GenCr@ft Studio - Organization-wide GitHub Files

Welcome to the `.github` repository for GenCr@ft Studio. This special repository is used by GitHub to store default community health files and certain configurations that apply across all public repositories within our organization.

Files placed here, such as `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, issue templates, and pull request templates, will be used by repositories in the organization that do not have their own versions of these files.

---

## Index of Contents

This repository contains (or is intended to contain) the following organization-wide files and configurations:

### Files

- **LICENSE**: The default open-source license for GenCr@ft Studio projects.
- **.pre-commit-config.yaml**: Default pre-commit hook configurations for ensuring code quality and consistency across repositories.
- **issue_template_config.yml**: Configuration for the issue template chooser in repositories.
- **CODE_OF_CONDUCT.md** (To be added/verified): Outlines the expected standards of behavior for our community.
- **CONTRIBUTING.md** (To be added/verified): Provides guidelines for contributing to GenCr@ft Studio projects.
- **SECURITY.md** (To be added/verified): Details how to report security vulnerabilities.
- **SUPPORT.md** (To be added/verified): Explains how to get support for our projects.

### Subdirectories

- **ISSUE_TEMPLATE/** (To be added/verified): Contains default templates for creating new GitHub issues.
- **PULL_REQUEST_TEMPLATE/** (To be added/verified): May contain a default template for pull requests.

---

## IA Instructions

**Purpose for AI Agents:**

This `README.md` (docId: `GC-GHUB-README-IDX-001`) is the master index for the `.github` special repository of the GenCr@ft Studio organization.

**Repository Structure and Content Nature:**

- **Overall Goal:** This repository centralizes default community health files (e.g., `LICENSE`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`) and certain configurations (e.g., issue templates, `.pre-commit-config.yaml`) that GitHub applies to public repositories within the `GenCr-ft` organization if those repositories do not have their own specific versions of these files.
- **Key Files/Directories:**
  - `LICENSE`: The default organizational license.
  - `.pre-commit-config.yaml`: Default pre-commit hooks.
  - `issue_template_config.yml`: Configures the issue template chooser.
  - `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`: Standard community guidelines.
  - `ISSUE_TEMPLATE/`: Directory for default issue templates.
- **Document Nature:** Files are typically Markdown (`.md`) for documentation/guidelines, YAML (`.yaml`, `.yml`) for configurations.

**How to Use This Repository (for AI Agents):**

- **Understanding Organization Defaults:** When a specific repository within the `GenCr-ft` organization lacks a `LICENSE`, `CONTRIBUTING.md`, or issue templates, the files in this `.github` repository are the defaults that apply.
- **Finding Community Guidelines:** Look for `CODE_OF_CONDUCT.md` and `CONTRIBUTING.md` here for organization-wide standards.
- **Issue/PR Templates:** The `ISSUE_TEMPLATE/` directory and `issue_template_config.yml` define default issue creation experiences.
- **Pre-commit Hooks:** `.pre-commit-config.yaml` provides a baseline for code quality checks.

This repository is crucial for understanding the baseline community standards and developer experience configurations for the GenCr@ft Studio GitHub organization.
