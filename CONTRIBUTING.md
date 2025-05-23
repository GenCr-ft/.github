# Contributing to GenCr@ft Product Requirements

Thank you for contributing to the GenCr@ft product requirements! This repository serves as the single source of truth for our product specifications, managed as code. By treating requirements as code, we aim for clarity, version control, collaboration, and traceability.

## How to Contribute

We follow a process similar to code contributions using GitHub Flow. All changes and additions to requirements should be proposed via Pull Requests (PRs).

1.  **Find/Create an Issue:** Before starting, check if there's an existing issue in **GitHub Issues for this repository** related to the requirement you want to add or change. If not, please create one to discuss the need and track the work. Reference the Issue ID in your branch name and commits.
2.  **Create a Branch:**
    * Ensure your local `develop` branch is up-to-date (`git checkout develop && git pull origin develop`).
    * Create a new branch from `develop`. Please follow the naming convention: `feature/ISSUE-ID-short-description` (or `fix/ISSUE-ID-correction` if correcting an existing requirement). Replace `ISSUE-ID` with the relevant ID from GitHub Issues.
    * Example: `git checkout -b feature/145-add-voxel-painting-tool`
3.  **Write/Edit Requirements:**
    * Add or modify requirement files (primarily `.md`) within the appropriate directory structure (see [Repository Structure](#repository-structure) below).
    * Follow the established format (Markdown). Use clear and unambiguous language.
    * **Features:** Define specific Features in dedicated `FEATURE_XXX.md` files within `03_Functional_Breakdown/Features/`. Use the `FEATURE_Template.md`. Each Feature file should detail the rationale, functional specification, and acceptance criteria.
    * **User Stories:** Define individual User Stories in separate `US-XXX.md` files within `03_Functional_Breakdown/User_Stories/`. Use the `USER_STORY_Template.md`. Each User Story should follow the "As a..., I want..., So that..." format and include specific Acceptance Criteria.
    * **Linking:**
        * Feature files (`FEATURE_XXX.md`) **must link to** their associated User Story files (`US-XXX.md`) using relative paths under a dedicated section (e.g., "Associated User Stories").
        * User Story files (`US-XXX.md`) **must link back to** their parent Feature file (`FEATURE_XXX.md`) using a relative path in the header section.
    * Reference related Epics using relative links where possible.
    * Link to relevant mockups or design documents (e.g., Figma links, files in `07_Design_UX_UI/Wireframes_Mockups/`) if available.
4.  **Commit Changes:**
    * Commit your changes using the **[Conventional Commits](https://www.conventionalcommits.org/)** format. This helps in generating automated changelogs and understanding the history.
    * Include the Issue ID (e.g., `Fixes #145` or `Relates #145`) in the commit message body or footer.
    * Example: `git commit -m "feat(construction): add initial spec for voxel painting tool" -m "Adds user stories and basic spec outline. Relates #145."`
5.  **Create a Pull Request:**
    * Push your branch to the GitHub repository (e.g., `git push origin feature/145-add-voxel-painting-tool`).
    * Create a Pull Request (PR) on GitHub, targeting the `develop` branch.
    * Fill in the PR description **using the provided Pull Request template**. Clearly explain the purpose of the change and link the relevant issue (e.g., `Closes #145`). *(Note: Ensure a `.github/pull_request_template.md` file is created in the repository to facilitate this.)*
6.  **Review Process:**
    * Request reviews from relevant stakeholders (e.g., Product Owner, Lead Designer, relevant Tech Lead) using GitHub's review request feature.
    * Engage in discussion within the PR comments to refine the requirement based on feedback.
    * Update your branch by pushing new commits as needed based on review comments.
7.  **Merge:** Once the PR is approved by the required reviewers, it will be merged into the `develop` branch by the **Product Owner or a designated repository Maintainer**.

## Repository Structure

Please place your requirement files in the appropriate location within the established structure. Refer to the [00_README_Index.md](00_README_Index.md) for a high-level overview of each section's purpose.

* **`/01_Product_Vision_Strategy/`**: Core vision, market analysis, business model.
* **`/02_Target_Audience/`**: Personas and target hardware configurations.
* **`/03_Functional_Breakdown/`**: Hierarchical breakdown of requirements.
    * `Epics/`: High-level initiatives (e.g., `EPIC_PLAYER_CORE.md`).
    * `Features/`: Detailed features (e.g., `FEATURE_001_Voxel_Placement.md`). User stories & criteria often go within these files.
* **`/04_Roadmap_Releases/`**: Scope definition for specific releases (e.g., `MVP/MVP_Scope_Definition.md`).
* **`/05_Architecture_Technical/`**: Non-functional requirements (e.g., `NFR_Summary_MVP.md`), architectural drivers, tech stack.
* **`/06_Game_Design_Details/`**: Specific game mechanics, balancing, content details (e.g., `Core_Mechanics_Balancing.md`, `Content_Details/`).
* **`/07_Design_UX_UI/`**: Design system, user flows, mockups/links (e.g., `Design_System_Guidelines.md`, `Wireframes_Mockups/`).
* **`/08_Project_Management/`**: Decision logs, action trackers (e.g., `Decision_Log.md`).
* **`/09_Project_Resources/`**: Glossary (`Glossary_V1.md`) and other shared resources.

## Formatting and Templates

* Use **Markdown** for all descriptive files.
* For **Acceptance Criteria** within feature files, use clear Markdown lists (e.g., bullet points with `[ ]` or `[x]` for status if needed) or, if the team adopts BDD practices formally, discuss the potential use of Gherkin format embedded in Markdown code blocks.
* *(Optional: Add links to specific templates here if created, e.g., for a standard Feature file structure within the Markdown)*

## Definition of Done for Requirements

A requirement or specification is generally considered "done" or ready for review/merge when it is:

* **Clear:** Written in unambiguous language understandable by all relevant roles.
* **Concise:** Contains necessary information without unnecessary jargon or verbosity.
* **Consistent:** Aligns with existing requirements, the product vision, and project goals. Does not contradict other documentation.
* **Complete (for its scope):** Provides enough detail for design, development, and testing activities related to this requirement to proceed.
* **Testable:** Includes clear, verifiable acceptance criteria. What must be true for this requirement to be considered implemented correctly?
* **Reviewed:** Has been reviewed and approved by the necessary stakeholders via the PR process.

## Communication

* For general questions or discussions about requirements *before* creating an Issue or PR, please use the `#product-requirements` Slack channel (or the designated primary communication channel for the product team).
* For discussions specific to a proposed change, please use the comments section within the relevant GitHub Issue or Pull Request.

Thank you for helping keep our product requirements clear, consistent, and up-to-date!
