# OVE-HR07 — Payroll

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR07

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P03. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Meera Iyer — Global Payroll Transformation Executive.

### A — Understand (master 01–04)
**Mission:** **Modernize global payroll without gambling with employee pay, legal compliance, or energy operations.**
OmniEnergy payroll must process offshore rotations, refinery shifts, overtime, hazard premiums, mobility, expatriate allowances, sales incentives, union rules, and country statutory obligations for 68,000 employees. Fragmented engines and manual interfaces create control and employee-trust risks.

**Personas and proposed decision rights:**
- **OVE-HR07-P01 — Meera Iyer, Global Payroll Transformation Executive:** Owns accuracy, strategy, controls, migration, and employee trust. Proposed domain design owner; sponsor approves funding.
- **OVE-HR07-P02 — Hans Becker, Germany Payroll Lead:** Protects statutory and works-council requirements. Domain counterpart; validate authority during discovery.
- **OVE-HR07-P03 — Luciana Costa, Refinery Employee Persona:** Needs understandable, accurate, and timely pay. Domain counterpart; validate authority during discovery.
- **OVE-HR07-P04 — Robert Li, Group Financial Controller:** Requires reconciled postings, liabilities, and evidence. Domain counterpart; validate authority during discovery.
- **OVE-HR07-P05 — Ngozi Adeyemi, Payroll Technology and Security Lead:** Owns interfaces, segregation of duties, recovery, and monitoring. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Should OmniEnergy create one global payroll platform, regional hubs, or a hybrid model? Meera must protect local compliance while reducing fragmentation and maintaining uninterrupted pay.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR07-CAP01 capability group:** Gross-to-net governance; payroll controls; reconciliation; continuity. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR07-VS01 value stream:** Approved inputs → validate → calculate → resolve → authorize → pay → post → reconcile. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** pay period; wage type; retro period; deduction; bank instruction; posting; control total. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Payroll owns gross-to-net and statutory calculation; EC owns employment inputs; treasury authorizes disbursement; finance accepts balanced postings.

**Architecture decision OVE-HR07-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR07-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR07-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR07-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Pay incident:** Luciana receives an unexplained deduction.
- **Localization conflict:** Hans rejects parts of the global template.
- **Finance mismatch:** Robert finds payroll-to-ledger differences.
- **Continuity test:** Ngozi simulates an unavailable interface before cutoff.

**OVE-HR07-T01 test portfolio:** Unexplained deduction; legitimate retroactive change; failed pre-cutoff feed; duplicate bank instruction; ledger mismatch. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Meera Iyer — Global Payroll Transformation Executive; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR07-KPI01:** On-time correct pay = employees paid correct authorized amount by due date / employees due; classify corrections by cause, not a zero-retro target. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR07-SRC → OVE-HR07-CAP01 → OVE-HR07-VS01 → OVE-HR07-REQ01/02 → OVE-HR07-ADR01 → OVE-HR07-EXP01 → OVE-HR07-T01 → OVE-HR07-KPI01. **OVE-HR07-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/0414bddb302b4ac1bda81984212bf533); fetched revision 2026-09-03T20:09:17.138Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Payroll Case — Persona-Led Architecture Lab**  
	All characters and events are fictional.

## Case Mission
> **Modernize global payroll without gambling with employee pay, legal compliance, or energy operations.**
OmniEnergy payroll must process offshore rotations, refinery shifts, overtime, hazard premiums, mobility, expatriate allowances, sales incentives, union rules, and country statutory obligations for 68,000 employees. Fragmented engines and manual interfaces create control and employee-trust risks.
## Fictional Lead Persona
### Meera Iyer — Global Payroll Transformation Executive
Meera must recommend a global, regional, or governed hybrid payroll model using SAP SuccessFactors Employee Central Payroll. Three days before pay date, a retroactive time-rule change creates unexpected deductions for employees at two refineries.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Meera Iyer
 | Global Payroll Transformation Executive
 | Owns accuracy, strategy, controls, migration, and employee trust.

 | Hans Becker
 | Germany Payroll Lead
 | Protects statutory and works-council requirements.

 | Luciana Costa
 | Refinery Employee Persona
 | Needs understandable, accurate, and timely pay.

 | Robert Li
 | Group Financial Controller
 | Requires reconciled postings, liabilities, and evidence.

 | Ngozi Adeyemi
 | Payroll Technology and Security Lead
 | Owns interfaces, segregation of duties, recovery, and monitoring.

## Transformation Dilemma
Should OmniEnergy create one global payroll platform, regional hubs, or a hybrid model? Meera must protect local compliance while reducing fragmentation and maintaining uninterrupted pay.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Accurate and timely pay, local compliance, segregation of duties, reconciliation, transparency, and tested recovery.
- **Portfolio:** Master data, time, calculation, controls, banking, statutory reporting, Finance, payslips, and cases.
- **Program:** Risk-based country waves with parallel runs and executive go/no-go gates.
### V2 — Value
- **Platform:** Employee Central Payroll, Employee Central, Time, Compensation, Finance, banking, and analytics.
- **Product:** Country payroll, control dashboard, employee payslip, reconciliation report, and inquiry journey.
- **Process:** Inputs → Validate → Calculate → Review → Approve → Pay → Post → Report → Reconcile.
### V3 — Victory
- **People:** Payroll specialists, employees, managers, Finance, HR, vendors, security, and country authorities.
- **Practice:** Pre-payroll controls, issue ownership, reconciliation, testing, release, incident, and hypercare governance.
- **Project:** Complete parallel runs and sustain stable cycles before scale.
### V4 — Venture
Create reusable country patterns, continuous payroll controls, global insight, intelligent exception handling, and financial-wellbeing services.
## Decision Scenes
- **Pay incident:** Luciana receives an unexplained deduction.
- **Localization conflict:** Hans rejects parts of the global template.
- **Finance mismatch:** Robert finds payroll-to-ledger differences.
- **Continuity test:** Ngozi simulates an unavailable interface before cutoff.
## 12-Stream Architecture Assignment
Connect payroll strategy, employee journeys, calculation and control processes, master and result data, payroll applications, time/Finance/banking integrations, technology, security, analytics, AI-supported exceptions, change, and value.
## Capstone Deliverables
1. Payroll operating-model recommendation
2. Country complexity and wave assessment
3. End-to-end payroll process and control architecture
4. Master, time, compensation, and result-data design
5. Integration, reconciliation, and segregation-of-duties matrix
6. Parallel-run and acceptance criteria
7. Cutover, fallback, recovery, and hypercare plan
8. Employee communication and inquiry journey
9. Incident response and corrective-action report
10. Accuracy, timeliness, compliance, effort, and trust dashboard
## Victory Measures
- Sustained on-time and accurate payroll
- Lower errors, off-cycle payments, and inquiries
- Reduced manual reconciliation
- Complete statutory and audit evidence
- Tested business continuity
- Improved employee confidence
## Assessment Checkpoint
Learners act as Meera’s Global Payroll Control Council. They must resolve the deduction incident and defend the operating model, migration sequence, controls, employee communication, and recovery readiness.
> 
	**Final Challenge:** What evidence should Meera require before declaring a payroll country ready for migration and scale?

