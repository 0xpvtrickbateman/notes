# **Complete Jira Stories for Sprint Pre-Planning**
**Date:** October 24, 2025  
**Total Stories:** 27

---

## **STORY 1**
**Title:** Write All Epics for 12-Week Planning Session

**Description:** Create comprehensive epics based on new organizational priorities and projects in preparation for the November 7th 12-week planning session. Partner with Speaker 2 to ensure all new initiatives are properly captured and structured as epics.

**Value Add:** Establishes clear project roadmap for next 12 weeks, ensures team alignment with organizational priorities, and provides foundation for resource planning and sprint capacity management.

**Acceptance Criteria:**
- [ ] All new priorities have corresponding epics created
- [ ] Each epic includes clear scope and objectives
- [ ] Epics are properly linked to FY26 priorities
- [ ] Review completed with Speaker 2
- [ ] All epics ready for November 7th planning session

---

## **STORY 2**
**Title:** Draft 4-5 Stories Per Epic for Story Pool

**Description:** Create detailed user stories for each epic established for the 12-week planning session. Each epic should have 4-5 stories drafted to ensure adequate work breakdown and sprint planning flexibility.

**Value Add:** Provides ready backlog for immediate sprint execution, reduces planning overhead during sprints, and ensures consistent team velocity through pre-defined work packages.

**Acceptance Criteria:**
- [ ] Each epic has minimum 4 stories drafted
- [ ] Stories follow standard format with clear acceptance criteria
- [ ] Story points estimated for capacity planning
- [ ] Stories reviewed and approved by team lead
- [ ] Complete before November 7th planning session

---

## **STORY 3**
**Title:** Add Cost Analysis to Unstructured Data PoC Proposal

**Description:** Develop comprehensive cost estimation model for the unstructured data proof of concept, including Azure resource integration costs, whitelisting requirements, and Databricks implementation expenses. Must address constraints including prohibited Hugging Face models and lack of whitelisted LLMs.

**Value Add:** Demonstrates fiscal due diligence to leadership, increases probability of CIO approval, and provides budget transparency for resource allocation decisions.

**Acceptance Criteria:**
- [ ] Cost model includes all Azure resource requirements
- [ ] Whitelisting process costs documented
- [ ] Databricks integration expenses calculated
- [ ] Risk mitigation strategies for technical constraints included
- [ ] Document reviewed by Speaker 2
- [ ] Proposal strengthened to minimize CIO rejection risk

---

## **STORY 4**
**Title:** Hide Monetary Cost Visuals on Databricks Dashboard

**Description:** Modify the "USCIS Databricks DBU and cost summary" dashboard to remove or hide all visuals displaying monetary costs while preserving underlying queries and tables for potential future use.

**Value Add:** Enables sharing of DBU usage analytics with stakeholders while maintaining contractual confidentiality, supports data-driven decisions without violating agreements.

**Acceptance Criteria:**
- [ ] All monetary cost visuals hidden or removed
- [ ] DBU usage metrics remain visible
- [ ] Underlying queries and tables preserved
- [ ] Dashboard functionality tested
- [ ] No cost data exposed to non-authorized users

---

## **STORY 5**
**Title:** Add Contractual Notice to Cost Dashboard

**Description:** Add explanatory text notice to the modified Databricks dashboard stating "Cost metrics are unavailable due to private contractual agreements with Databricks."

**Value Add:** Provides transparency to dashboard users about missing cost data, prevents confusion and unnecessary inquiries, maintains professional communication standards.

**Acceptance Criteria:**
- [ ] Notice text added to dashboard in visible location
- [ ] Text formatting matches dashboard design standards
- [ ] Notice appears on all relevant dashboard pages
- [ ] Reviewed by legal/contracts team if required

---

## **STORY 6**
**Title:** Rename Project to "Data Enterprise Projects Portfolio Metrics"

**Description:** Update project naming conventions and documentation to reflect expansion from single program metrics to portfolio-wide analytics covering multiple teams and programs.

**Value Add:** Accurately reflects expanded project scope, improves stakeholder understanding, and positions project as enterprise-level initiative for increased visibility and support.

**Acceptance Criteria:**
- [ ] Project renamed in all documentation
- [ ] Confluence spaces updated
- [ ] Dashboard titles updated
- [ ] Communication sent to stakeholders about name change
- [ ] Jira project settings updated if applicable

---

## **STORY 7**
**Title:** Obtain AA Team Permissions for Portfolio Analytics

