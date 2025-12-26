# 8. AI Agent Build

**Owner:** Gainesville Labs Team

**Description:** With the knowledge base and any custom workflows in place, the AI agent is built (usually on the Raia platform / raia2.com). This involves uploading all information into the vector store, configuring the agent's advanced training & model settings, defining its personality and tone, and writing the system prompt instructions that will guide its behavior.

**Key Steps:**

1. Making sure that all converted documents are uploaded to the agent's vector store
2. Configure agent settings and parameters (model version, file search, etc)
3. Write system prompts and instructions - Feel free to edit and use [Aurec's Master prompt](https://docs.google.com/document/d/18QuYMH716yoD6P_8WaxtuiklGYIl6TGa-DNMqyum_V4/edit?tab=t.0) & adjust as needed.
4. Define agent personality and tone (warm, concise, professional, casual, etc)
5. Set up model selection and configuration
6. Configure response guard rails (add the global policy/Content packs, put inside the instructions to not veer off topic, etc)
7. Begin initial testing a few queries within copilot. (Make sure the agent generally works for the overall goal and guardrails)

**Prerequisites:**

* ETL setup must be complete
* Internal AI audit must show sufficient coverage

**Support Tools:** Thomas is working on creating simulated tickets using Manus workflows to accelerate the agent build process.

**Key Insight:** The team should be able to start testing the agent within this phase, though formal QA (simulations via raia connect) happens in the next step.

**Milestone/Deliverable:** Fully configured / pre-tested AI agent ready for internal QA testing. Update when completed JIRA + Google Chat Space

**Note:** This step should not begin until the Internal AI Audit passes, as audit failures often require changes to documents or ETL that would impact the agent build. By waiting, the team avoids rework.
