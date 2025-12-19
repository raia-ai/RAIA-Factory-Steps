## Process Management & Best Practices

### Jira Structure

The factory process is managed in Jira with the following structure:

- **One Agent = One Epic:** Each AI agent being built is represented as a single epic in Jira
- **Steps as Columns:** Each of the 15 steps is a column in the Kanban board
- **Subtasks:** Within each epic, subtasks are created for specific activities and assigned to team members
- **Milestones:** Milestones are set at key transition points to trigger notifications for downstream personnel
- **Timeline View:** The Gantt chart view shows all agents in progress with their 100-day timeline

### Column Movement Philosophy

The ideal flow is that once an agent moves into a new column, it should never revert to a previous column. If it does, this indicates:

- **Process Failure:** A step was missed or not completed properly
- **Scope Creep:** Client introduced new requirements or data late in the process
- **Client Data Issues:** Client forgot to provide necessary information

**Exception:** QA going back to Dev is natural and expected as part of the quality assurance process.

### Blocking and Holds

Rather than creating separate "blocked" or "on hold" columns, cards remain in their current column and are tagged with a "Hold" or "Blocked" status. This ensures our team always knows what step the agent was in when it was blocked.

**Common Blocking Scenarios:**
- Waiting on client to provide credentials
- Waiting on security compliance approval
- Waiting on client feedback during testing

### Phase Ownership

The 15 steps are grouped by ownership to enable clear handoffs:

- **Setup (Steps 1-3):** Primarily Andres Pareja, with Sales team involvement
- **Auth (Step 4):** Gainesville Labs developers
- **Docs (Step 5):** Gainesville Labs team
- **Dev (Steps 6, 8-9):** Mix of Gainesville Labs and HQ specialists (for custom workflows)
- **QA (Steps 7, 10-12):** Mix of Gainesville Labs QA and HQ team
- **Live (Steps 13-15):** Team and client collaboration

This structure allows team members to focus on their specific areas of expertise without needing to track the entire process.

---

## Timeline & Pricing Insights

### 100-Day Roadmap

While a basic agent can be built in just a few days, the 100-day timeline accounts for:

- Custom workflow development
- Back-and-forth communication with clients
- Time spent waiting on client responses
- Multiple rounds of testing and iteration
- Integration complexity

The 100-day roadmap is primarily a client communication tool to set expectations about the process duration, especially for projects with integration work and tiered support needs.


---

## Team Structure & Training

### Gainesville Labs Integration

The factory process is designed to incorporate Gainesville Labs. The process is:

- **Clear:** Obvious start and end points for each step
- **Simple:** Easy to understand for new team members
- **Structured:** Clear handoffs between phases
- **Documented:** Comprehensive documentation and training materials

### Developer Certification Program

The long-term goal is to encourage every CSI company to have a certified Raia developer who has completed the Labs training. This enables clients to:

- Handle some custom workflow development themselves
- Reduce project costs
- Maintain and extend their agents independently
- Follow best practices established by our team
---

## Tools & Automation

### Current Tool Development

**Access Management Tool:** Helps bridge the gap in getting API keys and credentials from clients. Provides a structured interface for requesting and tracking access.

**ETL Templates:** Pre-built connectors for common platforms (HubSpot, Salesforce, SharePoint, etc.) to reduce custom development time.

**Audit Automation:** Thomas Hall is working on automating the documentation aspects of QA, including creating zip files of knowledge bases and tickets for Manus audit.

**Starter Prompts:** Using Manus workflows to generate starter system prompts and simulated tickets to accelerate agent builds.

**Directory Automation:** Streamlining the creation of consistent directory structures across Jira, Google Drive, and other platforms.

### Milestone Deliverables

Every step in the factory process should have:

- **A clear deliverable:** Something tangible that can be handed off to the next phase
- **A milestone:** A checkpoint that triggers notifications for downstream personnel
- **Documentation:** Evidence that the step was completed properly

Examples:
- **Step 3 (Access):** Auth paperwork sent to client, credentials documented
- **Step 7 (AI Audit):** Audit report showing 60-80% coverage
- **Step 10 (Internal QA):** QA report confirming agent is ready for client testing

---

## Key Success Factors

### Simplification Focus

Our team is actively working to:
- Eliminate over-engineering
- Remove wasted effort
- Simplify processes
- Focus on what has impact on the business

### Quality Gates

The process includes multiple quality gates to catch issues early:

1. **Pre-Audit (Step 5):** Ensures documents are complete before ETL
2. **Internal AI Audit (Step 7):** Validates knowledge base before agent build
3. **Internal QA (Step 10):** Catches issues before client involvement
4. **Client Agent Test (Step 11):** Validates client requirements
5. **End-to-End Test (Step 12):** Final validation before launch

---

## Conclusion

The AI Agent Building Process Lifecycle represents a mature, scalable approach to building AI agents. By breaking the process into 15 discrete steps across 5 phases, our team has created a factory model that can:

- Scale to handle multiple agents simultaneously
- Onboard and train new team members effectively
- Maintain quality through structured gates
- Manage client expectations through transparency
- Reduce bottlenecks through specialization and automation

The process continues to evolve based on lessons learned, with ongoing efforts to simplify, automate, and optimize each step.