**Description:** Contact Ben Steiner to request job lists and permissions from the AA team for integration into the portfolio-level analytics dashboard. Document any access challenges given team's historical unresponsiveness.

**Value Add:** Enables comprehensive portfolio visibility, improves cross-team performance monitoring, and supports data-driven resource allocation decisions.

**Acceptance Criteria:**
- [ ] Initial contact made with Ben Steiner
- [ ] Permissions request formally documented
- [ ] Job lists obtained or blockers documented
- [ ] Access permissions granted or escalation path identified
- [ ] Integration requirements documented

---

## **STORY 8**
**Title:** Obtain NPD Team Permissions for Portfolio Analytics

**Description:** Contact Mike Gorman to request job lists and permissions from the NPD team for integration into the portfolio-level analytics dashboard.

**Value Add:** Expands analytics coverage to include NPD team metrics, enables cross-program performance comparison, and supports enterprise-wide optimization initiatives.

**Acceptance Criteria:**
- [ ] Contact established with Mike Gorman
- [ ] NPD job lists obtained
- [ ] Required permissions granted
- [ ] Integration requirements documented
- [ ] Timeline for integration agreed upon

---

## **STORY 9**
**Title:** Obtain E2E Team Permissions for Portfolio Analytics

**Description:** Request job lists and permissions from the E2E team for integration into the enterprise portfolio analytics dashboard.

**Value Add:** Completes portfolio coverage for end-to-end process visibility, enables identification of cross-team dependencies and bottlenecks.

**Acceptance Criteria:**
- [ ] E2E team contact identified and engaged
- [ ] Job lists and permissions obtained
- [ ] Access validated in Databricks
- [ ] Integration requirements documented

---

## **STORY 10**
**Title:** Obtain GDS Team Permissions for Portfolio Analytics

**Description:** Request job lists and permissions from the GDS team for integration into the enterprise portfolio analytics dashboard.

**Value Add:** Incorporates GDS metrics into portfolio view, enables comprehensive performance monitoring across all data teams.

**Acceptance Criteria:**
- [ ] GDS team contact identified and engaged
- [ ] Job lists and permissions obtained
- [ ] Access validated
- [ ] Integration timeline established

---

## **STORY 11**
**Title:** Obtain SCP Team Permissions for Portfolio Analytics

**Description:** Request job lists and permissions from the SCP team for integration into the enterprise portfolio analytics dashboard.

**Value Add:** Completes portfolio coverage, ensures all teams are represented in enterprise metrics, supports comprehensive resource optimization.

**Acceptance Criteria:**
- [ ] SCP team contact identified and engaged
- [ ] Permissions and job lists obtained
- [ ] Access validated
- [ ] Integration requirements documented

---

## **STORY 12**
**Title:** Fix Dashboard Visual Mismatch Bug in Table Metadata Analysis

**Description:** Investigate and resolve bug where table visual does not match corresponding bar chart on the Table Metadata Analysis dashboard.

**Value Add:** Ensures data visualization accuracy, maintains dashboard credibility, and prevents misinterpretation of metrics by stakeholders.

**Acceptance Criteria:**
- [ ] Root cause of mismatch identified
- [ ] Bug fix implemented
- [ ] Visual and bar chart display matching data
- [ ] Fix tested across different browsers
- [ ] Documentation updated if needed

---

## **STORY 13**
**Title:** Integrate Table Cleanup Log into Metadata Dashboard

**Description:** Add the "Table cleanup log" to the "Table Metadata Analysis" dashboard to display cleanup impact, trends, and effectiveness over time.

**Value Add:** Provides visibility into cleanup efforts ROI, demonstrates storage optimization progress, and supports data governance initiatives.

**Acceptance Criteria:**
- [ ] Cleanup log data source connected
- [ ] Visualizations created for cleanup trends
- [ ] Impact metrics clearly displayed
- [ ] Historical data preserved and visible
- [ ] Dashboard performance not degraded

---

## **STORY 14**
**Title:** Rerun Table Cleanup Script for Small Files

**Description:** Execute table cleanup script targeting tables with excessive small files, addressing issues from partially effective previous run.

**Value Add:** Reduces storage costs, improves query performance, and optimizes Databricks resource utilization through file consolidation.

**Acceptance Criteria:**
- [ ] Script updated to address previous run limitations
- [ ] All tables with excessive small files identified
- [ ] Cleanup script successfully executed
- [ ] Results logged and documented
- [ ] Performance improvements measured

---

