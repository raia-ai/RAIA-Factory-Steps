# Phase 2: Auth & Data

**Owner**: Gainesville Labs Dev Team / Aurec

**Description**: In this step, the labs team verifies the API / Auth credentials provided by the client to ensure they have the necessary permissions to access the required systems and data. The appropriate auths will be identified in the onboarding call. This verification is critical to prevent roadblocks later in the development process. The team tests API connections, and data access to confirm everything works as expected.

1. Aurec will copy over a templated workflow from N8N & create a Client Folder in N8N.&#x20;
2. From there you will go to that workflow and take the necessary auth/api keys from either the Google Drive Folder or Jira and input these into the appropriate nodes in n8n.&#x20;

<p align="center"><em>This could be an https request node, setting up a predefined credential, or even setting up an OAuth2.</em></p>

3. After setting up and inputting the credentials, you will need to test the nodes and workflow to make sure the credentials work & are setup properly.

<p align="center"><em>If the credentials don't work you will need to inform Aurec &#x26; Andres to troubleshoot if our setup is incorrect, if we didn't read the documentation to setup correctly, or if the client gave us the wrong credentials/authorizations.</em></p>

4. If something does not work, it needs to be noted in JIRA + Google Chat.

**Challenges**:

• Credentials may not have admin-level access when required

• GitHub tokens may be regular tokens instead of Personal Access Tokens (PAT)

• API keys may have insufficient permissions

• API endpoints may be setup incorrectly

• You may need to create a JWT

**Milestone/Deliverable:** Documenting in JIRA + Gchat space confirming all systems are accessible and ready for development

**Note:** If verification fails, the card stays in this column until issues are resolved. The team may need to work with Andres to request corrected credentials from the client. This step ensures developers have everything they need before starting ETL work.
