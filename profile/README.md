# Welcome to the GenCr@ft Project

**Version:** 0.1.0 (Initial Development Underway)
**README Last Updated:** May 16, 2025

## 1. What is GenCraft?

GenCraft is an ambitious multiplayer sandbox video game set in a vast and dynamic, procedurally generated open world. It offers players unprecedented freedom to explore, build, and interact in a rich and varied environment. This document and this meta-repository (`GenCr-ft`) are intended for anyone joining the project, regardless of their role (development, marketing, sales, architecture, product management, project management).

GenCraft combines elements from several popular genres:

* **Sandbox:** Players have the ability to modify the world around them, build complex structures, and create their own gameplay experiences.
* **Multiplayer:** Players can interact with others, collaborate on common projects, exchange resources, and participate in community events.
* **RPG:** The game integrates character progression mechanics, allowing players to develop their skills, acquire new items, and overcome challenges.
* **UGC (User-Generated Content):** The game emphasizes player-generated content, offering powerful tools to create and share creations.

## 2. Project Vision

The vision for GenCraft is to create a game that offers an infinite and stimulating experience, where players are in control of their own adventure. We want to build a community of passionate and creative players who contribute to shaping the game.

## 3. Key Features (Expected)

* **Procedurally Generated World:** A vast and varied universe, filled with unique biomes, rare resources, and hidden secrets.
* **Free-form Construction:** The ability to build anything, from simple houses to sprawling cities, using an intuitive voxel system.
* **RPG Progression:** A rich progression system that allows players to develop their skills and specialize in different playstyles.
* **User-Generated Content:** Powerful tools to create and share items, structures, and even mini-games.
* **Multiplayer:** The ability to play with friends and other players, collaborate on projects, and participate in community events.
* **Ethical Monetization:** A monetization model that supports game development without harming the player experience.

## 4. Target Audience

GenCraft targets a broad audience of players, including:

* Sandbox game fans who enjoy exploring and building.
* Multiplayer gamers seeking social and collaborative experiences.
* RPG enthusiasts who appreciate character progression and challenges.
* Creators who love to design and share their own content.

## 5. Why is GenCraft Unique? (Ambition)

GenCraft aims to distinguish itself from other games through:

* Its modular extensibility, allowing players and developers to add new features to the game.
* Its variable voxel system, offering unprecedented construction freedom.
* Its integration of generative AI, which enhances immersion and creates dynamic experiences.
* Its ethical monetization model, which values player contributions.

## 6. Structure of this Meta-Repository and Opportunities

This meta-repository (`GenCr-ft`) centralizes all sub-projects related to GenCraft. Each folder represents an aspect of development and offers specific opportunities:

* **`gencraft-requirements/`**
    * **Content:** Product vision, target audience, functional breakdown (Epics, Features, User Stories), roadmap, initial technical architecture, design (UX/UI), project management, resources (templates, glossary).
    * **Opportunity (Product/Project Management):** Shape the game's vision and define development priorities. Coordinate team efforts and ensure adherence to deadlines/budgets.
    * **Main entry point:** `gencraft-requirements/00_README_Index.md`

* **`gencraft-architecture/`**
    * **Content:** Formal architectural documentation (Principles, ADRs, C4 diagrams).
    * **Opportunity (Architecture):** Design a scalable and high-performance game architecture.

* **`gencraft-iac/`**
    * **Content:** Infrastructure as Code (Terraform), modules, environment configurations, initialization scripts.
    * **Opportunity (Development/DevOps):** Contribute to the game's cloud infrastructure.

* **`gencraft-gem/`** (and `gencraft-gem-blueprints/`)
    * **Content:** "AI Gems" (G-FT.ai) to assist in development.
    * **Opportunity (Development/AI):** Develop innovative AI tools for the game and studio.

* **`gencraft-studio-handbook/`**
    * **Content:** Studio manual, vision, protocols, Knowledge Base, archiving, tooling.
    * **Opportunity (All Roles):** Understand and contribute to studio processes.

* **`devops-standards/`**
    * **Content:** DevOps Standards (CI/CD, GitHub, IaC, tooling, security).
    * **Opportunity (Development/DevOps):** Ensure the quality and efficiency of development processes.

* **`gencraft-devops-automation/`**
    * **Content:** DevOps automation scripts, onboarding.
    * **Opportunity (DevOps):** Improve efficiency through automation.

* **Application Code Repositories (Current Placeholders):**
    * `gencraft-client/`, `gencraft-server/`, `gencraft-pcg/`, `gencraft-service-auth/`, `gencraft-service-persistence/`.
    * **Opportunity (Development):** Work on cutting-edge technologies (procedural generation, AI, complex multiplayer systems).

* **Marketing and Sales (implied in the structure, supported by `gencraft-requirements/` and AI Gems):**
    * **Opportunity (Marketing):** Build a strong brand and an engaged community around the game.
    * **Opportunity (Sales):** Develop innovative and fair monetization strategies.

## 7. Key Principles and Conventions of this Meta-Repository

* **Documentation First:** Clear, up-to-date documentation is paramount. The `gencraft-studio-handbook/` and the `README.md` files in each repository are essential.
* **DevOps Standards:** Adherence to the standards in `devops-standards/` is expected (e.g., Conventional Commits).
* **Decision-Driven Architecture:** ADRs in `gencraft-architecture/adrs/` track major choices.
* **Modularity:** The project is broken down into modules that are as independent as possible.
* **Language:** English is the primary language for technical documentation and code, with French translations for some key documents.

## 8. Quick Start (Contribution)

1.  **Consult the `gencraft-studio-handbook/`**, especially the Studio Vision and Contribution Guide.
2.  **Refer to `devops-standards/`** and the developer onboarding guide.
3.  **Explore `gencraft-requirements/`** for the project's substance.
4.  **For infrastructure,** see `gencraft-iac/README.md`.
5.  **Before any creation,** check templates in `gencraft-requirements/09_Project_Resources/Templates/` and `gencraft-studio-handbook/02-Knowledge-Base-Hub/Templates/`.

## 9. Conclusion

GenCraft is an ambitious and exciting project with the potential to redefine the sandbox game genre. We are convinced that, together, we can create a game that will delight players worldwide.

## 10. Current Status and Contacts

This project is in an active phase of design and initial structuring. For any questions:
* General questions: [Project Lead Name / Main Communication Channel]
* Technical/architecture questions: [Lead Architect Name / Dedicated Channel]
* Process/standards questions: `gencraft-studio-handbook/` or Governance Crew.

---

This `README.md` is a living document. Please keep it updated as the project evolves.
