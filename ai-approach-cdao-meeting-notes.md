# AI Approach — CDAO Leadership Meeting Notes

**Office:** Chief Data & Analytics Office (CDAO), USCIS
**Date:** June 26, 2026
**Attendees:** Jake Stone, Joe Knarich, Lynn Wallace, Susan Love, Jake Hobbs
**Type:** Brainstorming / strategy working session

## Purpose

Continuing a running series of brainstorming sessions on the CDAO's approach to AI. This session focused on how to get the data environment ready for the new AI and cataloging tools, and on the governance, semantic-layer, and data-sharing groundwork needed before those tools arrive. Discussion built on the data-fabric diagram originally sketched on Lynn's whiteboard.

## Summary

The team is well-positioned on existing data quality and governance, but new tools (Databricks Genie, plus a catalog tool — Collibra 2.0 or Alation) are coming later this year, and CDAO will likely sit lower in the access queue than groups like FOD. The central idea is to build a comprehensive semantic layer / business glossary — with lineage back to source tables and columns — so AI tools (and analysts) operate with explicit context instead of guessing. The group connected this to the DHS data-fabric / Delta Share effort and the longer-term shift of eCISCOR into a true operational data source. The recurring theme throughout: governance is the gating dependency for almost everything, and CDAO needs a seat at the table before OIT turns tools on without it.

## 1. Readiness for new tools (gap analysis)

- New tooling arriving later this year: Databricks Genie, and a data catalog (Collibra 2.0 or Alation — selection pending).
- CDAO is well-positioned on existing data quality and governance structures, but there are gaps the new tools can fill.
- Realistic expectation that CDAO will be lower on the access priority list than other groups (e.g., FOD).
- Known data-quality issues in the lake; getting data ready is a prerequisite to using the tools well.
- The new catalog tools include capabilities that make ongoing data management more manageable.

## 2. Semantic layer & business glossary (core idea)

- Analogy (Susan): AI is like a sharp but socially awkward new analyst — it needs every term explicitly defined (what a form is, Form N-400 vs. another form, all synonyms and acronyms). Humans currently supply this context implicitly; the tools don't capture it yet.
- Alation and Collibra can explicitly store these definitions so they're machine-referenceable.
- Joe: "Use AI to train AI" — use AI to help build the semantic layer and improve data quality. Expose the semantic layer to business users through a glossary, with lineage back to the table/column implementation.
- Goal is *business literacy*, not just data literacy — encode not only data definitions but information (e.g., a derived field "age = current date − date of birth"), with lineage to the source fields.
- The picture is effectively four-dimensional: rules change over time, so the layer should let you trace what the rules were at any point in history.
- Directly supports the "classic admission problems": encode the INA, executive orders, and subsections so analysts don't rely on a memorized chart; capture historical policy changes (e.g., the 1986 and 1996 reforms that reclassified populations, including to LPR status).
- Practical near-term win (Lynn): even short of a full ontology, this helps prevent "bonkers" numbers reaching the press when someone queries GenAI faster than the team can produce an authoritative pull.

## 3. The "harness" + enterprise counting (Genie)

