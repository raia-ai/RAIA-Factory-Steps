##### Link to Master Prompt for Support Audit: 
https://docs.google.com/document/d/18HIZZg6TYldUVOZtIno4Il1EM7a0qBBqKF6ztHO7Nkg/edit?usp=sharing

**Owner:** Gainesville Labs Team (QA) - may be later automated 

**Description:** Before the agent is built, an internal AI audit is performed on the training data. This is NOT an audit of the agent itself, but rather an audit of the training materials and knowledge base. The audit takes the content from the vector store and matches it against a set of test tickets or example queries to ensure the AI will have sufficient knowledge to answer them. If there are no tickets or example queries available, we can generate some using ai or prompt ai to perform the audit based on being able to answer T1, T2, T3 support inquires.

**Key Activities:**
- Create zip file of knowledge base and tickets
- Feed training data into Manus AI & use the Master Audit prompt (if doing for support)
- Generate audit report showing ticket coverage
- Note gaps in knowledge base
- Review documentation quality and formatting
	- Ensure that no mention of: "Created by Manus" or "Authored by Manus" is in there. 
	- Ensure no ai generated images that look like fake dashboards or CRM UI's are not in there.
	- Ensure no ROI Analysis or any mention of Money on these reports
	- Account for clients who help customers with multiple languages, sometimes coverage can seem "low" due to training docs not being in certain languages, however LLM's dont necessarily care as they can speak in most languages.
- Check taxonomy and knowledge graph integrity
- Aim for 60-80%+ coverage by AI

**Audit Components:**
1. **Documentation Quality Audit:** Checks formatting, taxonomy, and knowledge  integrity
2. **Coverage Audit:** Tests whether the vector store content can answer client's historical tickets

**Critical Insight:** This audit answers the question: "If the AI has this vector store, will it be able to answer these tickets in the future?"

**Failure Loop:** If the audit fails or shows insufficient coverage, the project loops back to either:
- **Step 5 (Docs):** If documents are missing or need to be recreated
- **Step 6 (ETL):** If the ETL process needs to be fixed or improved
- We may also have Andres reach back out to the client to ask for more training materials due to the initial training materials given were not enough. 

**Milestone/Deliverable:** AI audit report showing 60-80% coverage, with documentation of any gaps or issues. Extract the audit into PDF & upload to JIRA and Google Drive + notify Google Chat space.

**Notes:** This step is critical for catching issues early before investing time in agent building. The audit should be completed quickly to maintain project momentum. Thomas is working on automating the documentation aspects of this QA process.
