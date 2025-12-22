# Phase 4: Quality Assurance

**Owner:** HQ Team (Rich, Aurec, Thomas) and Gainesville Labs QA

**Description:** Once the agent is built, it undergoes an internal testing process. The QA team tests the agent's knowledge, functionality, and overall performance to identify any bugs or issues. This is a critical step in ensuring the agent is ready for client testing.

**Key Steps:**

1. Test agent responses against known queries generated via example tickets, training
   * We will usually generate 100 test queries using ai and example tickets, which then get ran via raia connect.
2. Verify knowledge base articles & training docs are referenced properly and accuracy
3. Test custom workflows and integrations
4. Check agent personality and tone consistency
5. Identify edge cases and error scenarios
6. Document any bugs or issues
7. Test guardrails and off topic-ness
8. Iterate on prompts and configuration as needed (Usually prompt adjustments are done by the person who initially created the agent system prompt instructions.)

**Testing Focus:**

* Agent knowledge coverage and accuracy
* Response quality and relevance
* Workflow functionality and error handling
* Any potential integration points with third-party systems
* Performance and response time

**Failure Loop:** If internal QA identifies significant issues, the project may loop back to:

* **Step 9 (Agent Build):** For prompt or configuration issues
* **Step 8 (Custom Workflow):** For workflow bugs or logic errors
* **Step 7 (AI Audit):** If knowledge base gaps are discovered

**Milestone/Deliverable:** Internal QA team confirming agent is ready for client testing. Update JIRA + Google Chat Space

**Notes:** This is where the team tests the agent thoroughly before exposing it to the client. The goal is to catch and fix issues internally before client involvement.
