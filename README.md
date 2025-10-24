Sprint Pre-Planning Jira Ticket Creation Report
Meeting Date: October 24, 2025
Prepared by: Jake
Total Tickets to Create/Modify: 27

SECTION 1: EPIC CREATION
Epic 1: Unstructured Data Intake Proof of Concept

Type: Epic
Components:

Proof of concept development
White paper creation
Cost analysis
Azure resource integration planning


Risk Level: High (CIO approval required)
Constraints: No Hugging Face models, no whitelisted LLMs, only XGB wrap model permitted
Child Stories: Will include cost analysis, technical implementation, white paper

Epic 2075: SPC Integration with NPD (Existing - Needs Update)

Type: Epic (existing)
Status: Blocked - pending statistician personnel decision
Action Required: Follow-up with Mike Gorman


SECTION 2: NEW STORIES TO CREATE
1. Epic Writing Session

Assignees: Speaker 1 & Speaker 2
Due Date: Before November 7th
Description: Write all epics based on new priorities and projects for 12-week planning session
Priority: High

2. Story Drafting for 12-Week Planning

Assignees: Speaker 1 & Speaker 2
Due Date: Before November 7th
Description: Draft 4-5 stories per epic to create robust story pool
Deliverable: Complete story backlog for planning session

3. Add Cost Analysis to Unstructured Data PoC

Assignees: Speaker 1 & Speaker 2
Parent Epic: Unstructured Data Intake PoC
Description: Develop estimated cost model for all required components including Azure resources, whitelisting requirements, and Databricks integration
Note: Must be exceptionally robust to avoid CIO rejection

4. Hide Monetary Cost Visuals - Databricks Dashboard

Dashboard: "USCIS Databricks DBU and cost summary"
Description: Remove/hide all visuals displaying monetary costs while retaining underlying queries and tables
Priority: High - enables sharing

5. Add Contractual Notice to Dashboard

Description: Add text notice: "Cost metrics are unavailable due to private contractual agreements with Databricks"
Related to: Ticket #4

6. Rename Project to Portfolio Metrics

Old Name: Current cost/usage analytics
New Name: "Data Enterprise Projects Portfolio metrics"
Scope: Expand to portfolio-level coverage

7. Obtain AA Team Permissions

Assignee: Speaker 1
Contact: Ben Steiner
Description: Request job lists and permissions from AA team for portfolio analytics
Risk: AA team historically unresponsive

8. Obtain NPD Team Permissions

Assignee: Speaker 1
Contact: Mike Gorman
Description: Request job lists and permissions from NPD team

9. Obtain E2E Team Permissions

Assignee: Speaker 1
Description: Request job lists and permissions for portfolio integration

10. Obtain GDS Team Permissions

Assignee: Speaker 1
Description: Request job lists and permissions for portfolio integration

11. Obtain SCP Team Permissions

Assignee: Speaker 1
Description: Request job lists and permissions for portfolio integration

12. Bug: Dashboard Visual Mismatch

Type: Bug
Dashboard: Table Metadata Analysis
Issue: Table visual doesn't match corresponding bar chart
Priority: Medium

13. Integrate Table Cleanup Log

Source: "Table cleanup log"
Target: "Table Metadata Analysis" dashboard
Description: Show cleanup impact and trends

14. Rerun Table Cleanup Script

Description: Execute cleanup script for tables with excessive small files
Note: Previous run only partially effective

15. Delete "Delete Me" Tables

Description: Remove all tables marked for deletion
Type: Cleanup task

16. Update Table Ownership

Description: Change table ownership from individuals to groups
Action: Outreach required to update assignments

17. Record Teddy Talk Rehearsal - Jake

Assignee: Speaker 1 (Jake)
Due Date: Monday
Description: Record rehearsal version for internal review

18. Record Teddy Talk Final Version - Jake

Assignee: Speaker 1 (Jake)
Due Date: Thursday
Description: Record production-quality video

19. Send Teddy Talk to Leadership

Assignee: Speaker 1 (Jake)
Due Date: Thursday
Description: Submit final version for leadership review