## **STORY 15**
**Title:** Delete Tables Marked "Delete Me"

**Description:** Remove all tables that have been marked for deletion in the metadata system as part of ongoing cleanup efforts.

**Value Add:** Reduces storage costs, eliminates confusion from obsolete tables, and maintains clean data environment for improved governance.

**Acceptance Criteria:**
- [ ] All "delete me" tables identified
- [ ] Deletion approval obtained where required
- [ ] Tables successfully removed
- [ ] Cleanup logged in tracking system
- [ ] Storage savings documented

---

## **STORY 16**
**Title:** Update Table Ownership from Individuals to Groups

**Description:** Execute outreach campaign to update table ownership from individual users to appropriate group ownership for better continuity and governance.

**Value Add:** Ensures business continuity when individuals leave, improves accountability, and aligns with data governance best practices.

**Acceptance Criteria:**
- [ ] All individually-owned tables identified
- [ ] Appropriate group owners determined
- [ ] Outreach to current owners completed
- [ ] Ownership transfers executed
- [ ] Documentation updated to reflect new ownership

---

## **STORY 17**
**Title:** Record Teddy Talk Rehearsal Version - Jake

**Description:** Record rehearsal version of Teddy Talk presentation for internal review and feedback before final production.

**Value Add:** Enables practice and refinement of presentation, reduces risk of issues in final recording, and ensures high-quality leadership communication.

**Acceptance Criteria:**
- [ ] Rehearsal version recorded by Monday
- [ ] Video quality meets standards
- [ ] Content covers all required topics
- [ ] Internal review feedback collected
- [ ] Improvements identified for final version

---

## **STORY 18**
**Title:** Record Teddy Talk Final Production Version - Jake

**Description:** Record production-quality version of Teddy Talk incorporating feedback from rehearsal for submission to leadership.

**Value Add:** Provides leadership with professional update on team accomplishments, supports visibility of data engineering initiatives, and strengthens stakeholder engagement.

**Acceptance Criteria:**
- [ ] Final version recorded by Thursday
- [ ] Production quality standards met
- [ ] All feedback from rehearsal incorporated
- [ ] Video edited and polished
- [ ] Ready for leadership distribution

---

## **STORY 19**
**Title:** Submit Teddy Talk to Leadership for Review

**Description:** Send completed Teddy Talk video to leadership for review and feedback.

**Value Add:** Ensures leadership awareness of team achievements, maintains communication cadence, and supports strategic alignment.

**Acceptance Criteria:**
- [ ] Video submitted by Thursday
- [ ] Appropriate distribution list used
- [ ] Submission includes context/summary
- [ ] Confirmation of receipt obtained
- [ ] Feedback tracking mechanism in place

---

## **STORY 20**
**Title:** Remove Two Master Collect Tasks from Daily Ephemeral Job Cluster

**Description:** Optimize daily ephemeral job cluster by removing two unnecessary master collect tasks that are impacting performance.

**Value Add:** Reduces processing time and DBU consumption, improves job cluster efficiency, and decreases operational costs.

**Acceptance Criteria:**
- [ ] Two master collect tasks identified
- [ ] Impact analysis completed
- [ ] Tasks safely removed from job cluster
- [ ] Performance improvements validated
- [ ] Documentation updated

---

## **STORY 21**
**Title:** UOBI-2173: Validate Latest Tables with Josh Williamson and WARM

**Description:** Set up and conduct meeting with Josh Williamson and WARM team to validate which tables should be used as authoritative sources. Add filing type dimensionality if WARM approves.

**Value Add:** Ensures data accuracy and consistency, reduces risk of using outdated tables, and adds valuable filing type dimension for enhanced analytics.

**Acceptance Criteria:**
- [ ] Meeting scheduled with Josh Williamson and WARM
- [ ] Latest authoritative tables identified and documented
- [ ] Filing type dimensionality requirements gathered
- [ ] WARM approval obtained for dimensionality addition
- [ ] Implementation plan created if approved

---

## **STORY 22**
**Title:** UOBI-2173: Validate CDO Lookup Table Lineage

**Description:** Investigate and validate the lineage of CDO lookup table which hasn't been updated in 9 months. Determine if updates are needed and document findings.

**Value Add:** Ensures data quality and reliability, identifies potential data staleness issues, and maintains integrity of downstream analytics.

**Acceptance Criteria:**
- [ ] Complete lineage analysis performed
- [ ] Update frequency requirements validated
- [ ] Root cause of 9-month gap identified
- [ ] Recommendations documented
- [ ] Update plan created if needed

