**Owner:** RAIA Devs (Sarasota HQ or Trained Gainesville Deveopers)

**Description:** If the AI agent requires custom functionalities, such as integrating with third-party applications or performing specific actions, a custom workflow is designed and built in this step. usually in n8n. This is often the most complex and time-consuming part of the development process and requires specialized skills in workflow automation tools like N8N.

**Key Activities:**
- Map out Blueprint Workflow chart (Can be done in whiteboard, Google Drawings, Whimsical, etc)
- Build workflow in N8N
- Implement function calling and escalation buttons as needed
- Create integrations with third-party applications
- Test workflow logic and error handling
- Document workflow design and functionality (sticky notes, looms, etc so others can be on the same page when viewing the workflow blind)
- Create & running test scenarios in collaboration with client

**Complexity Factors:**
- Custom workflows are never exactly the same between clients
- Each integration point adds 20-50 hours to project timeline
- Sophisticated agent features (escalation, function calling) require advanced skills
- Authentication setup should be completed way early in the process already before this step

**Milestone/Deliverable:** Functional custom workflow with documentation, ready for integration with agent. fully tested by dev. Please update with link to wf's in JIRA + Google Chat Space when done. 

**Notes:** Not all agents require custom workflows. Simple support agents may only need template ETL. This step is skipped if no custom functionality is required. The team encourages clients with developers to handle parts of this work using provided best practices documentation.

***Bottleneck Identification:** This step has been identified as one of the biggest challenges and bottlenecks in the factory process. The team is addressing this by:*
- *Identifying individuals with technical skills*
- *Moving them directly into N8N testing and training*
- *Dedicating several weeks to training (high-value skill)*
- *Creating best practices documentation*
- *Building node libraries and pre-built connectors*

***Team Structure:** A team of devs focused on N8N workflows doesn't necessarily require 20 hours/week per person; 10 hours might be sufficient for complex workflows, especially if authentication is set up early.*