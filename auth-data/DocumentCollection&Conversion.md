# 4. Document Collection & Conversion

**Owner:** Gainesville Labs Team

**Description:** This step involves collecting and preparing the client's documents and knowledge base for ingestion by the AI. This includes retrieving documents from various sources (SharePoint, Website Scrape, Knowledge Base Articles, Google Drive, etc.), and converting them into a usable format, cleaning the data, and structuring it in a way that the AI can effectively utilize. This is a critical step in ensuring the quality of the AI agent's knowledge base.

**Key ASteps:**

1. Retrieve documents from SharePoint drives, Google Drive, and other sources (Usually in TRAINING - SOURCE file in Google Drive)
2. Collect support tickets and historical data
3. Convert documents into markdown (.md) format
4. Clean and structure data for AI ingestion (make sure to look inside the documents to see if there is any strange formatting)
5. You will usually be using: [https://raiaconnect.com/dashboard-home](https://raiaconnect.com/dashboard-home) to convert documents.
6. Organize documents by category or topic
7. Use consistent and proper naming convention. For example, if the file is from a knowledge base article about a product it would be "KB-PRODUCT.md"
8. Prepare knowledge base taxonomy
9. Put ALL converted files into TRAINING - MD Google Drive Folder
10. Conduct pre-audit using Manus AI of materials to ensure completeness (upload the Articles/Training and ask AI to categorize the articles, etc)

**Key Considerations:**

* Volume of documents is a scaling factor for project cost and timeline
* Document quality and formatting affect AI performance
* Proper taxonomy and organization are important
* A github -> gitbook may need to be made for the client to easily view/access/edit the training. This would require use of Manus AI to create a taxonomy / Table of contents & zip folder to import into Github which then syncs to Gitbook. This also would require YAML frontmatter for each MD.
* Sometimes we may upload the documents manually into the Agent's vector store depending on volume

**Milestone/Deliverable:** Complete set of cleaned, MD formatted documents ready for ETL processing inside Google Drive TRAINING - MD folder. Make to sure always update the JIRA and Google Chat Space notifying that this is completed.

**Notes:** This step can begin in parallel with Auth verification once basic access is confirmed. The quality of document preparation directly impacts the AI agent's performance.