20. Remove Master Collect Tasks from Daily Ephemeral

Type: Technical Optimization
Description: Remove 2 master collect tasks from daily ephemeral job cluster
Purpose: Optimize job cluster performance

21. UOBI-2173: Schedule Table Validation Meeting

Type: Story (continuation)
Attendees: Josh Williamson, WARM team
Description: Validate latest tables and add filing type dimensionality if approved

22. UOBI-2173: Validate CDO Lookup Table Lineage

Type: Story (continuation)
Issue: Table hasn't been updated in 9 months
Actions: Check lineage, validate accuracy, document findings

23. Create Teddy Talk - Nate Lanfranca

Assignee: Nate Lanfranca
Type: Story
Description: Create separate Teddy Talk for leadership

24. NPD Statistical Process Controls Kickoff Meeting

Organizer: Nate Lanfranca (Data Engineering Federal Lead)
Attendees: Mike Gorman, Josh Williamson, NPD team
Deliverables:

Meeting setup
Business need report
Problem scope documentation



25. Update Onboarding Documentation

Assignee: Jake
Location: Data Engineering Confluence space
Description: Prepare comprehensive onboarding materials for incoming new hire

26. Document FY26 Priorities and Jira Label Strategy

Assignee: Jake
Deliverables:

Add FY26 priorities to Confluence
Document DE/DSP team alignment to D1 & OPQ priorities
Create Jira label usage guide



27. Create AI Presentation Part IV for MESH

Assignee: Jake
Description: Continue AI presentation series (Part IV) for MESH meeting


SECTION 3: TICKETS TO CLONE/MODIFY
Clone Issue 2175 - Liquid Clustering

Assignee: Andre
Current Success: DBUs reduced from 1,000-1,003 to 919
Action: Clone for continued work across all applicable jobs
Timeline: Multiple sprints
Future Rollout: AA, E22, and NPD teams

Clone Current Sprint Carryover Issues

Assignee: Speaker 3
Description: Identify and clone all tickets that need to continue into next sprint

Add Sue's Requested Tickets

Assignee: Speaker 2
Description: Add specific tickets Sue messaged about to next sprint
Note: Ensure she has work ready at sprint start

Pull Andre's Backlog Items

Action Needed: Identify specific tickets from Andre's backlog
Note: Andre has existing work ready to pull

Finish and Publish Mesh Confluence Draft

Assignee: Speaker 1
Due Date: Today
Status: Currently saved as draft
Action: Complete and publish


SECTION 4: IMPLEMENTATION TIMELINE
Immediate (Today)

Publish Mesh Confluence draft

This Week

Monday: Record Teddy Talk rehearsal (Jake)
Thursday: Record and submit final Teddy Talk (Jake)
Hide cost visuals on dashboard
Add contractual notice

Next Sprint

Add Sue's requested tickets
Pull Andre's backlog items
Clone carryover issues
UOBI-2173 continuation stories
Remove master collect tasks
Update onboarding documentation
Document FY26 priorities
Create AI Presentation Part IV

Before November 7th

Complete all epic writing
Draft 4-5 stories per epic
Setup unstructured data PoC epic

Ongoing/Multi-Sprint

Liquid clustering implementation
Portfolio metrics expansion (all team permissions)
SPC/NPD integration
Table metadata cleanup activities


SECTION 5: DEPENDENCIES & BLOCKERS
Known Blockers:

SPC/NPD Integration: Waiting on statistician personnel decision
AA Team Permissions: Historically unresponsive team
Unstructured Data PoC: High risk of CIO/security rejection

Dependencies:

Portfolio expansion requires permissions from 5 teams
Liquid clustering rollout depends on current program completion
12-week planning requires epic/story completion by November 7th


SECTION 6: RISK NOTES

Unstructured Data PoC - Extreme technical constraints and high rejection risk
AA Team Integration - Past unresponsiveness may delay portfolio expansion
Table Cleanup - Previous attempts only partially successful, may need process revision
Multiple Teddy Talks - Coordination needed between Jake and Nate versions

