# OVE-HR09 — Workforce intelligence

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR09

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P16, OVE-P03. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Dr. Ananya Bose — Chief Workforce Intelligence Officer.

### A — Understand (master 01–04)
**Mission:** **Turn trusted workforce data into explainable decisions and measurable action—not employee surveillance.**
OmniEnergy must connect workforce decisions to refinery reliability, offshore staffing, renewable expansion, customer operations, safety, succession, cost, and energy-transition skills. Today, HR reports are manually assembled, definitions vary, and planning relies on historical headcount rather than future capability demand.

**Personas and proposed decision rights:**
- **OVE-HR09-P01 — Dr. Ananya Bose, Chief Workforce Intelligence Officer:** Owns decision value, metric governance, privacy, adoption, and evidence. Proposed domain design owner; sponsor approves funding.
- **OVE-HR09-P02 — George Mwangi, Renewables Operations President:** Needs credible capacity and skill forecasts for a 5 GW growth plan. Domain counterpart; validate authority during discovery.
- **OVE-HR09-P03 — Emily Zhao, Workforce Data Product Manager:** Must reconcile inconsistent sources, definitions, and hierarchies. Domain counterpart; validate authority during discovery.
- **OVE-HR09-P04 — Mateo Ruiz, Employee Privacy Representative:** Opposes opaque prediction, hidden scoring, and surveillance. Domain counterpart; validate authority during discovery.
- **OVE-HR09-P05 — Sara Lindberg, Refinery Manager Persona:** Needs actionable decisions rather than complex dashboards. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Which decision products should OmniEnergy prioritize: capacity, skills, cost, safety, succession, recruiting, retention, or transition readiness? Ananya must maximize value without combining data in ways that damage employee trust.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR09-CAP01 capability group:** Metric governance; workforce forecasting; decision support. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR09-VS01 value stream:** Decision need → define metric → govern data → analyze → decide → evaluate. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** metric definition; as-of date; population; lineage; forecast horizon; cohort; decision log. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Analytics consumes governed data products; does not overwrite source employment facts; privacy controls restrict granular cross-domain joins.

**Architecture decision OVE-HR09-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR09-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR09-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR09-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Explainability:** The attrition model cannot justify individual risk scores.
- **Metric conflict:** Emily finds four definitions of headcount and three vacancy calculations.
- **Actionability:** Sara receives 60 metrics without thresholds, owners, or recommended actions.
- **Privacy:** Mateo challenges the combination of time, safety, performance, and employee-listening data.

**OVE-HR09-T01 test portfolio:** Four headcount definitions; tiny cohort disclosure; opaque attrition score; missing forecast assumptions; 5 GW scope conflict. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Dr. Ananya Bose — Chief Workforce Intelligence Officer; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR09-KPI01:** Metric consistency = reconciled published metric instances / metric instances tested; forecast error uses defined horizon and holdout data. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR09-SRC → OVE-HR09-CAP01 → OVE-HR09-VS01 → OVE-HR09-REQ01/02 → OVE-HR09-ADR01 → OVE-HR09-EXP01 → OVE-HR09-T01 → OVE-HR09-KPI01. **OVE-HR09-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/4ecbe054a901407ebf1106b6137e5e17); fetched revision 2026-09-03T20:10:14.970Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Workforce Intelligence Case — Persona-Led Architecture Lab**  
	All characters and scenarios are fictional.

## Case Mission
> **Turn trusted workforce data into explainable decisions and measurable action—not employee surveillance.**
OmniEnergy must connect workforce decisions to refinery reliability, offshore staffing, renewable expansion, customer operations, safety, succession, cost, and energy-transition skills. Today, HR reports are manually assembled, definitions vary, and planning relies on historical headcount rather than future capability demand.
## Fictional Lead Persona
### Dr. Ananya Bose — Chief Workforce Intelligence Officer
Ananya must build a governed workforce intelligence capability using SAP SuccessFactors People Analytics and SAP Analytics Cloud. Her first controversy arises when an attrition-risk model flags scarce engineers without providing a clear explanation, and business leaders request individual names.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Dr. Ananya Bose
 | Chief Workforce Intelligence Officer
 | Owns decision value, metric governance, privacy, adoption, and evidence.

 | George Mwangi
 | Renewables Operations President
 | Needs credible capacity and skill forecasts for a 5 GW growth plan.

 | Emily Zhao
 | Workforce Data Product Manager
 | Must reconcile inconsistent sources, definitions, and hierarchies.

 | Mateo Ruiz
 | Employee Privacy Representative
 | Opposes opaque prediction, hidden scoring, and surveillance.

 | Sara Lindberg
 | Refinery Manager Persona
 | Needs actionable decisions rather than complex dashboards.

## Transformation Dilemma
Which decision products should OmniEnergy prioritize: capacity, skills, cost, safety, succession, recruiting, retention, or transition readiness? Ananya must maximize value without combining data in ways that damage employee trust.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Decision-led analytics, transparent definitions, purpose limitation, minimum-necessary access, explainability, and human judgment.
- **Portfolio:** Workforce composition, skills, cost, capacity, succession, safety, mobility, retention, and scenario planning.
- **Program:** Deliver minimum viable decision products before advanced prediction.
### V2 — Value
- **Platform:** People Analytics, SAP Analytics Cloud, SuccessFactors, payroll, time, learning, Finance, HSE, and operational data.
- **Product:** Executive dashboard, manager decision workspace, skills heatmap, capacity scenario, and intervention register.
- **Process:** Define decision → Govern metric → Integrate data → Analyze → Intervene → Measure outcome → Learn.
### V3 — Victory
- **People:** Leaders, managers, HR, data owners, analysts, privacy representatives, and employees.
- **Practice:** Metric stewardship, data-quality review, model validation, access review, and quarterly workforce-value governance.
- **Project:** Pilot renewable-capacity and refinery-skill decision products.
### V4 — Venture
Scale workforce scenario planning, skills intelligence, evidence-based interventions, responsible prediction, and ecosystem labor-market insight.
## Decision Scenes
- **Explainability:** The attrition model cannot justify individual risk scores.
- **Metric conflict:** Emily finds four definitions of headcount and three vacancy calculations.
- **Actionability:** Sara receives 60 metrics without thresholds, owners, or recommended actions.
- **Privacy:** Mateo challenges the combination of time, safety, performance, and employee-listening data.
## 12-Stream Architecture Assignment
Connect workforce strategy, leader and manager journeys, planning and intervention processes, data and semantics, analytics applications, integrations, security, privacy, predictive assurance, change, and value realization.
## Capstone Deliverables
1. Workforce decision and persona inventory
2. Enterprise metric dictionary
3. Data lineage and ownership map
4. Minimum viable decision-product portfolio
5. Role-based security and privacy model
6. Skills and capacity scenario architecture
7. Responsible predictive-analytics controls
8. Intervention workflow and evidence register
9. Quarterly workforce-value review
10. Quality, adoption, forecast accuracy, intervention, and trust dashboard
## Victory Measures
- Reduced manual reporting and reconciliation
- Improved workforce-data quality
- Increased decision-product adoption
- Higher skill and succession coverage
- Improved forecast accuracy
- Documented value from workforce interventions
## Assessment Checkpoint
Learners act as Ananya’s Workforce Intelligence Product Council. They must decide whether to pause, aggregate, validate, or redesign the attrition model and demonstrate how every insight leads to a governed action and measurable outcome.
> 
	**Final Challenge:** How should Ananya create predictive workforce value without turning employees into unexplained risk scores?

