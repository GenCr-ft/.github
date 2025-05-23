# Feature: [Clear and Concise Feature Title] (`FEATURE-XXX`)

* **Feature ID:** `FEATURE-XXX` (Assign unique ID)
* **Title:** [Clear and Concise Feature Title]
* **Status:** [e.g., Draft, Ready for Dev, In Progress, Ready for QA, Done, On Hold]
* **Date Created/Updated:** [YYYY-MM-DD]
* **Owner:** [Name or Role, e.g., Product Owner]
* **Parent Epic:** [`EPIC-YYY: Parent Epic Title`](../Epics/EPIC-YYY_Title.md)
* **Related Release(s):** [e.g., MVP, MVP+1]

---

## 1. Summary

* *[Briefly describe (1-2 sentences) what this feature does and the value it provides.]*

---

## 2. Rationale / User Goal

* *[Explain why this feature is needed. What user need (Persona?) does it address? What business goal does it support? Link to the parent Epic's objective.]*

---

## 3. Associated User Stories

* *[List the specific User Stories that make up this feature. Include relative links if User Stories are in separate files, or write them directly here if the chosen structure keeps US within the Feature file.]*
    * [US-AAA: User Story Title A](./user_stories/US-AAA_Title.md)
    * [US-BBB: User Story Title B](./user_stories/US-BBB_Title.md)
    * *OR*
    * **US-AAA:** As a [Persona], I want to [action], so that [benefit].
    * **US-BBB:** As a [Persona], I want to [action], so that [benefit].

---

## 4. Functional Specification / Business Rules

* *[Describe in detail how the feature works. Use subsections, lists, tables as needed.]*

    ### 4.1. Core Behavior
    * [Detail the primary workflow.]

    ### 4.2. Specific Rules
    * Rule 1: [Condition] -> [Action/Result]
    * Rule 2: [Specific limit, validation, calculation]

    ### 4.3. Edge Cases / Error Handling
    * Handling Error X: [Expected behavior]
    * Edge Case Y: [Expected behavior]

    ### 4.4. Data Involved (Optional)
    * [Data types handled, expected format, etc.]

    ### 4.5. Flow Diagram (Optional - Mermaid)
    ```mermaid
    graph TD
        A[Start] --> B{Condition?};
        B -- Yes --> C[Action 1];
        B -- No --> D[Action 2];
        C --> E[End];
        D --> E[End];
    ```

---

## 5. UI / UX Considerations

* *[Describe key UI elements or specific interaction flows. Reference mockups or wireframes (link to Section 07) if available.]*
    * Main Screen: [Link to Mockup XXX]
    * Key Interaction: [Describe expected behavior of Button Y]

---

## 6. Acceptance Criteria

* *[List the specific, testable, clear criteria that must be met for this feature to be considered complete. Often derived from User Stories.]*
    * Criterion 1: Given [context], when [action], then [expected outcome].
    * Criterion 2: Verify that [specific condition is true].
    * Criterion 3: The system correctly handles [error case Z].
    * ...

---

## 7. Specific Non-Functional Requirements (NFRs)

* *[List NFRs that particularly apply to this Feature.]*
    * **Performance:** [e.g., Screen Z must load in under N seconds on recommended config.]
    * **Security:** [e.g., Data entered in this form must be server-side validated.]

---

## 8. Dependencies

* *[List other Features, systems, APIs, assets, or data this Feature depends on to function.]*

---

## 9. Open Questions / Design Notes

* *[Document any outstanding points, specific design choices made, or assumptions.]*

---
