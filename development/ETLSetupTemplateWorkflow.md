# Phase 3: Development

**Owner:** Gainesville Labs Dev Team / Aurec

**Description:** ETL (Extract, Transform, Load) is the process of extracting data from various sources, transforming it into a consistent format, and loading it into the AI's vector store. This step primarily uses pre-built templates for common data sources, though custom ETL workflows can be created for more complex integrations. This can be thought of in the same vein as the previous step except that this is automating & at mass extracting data/docs from various sources. Where as the, Docs - Convert to AI step may have just been converting already provided documents that are easily exported from the client's side.

**Key Steps:**

1. Select appropriate ETL template based on the data sources listed [in the n8n folder.](https://raia.app.n8n.cloud/projects/T9NHCi5HCuLOIJcZ/folders/7Ww0b1QESlC39iif/workflows)
2. Configure template parameters for client-specific requirements (Sources, Limits on how many requests we can send in a certain time period, etc)
3. Extract data.
4. Transform data into consistent markdown format (can be done inside the workflow)
5. Load processed data files into the agent's vector store (can be done inside the workflow)
6. Create documentation of ETL pipeline
7. Test data flow and integrity

**Template vs. Custom:**

* **Template ETL:** Most projects use pre-built templates for common sources (HubSpot, Salesforce, SharePoint, etc.)
* **Custom ETL:** Only created when client has unique data sources or complex transformation requirements
* Templates can be customized with client-specific parameters

**Key Considerations:**

* ETL templates should be reusable across similar projects
* Pre-built connectors exist for common platforms
* Thomas is working on creating node and function libraries within N8N
* Good ETL coverage is essential for the AI audit in the next step

**Milestone/Deliverable:** Functional ETL pipeline with data successfully loaded into vector store, documented in project files. Make sure to update the JIRA and Google Chat space.

**Notes:** The team aims to templatize as many ETL workflows as possible to reduce development time. If a custom ETL is needed, it may require more specialized dev skills.