- Jake Hobbs has a presentation ready for next week on the "harness" concept. Analogy: a student arriving to class with vs. without a textbook — the harness is the textbook that gives Genie context.
- Genie space table limit is ~30 (not 20). The team doesn't want to consume that budget with catalog/definition tables pulled from the catalog tool.
- A well-built harness can be reused across projects, with custom versions for specific projects or areas.
- CDAO are the keepers of how USCIS counts (PAIR counts/calculations). The team wants an enterprise-level Genie space that is automatically inherited — so any Genie space is forced to use PAIR counting rules.
- Databricks reps "hand-waved" that this is possible (last week's presentation) but gave no concrete demo; the mechanism is inheritance-based (a hierarchy of "rooms").
- OIT has not yet thought about a super-level / enterprise group for things like information control — this is going on Kathy's talking points to the CIO. "This is why we need a seat at that table."

## 4. DHS data fabric, Delta Share & C3 / eCISCOR

- Open questions on how DHS HQ will govern the environment once it has control, and what rules/restrictions it will impose.
- DHS currently views Databricks as a federated tool (a Delta Share perspective), focused on specific datasets for emerging needs (e.g., HLR, administrative data, H-1B). DHS appears to be overlooking administrative control of individual data instances.
- Risk: a shared space must inherit USCIS counting rules, or DHS and USCIS will report different numbers.
- The data-fabric memo and this week's C3 decommissioning presentation add urgency. C3 has 57 interfaces (31 internal to USCIS).
- Long-term vision: shift from a network/point-to-point model to hub-and-spoke, with everyone publishing to and consuming from eCISCOR, turning it into a true operational data source (today it's an ODS in name only / really an analytical database).
- Selling point to OIT: the current internal-sharing model dates to 2008 and is now holding the agency back. A centralized hub enables data quality, governance, consistent external sharing and AI training, and standardized data products you can query in natural language.
- Ties to the data strategy as Objective 2.1 — "a single centralized source for USCIS data." It needs wording plain enough that the CIO recognizes it, and should be emphasized as the #1 objective with the longest tail. Estimated 3–5 year effort (analogous to C3 decommissioning).
- The new CIO is described as AI-driven and technically capable, and likely receptive. Contract politics are a factor.

## 5. Unstructured data

- Genie sits on structured data; USCIS holds large volumes of unstructured data (contracting, HR, policy) in disparate documents. The team is not convinced Genie is the right tool for massive unstructured data, and questions whether loading it all into the lake is the answer.
- Code Genie (the assistant alongside Databricks notebooks) is expected to speed up development work; its fit for unstructured-data cleanup is TBD.
- Concrete use case (Lynn): writing the 9th version of a PWS currently means opening and re-reading all prior PWSs. These documents live on desktops / in the cloud, not in a single repository and not in the lake (they aren't reporting data). Much free text isn't in the lake; scanned content sits in a separate store (possibly CPMS modules), which CDAO doesn't have access to — Scott and Todd could confirm.
- Cautionary note (Joe): a large amount of paper is unavailable to any electronic system. USCIS is still a paper-based agency; many applications arrive on paper (law offices print and mail because there's no API for them).

## 6. Tools landscape (OIT priorities)

- Latest from OIT: expansion of the M365 Copilot pilot; Genie remains further down OIT's list.
- Copilot is proving less reliable for code generation/review.
- Risk: OIT tends to release tools broadly to drive adoption. There's a better-than-60% chance tools get turned on before governance exists — the nightmare scenario is Genie being switched on with no notice.

## 7. Top risks (as discussed)

- **Misuse of operational migration data** — the highest risk; the kind of thing that lands on the front page for days. (Contract/administrative-data misuse won't make headlines.)
- **Cross-agency misinterpretation** — other DHS components misinterpreting/misusing USCIS data. Each agency understands its own imperfect data, but cross-agency interpretation invites disaster.
- **Loss of control once data crosses the boundary** (e.g., into Palantir) — ISAs/ICAs have hooks but are effectively unenforceable once data leaves USCIS. Delta Share / the fabric is one of the biggest risks: controls on what's exposed, plus "rules of the road" for permitted use.
- **Limited ability to refuse sharing** — the EO and a CIO policy memo leave little room to say no; the only real stick (shutting down Delta Share) would itself be a front-page story.
- **Inevitability of some misuse** — no governance fully prevents it. The aim is to minimize risk while keeping velocity high enough that people don't bypass governance.

## 8. CDAO strategy & governance approach

- Stay involved by pushing forward on the pieces OIT isn't yet thinking about; prioritize by risk (migration data first).
- Consider standing up a small, focused team to drive these angles.
- Approach OIT with a ready-made governance plan, framed as "yes, and" rather than "no" — "we know this is boring, we've done the work, let us do it." (Contrast: feedback from the MPD symposium that FOD heard "no.")
- CDAO has capacity available right now (between major projects — AOA zero-trust, tagging restart, address investigation) to help move these workstreams forward.
- Building a comprehensive semantic layer and establishing governance are valuable regardless of how the data-sharing and interface questions resolve — "having governance solves half our problems."

## Next steps

- Jake Hobbs to deliver the harness presentation next week.
- Lynn + Jake Hobbs to draft a risk-scenario matrix on Monday.
- Joe to annotate the data-fabric diagram (independent vs. dependent work; mind map) and to lay out data strategy Objective 2.1 for Kathy on Wednesday.
- Talking points prepped for Kathy's CIO meeting (week from Monday): integrated data & IT governance; Databricks apps governance; strategic AI implementation.
- Follow up with Databricks on enterprise-level Genie inheritance / counting.
- Continue zero-trust tagging; consider a pilot to expand tagging into broader governance/master-data tagging (gated on governance and steward buy-in).
- Identify bottlenecks; stand up governance with the right data stewards.