---

## **STORY 23**
**Title:** Create Teddy Talk Video - Nate Lanfranca

**Description:** Nate Lanfranca to create and record separate Teddy Talk video for leadership review, complementing Jake's presentation.

**Value Add:** Provides federal lead perspective to leadership, strengthens team visibility, and demonstrates depth of expertise across team.

**Acceptance Criteria:**
- [ ] Video recorded by Nate Lanfranca
- [ ] Content aligns with team messaging
- [ ] Production quality standards met
- [ ] Video submitted for review
- [ ] Coordination with Jake's version completed

---

## **STORY 24**
**Title:** Setup NPD Statistical Process Controls Implementation Meeting

**Description:** Nate Lanfranca to organize kickoff meeting with Mike Gorman, Josh Williamson, and NPD team to initiate Statistical Process Controls implementation. Create business need report documenting problems SPC will solve.

**Value Add:** Enables data quality monitoring for NPD, establishes proactive issue detection, and aligns with industry best practices for statistical control.

**Acceptance Criteria:**
- [ ] Meeting scheduled with all stakeholders
- [ ] Business need report drafted
- [ ] Problem statements clearly defined
- [ ] SPC implementation scope documented
- [ ] Next steps and timeline established

---

## **STORY 25**
**Title:** Update Data Engineering Onboarding Documentation

**Description:** Jake to update comprehensive onboarding documentation in the Data Engineering Confluence space in preparation for incoming new hire.

**Value Add:** Reduces onboarding time for new team member, ensures consistent knowledge transfer, and maintains operational continuity.

**Acceptance Criteria:**
- [ ] All current processes documented
- [ ] Tool access procedures updated
- [ ] Training materials refreshed
- [ ] Confluence space organized and accessible
- [ ] Review completed with team lead

---

## **STORY 26**
**Title:** Document FY26 Priorities and Jira Label Strategy

**Description:** Jake to add FY26 priorities to Confluence and document how DE and DSP teams will align all work to D1 & OPQ FY26 priorities through strategic use of Jira labels.

**Value Add:** Ensures team alignment with organizational goals, enables priority-based reporting, and supports resource allocation decisions.

**Acceptance Criteria:**
- [ ] FY26 priorities documented in Confluence
- [ ] Jira label taxonomy created
- [ ] Alignment strategy documented
- [ ] Team training materials created
- [ ] Label implementation guide published

---

## **STORY 27**
**Title:** Create AI Presentation Part IV for MESH

**Description:** Jake to develop Part IV of the AI presentation series for upcoming MESH meeting, continuing the narrative from previous presentations.

**Value Add:** Maintains momentum on AI initiatives, educates stakeholders on AI capabilities, and supports AI adoption across the organization.

**Acceptance Criteria:**
- [ ] Presentation builds on Parts I-III
- [ ] Content relevant to MESH audience
- [ ] Slide deck professionally formatted
- [ ] Speaker notes included
- [ ] Review completed before MESH meeting

---

## **CLONE/MODIFY ITEMS**

### **CLONE 1: Issue 2175 - Continue Liquid Clustering Implementation**
**Description:** Clone issue 2175 to capture ongoing liquid clustering work. Continue implementing across all suitable jobs with Andre leading implementation.

**Value Add:** Already achieved DBU reduction from 1,000-1,003 to 919, continued implementation will further reduce costs and improve performance.

**Acceptance Criteria:**
- [ ] Issue 2175 successfully cloned
- [ ] All applicable jobs identified
- [ ] Implementation plan updated
- [ ] Future rollout to AA, E22, NPD teams planned

### **CLONE 2: Current Sprint Carryover Issues**
**Description:** Identify and clone all issues from current sprint that need to continue into next sprint.

**Value Add:** Maintains work continuity, prevents loss of progress, and ensures smooth sprint transition.

**Acceptance Criteria:**
- [ ] All carryover work identified
- [ ] Issues properly cloned
- [ ] Progress preserved in new tickets
- [ ] Sprint planning updated

### **MODIFY 1: Publish Mesh Confluence Draft**
**Description:** Complete and publish the Mesh-related Confluence draft that is currently saved.

**Value Add:** Provides documentation for mesh architecture, supports knowledge sharing, and enables team collaboration.

**Acceptance Criteria:**
- [ ] Draft content completed
- [ ] Review performed
- [ ] Document published in Confluence
- [ ] Stakeholders notified
- [ ] Due: Today
