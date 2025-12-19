**Owner:** Gainesville Labs Team

**Description:** This step involves collecting and preparing the client's documents and knowledge base for ingestion by the AI. This includes retrieving documents from various sources (SharePoint, Website Scrape, Knowledge Base Articles, Google Drive, etc.), and converting them into a usable format, cleaning the data, and structuring it in a way that the AI can effectively utilize. This is a critical step in ensuring the quality of the AI agent's knowledge base.

**Key Activities:**
- Retrieve documents from SharePoint drives, Google Drive, and other sources (Usually in TRAINING - SOURCE file in Google Drive)
- Collect support tickets and historical data
- Convert documents into markdown (.md) format
- Clean and structure data for AI ingestion (make sure to look inside the documents to see if there is any strange formatting)
- You will usually be using https://raiaconnect.com/dashboard-home to convert documents.
- Organize documents by category or topic
- Use consistent and proper naming convention. For example, if the file is from a knowledge base article about a product it would be "KB-PRODUCT.md"
- Prepare knowledge base taxonomy
- Put ALL converted files into TRAINING - MD Google Drive Folder
- Conduct pre-audit using Manus AI of materials to ensure completeness (upload the Articles/Training and ask AI to categorize the articles, etc)

**Key Considerations:**
- Volume of documents is a scaling factor for project cost and timeline
- Document quality and formatting affect AI performance
- Proper taxonomy and organization are important
- A github -> gitbook may need to be made for the client to easily view/access/edit the training. This would require use of Manus AI to create a taxonomy / Table of contents & zip folder to import into Github which then syncs to Gitbook. This also would require YAML frontmatter for each MD.
- Sometimes we may upload the documents manually into the Agent's vector store depending on volume

**Milestone/Deliverable:** Complete set of cleaned, MD formatted documents ready for ETL processing inside Google Drive TRAINING - MD folder. Make to sure always update the JIRA and Google Chat Space notifying that this is completed.

**Notes:** This step can begin in parallel with Auth verification once basic access is confirmed. The quality of document preparation directly impacts the AI agent's performance.
