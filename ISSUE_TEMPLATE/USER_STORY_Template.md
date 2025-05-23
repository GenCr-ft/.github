# User Story: [Short Title Describing Action] (`US-XXX`)

* **Story ID:** `US-XXX` (Assign unique ID)
* **Title:** [Short Title Describing Action, e.g., Place Voxel Block]
* **Status:** [e.g., New, Ready for Dev, In Dev, Ready for QA, Done]
* **Date Created/Updated:** [YYYY-MM-DD]
* **Owner:** [Name or Role, e.g., Product Owner]
* **Parent Feature:** [`FEATURE-YYY: Feature Title`](../FEATURE-YYY_Title.md)
* **Related Epic:** [`EPIC-ZZZ: Epic Title`](../../Epics/EPIC-ZZZ_Title.md)
* **Priority:** [e.g., Must Have (MVP), Should Have, Could Have, Won't Have this time]
* **Estimate (Optional):** [Story Points, T-Shirt Size, etc.]

---

## User Story

**As a** [Type of user / Persona, e.g., P-ARC]
**I want to** [Perform some action, e.g., place a wood block onto an existing surface]
**So that** [Benefit / Goal, e.g., I can build the walls of my base]

---

## Conversation / Details / Notes

* *[Add any additional context, clarifications from discussions, specific business rules relevant to this story not covered elsewhere, or assumptions.]*
    * Placement should use the snapping system.
    * The block must be consumed from inventory.
    * Visual feedback for placement should be clear.

---

## Acceptance Criteria

* [ ] **AC 1:** Given the player has a wood block in their hotbar/inventory and is looking at a valid surface, when they perform the place action, then a wood block appears on the surface at the targeted location.
* [ ] **AC 2:** Given the block is placed successfully, when the player checks their inventory, then the wood block count has decreased by 1.
* [ ] **AC 3:** Given the player is targeting an invalid surface (e.g., air, too far away), when they attempt the place action, then no block is placed and no block is consumed from inventory.
* [ ] **AC 4:** Given the player places a block, when the action completes, then a placement sound effect is played.
* [ ] **AC 5:** Verify that the placed block persists after saving and loading the game (if applicable at this stage).
* ...

---

## UI / UX Links (Optional)

* [Link to specific Mockup ZZZ if relevant to this story]

---

## Technical Notes (Optional)

* [Any technical hints or constraints useful for the developer, e.g., Use VoxelService.placeBlock() API, Consider multiplayer permissions.]

---
