# GenCr@ft Studio — GitHub Organization Defaults

Centralized repository for organization-wide community health files and shared configurations for the GenCr@ft Studio GitHub organization.

## Overview

This repository stores the default files that GitHub applies to all public repositories within the `GenCr-ft` organization if they do not provide their own versions. This ensures a consistent community experience and baseline governance across all projects.

## Contents

- **`CODE_OF_CONDUCT.md`**: The standards of behavior for our community.
- **`CONTRIBUTING.md`**: Guidelines for contributing to GenCr@ft projects.
- **`SECURITY.md`**: Instructions for reporting security vulnerabilities.
- **`LICENSE`**: The default open-source license for our projects.
- **`ISSUE_TEMPLATE/`**: Standard templates for bug reports and feature requests.
- **`issue_template_config.yml`**: Configuration for the issue template chooser.
- **`.pre-commit-config.yaml`**: Default pre-commit hook configurations.

## Usage

These files are automatically inherited by other repositories in the organization. To override a default for a specific project, simply add a file with the same name to that project's `.github/` directory or root.

---

*For detailed technical workflows and agent-specific instructions, see [AGENTS.md](./AGENTS.md).*
