Slide 1 – Priority Projects Progress: Databricks & NPD (table)

“On this slide I’ll start with four of our biggest data‑engineering accomplishments for the quarter.

First, Databricks Efficiency & Cost Analytics.
We now have agency‑grade DBU and cost analysis tables running as daily jobs, reconciled with platform reporting. On top of that, we built usage dashboards with KPIs, time series, and failure plots, and stood up a governed table‑cleanup framework with an auditable log. That means we can finally see where Databricks dollars are going, where jobs are under‑performing, and we have safe, repeatable controls to reduce storage and run‑time cost.

Second, Division‑wide Databricks Permissions Audit.
We created a new pipeline that ties Databricks job permissions to HR data so we can automatically identify inactive accounts. We produced inventories of AA and NPD workspaces and schemas, and built job‑to‑user and job‑to‑group mappings. This is the backbone for a standard, role‑based access model and is already driving cleanup of obsolete accounts and reduced audit risk.

Third, NPD & Director’s Dashboards – Data Integrity & Sharing.
We replicated the core NPD pending, completions, and historical pending tables into a governed public schema so partners can self‑serve using the same authoritative metrics the Director sees. We also fixed key logic issues—such as future‑dated approvals and mis‑alignment of I‑589 and EOIR business rules—so the Director’s dashboards now better match program expectations and are easier to defend in high‑visibility settings.

Finally, Decommissioning High‑Cost Legacy Pipelines for OAW.
Working with PAER, we resolved discrepancies between OAW datasets and stakeholder spreadsheets, confirmed the authoritative source, and then, per leadership direction, redirected BI reporting to the PAER OAW dashboard. That allowed us to safely shut down the OAW Databricks production jobs and document the resource savings—retiring one of our most expensive job suites while preserving mission reporting.”

Slide 2 – Priority Projects Progress: Lineage & DSP Dashboards

“Here we focus on observability and front‑end value.

For Databricks Lineage & Observability, we implemented a recurring lineage capture process. We defined a Delta table with partitions and retention, built an extraction and transform pipeline that captures key job metadata—names, IDs, owners, schedule—and wired it to a monthly Databricks job with retries, timeouts, and failure notifications. We validated sample runs to ensure records are written correctly, so we now have a consistent, queryable lineage dataset to support audits, impact analysis, and future dashboards.

On the DSP BI Data Visualization side, we delivered several high‑value dashboards:

The OAW HiVUE dashboard connects directly to the cdo_oaw table. It lets users explore A‑Number lists with familiar filters and export to Excel, which has significantly reduced one‑off data pulls.
We continued building the Dashboard of Dashboards for Tableau usage, which will provide KPIs like session duration, filter usage, and tab navigation. That will give us a clear picture of which BI products are most used, and where to focus improvements.
And we began development of the SNOW dashboard, which will combine high‑level ServiceNow metrics with detailed intake‑and‑resolution views, helping the program identify bottlenecks in the ticket pipeline and improve service.
We also replicated the lineage work for the DECP portfolio, so both the broader BI organization and our own program now share a common lineage standard and code base.”

Slide 3 – Priority Projects Progress: DECP Monitoring & Optimization Dashboards

“This slide highlights how we’re turning that data into operational insight.

First, the Databricks DBU & Cost Summary Dashboard.
This dashboard shows how much Databricks compute power we’re using over time, broken down by job type. It turns complex usage logs into simple visuals leaders can understand—supporting budget discussions and helping us prioritize optimization work. Today it shows about 22.5 million DBUs of total agency usage over the last year, including 13.5 million DBUs from scheduled jobs, around 5.8 thousand jobs run with an average duration of about 67 minutes, and another 9 million DBUs / 2.3 thousand runs from interactive and legacy “other” workloads.

Second, the Schema Cleanup Dashboard.
This tracks the impact of our table‑cleanup efforts: how many files we’ve consolidated, how much storage we’ve reclaimed, how many files have been vacuumed, and how many unused tables have been dropped. It also surfaces current file counts, data volume, and row counts across key schemas. To date, we’ve optimized 10,917 files, achieved about 491 MB of table‑size reductions across the top tables, vacuumed 1,951 files, and dropped 16 unused tables. Current snapshots show roughly 30,000 files, 2.56 TB of data, and 20.3 billion rows across the monitored schemas—giving us a clear baseline and proof of progress.

Lastly, the Backend Dataset Curation Program Job Metrics Dashboard.
This monitors the health of our production jobs: failure rates, run times, DBU consumption, and how frequently each pipeline runs. Over the last 90 days we’re seeing weekly job and task success rates near 100%, with only small percentages of failed or cancelled runs. Frequency plots show our busiest pipelines running about 30 to 38 times per month, and heatmaps highlight which specific jobs consume the most run time and DBUs. This lets us spot instability early, protect downstream dashboards, and target our engineering time where it has the greatest impact.”

Slide 4 – Priority Projects Progress: Dashboard Views (screenshots)

“To close out this section, this slide gives you a visual snapshot of those dashboards in action.

On the upper left you see the Task and Job Failure plots—almost entirely green—illustrating the very high success rates I just mentioned. Below that is the DBU Utilization summary, which shows total DBUs, how much is coming from scheduled versus interactive work, and the average job durations.

On the right side, at the top, is the Schema Cleanup dashboard, highlighting the number of files optimized, size reductions in megabytes, and the count of vacuumed files and dropped tables. At the bottom right are the heatmaps from the Job Metrics dashboard, which quickly show which jobs are the heaviest consumers of time and compute.

Taken together, these views demonstrate how far we’ve come in one quarter: we now have transparent, data‑driven visibility into Databricks usage, cost, reliability, and data hygiene across the BI program—and we’re already using these insights to decommission expensive workloads and improve service to our customers.”
