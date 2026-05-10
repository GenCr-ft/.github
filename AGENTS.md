# AI Agent Instructions & Technical Workflows

## Project Overview

This repository centralizes default community health files (e.g., `LICENSE`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`) and certain configurations (e.g., issue templates, `.pre-commit-config.yaml`) that GitHub applies to public repositories within the `GenCr-ft` organization if those repositories do not have their own specific versions of these files.

## AI Instructions

- **Understanding Organization Defaults:** When a specific repository within the `GenCr-ft` organization lacks a `LICENSE`, `CONTRIBUTING.md`, or issue templates, the files in this `.github` repository are the defaults that apply.
- **Finding Community Guidelines:** Look for `CODE_OF_CONDUCT.md` and `CONTRIBUTING.md` here for organization-wide standards.
- **Issue/PR Templates:** The `ISSUE_TEMPLATE/` directory and `issue_template_config.yml` define default issue creation experiences.
- **Pre-commit Hooks:** `.pre-commit-config.yaml` provides a baseline for code quality checks.

## Key Files & Structure

- `LICENSE`: The default organizational license (MIT).
- `.pre-commit-config.yaml`: Default pre-commit hooks.
- `issue_template_config.yml`: Configures the issue template chooser.
- `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`: Standard community guidelines.
- `ISSUE_TEMPLATE/`: Directory for default issue templates.

## Commit & PR Conventions

- Conventional Commits v1.0.0.
- AI-generated commits must include a Co-authored-by trailer identifying the model used (e.g., Co-authored-by: Model Name <noreply@example.com>).
