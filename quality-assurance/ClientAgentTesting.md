# 10. Client Agent Testing

**Owner:** Client (with support from team)

**Description:** After internal testing, the agent is handed over to the client for their own testing. The client is provided with guidance and support to help them effectively test the agent and provide feedback. This is an opportunity for the client to validate that the agent meets their requirements and expectations.

**Key Steps:**

1. Generate test questions with Manus
2. Populate test scenarios in co-pilot
3. Ensure the feedback skill is configured on the agent before sending to client
4. Send Loom videos or walkthrough guides to client on how to use copilot & test agent
5. Collect client feedback and iterations. Sometimes their feedback will be put into a document which you can find in the Google Drive folder CLIENT FEEDBACK
6. Look at feedback skill after client confirms their testing is done
7. Iterate on agent based on feedback

**Testing Environment:** Clients primarily test in the co-pilot environment, not in their production systems yet.

**Client Feedback Iteration:** This step may involve multiple rounds of feedback and iteration as the client refines their requirements and tests various scenarios.

**Failure Loop:** If client testing reveals significant issues, the project loops back to:

* **Step 10 (Internal QA):** For issues that should have been caught internally
* **Step 9 (Agent Build):** For configuration or prompt changes
* **Step 8 (Custom Workflow):** For workflow modifications

**Milestone/Deliverable:** Client approval to proceed to end-to-end testing. Usually this is notified to the team via Andres.

**Note:** This step is client-facing and may take variable amounts of time depending on client availability and responsiveness. The team provides support but the client drives the testing process.
