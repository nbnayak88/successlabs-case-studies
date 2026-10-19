# OVE-HR08 — Time and absence

[HR studio](README.md) · [Enterprise master](../../master/README.md)

## Canonical HR expansion — OVE-HR08

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P04. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Vikram Deshpande — Global Workforce Time Product Director.

### A — Understand (master 01–04)
**Mission:** **Build accurate, fair, privacy-aware, and safety-led workforce time operations.**
OmniEnergy must manage offshore rotations, refinery shifts, control-room coverage, maintenance call-outs, field travel, retail schedules, project time, overtime, premiums, leave, and fatigue limits. Paper, terminals, spreadsheets, and local systems create payroll and compliance risk.

**Personas and proposed decision rights:**
- **OVE-HR08-P01 — Vikram Deshpande, Global Workforce Time Product Director:** Owns policy, architecture, integration, adoption, and value. Proposed domain design owner; sponsor approves funding.
- **OVE-HR08-P02 — Monika Reed, Shutdown Maintenance Supervisor:** Needs staffing flexibility during critical work. Domain counterpart; validate authority during discovery.
- **OVE-HR08-P03 — Idris Bello, Maintenance Technician Persona:** Needs correct premiums, rest protection, and transparent corrections. Domain counterpart; validate authority during discovery.
- **OVE-HR08-P04 — Claire Martin, Labor Relations and Privacy Counsel:** Challenges excessive tracking and unlawful overrides. Domain counterpart; validate authority during discovery.
- **OVE-HR08-P05 — Akira Tan, Payroll Integration Lead:** Requires approved, complete, and reconciled time inputs. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Should OmniEnergy enforce one global time model or create governed variants by workforce pattern and country? Vikram must balance accuracy, operational flexibility, safety, privacy, collective agreements, and payroll deadlines.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR08-CAP01 capability group:** Time capture; absence entitlement; premium valuation; fatigue exception control. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR08-VS01 value stream:** Schedule → capture → validate → assess fatigue → approve → value → reconcile. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** time event; time zone; shift; overtime; rest interval; absence; premium; approval. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Time records approved hours and absence; scheduling allocates crews; operations owns staffing; payroll values/payments follow approved rules.

**Architecture decision OVE-HR08-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR08-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR08-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR08-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Fatigue risk:** Monika requests an override after repeated excessive hours.
- **Privacy challenge:** Claire questions location tracking for field workers.
- **Pay dispute:** Idris reports missing call-out and hazard premiums.
- **Payroll cutoff:** Akira finds late, duplicate, and unapproved records.

**OVE-HR08-T01 test portfolio:** Cross-midnight shift; daylight-saving boundary; repeated excessive hours; duplicate terminal event; missing call-out premium; late approval. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Vikram Deshpande — Global Workforce Time Product Director; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR08-KPI01:** Approved-time reconciliation = accepted approved time records / submitted approved records; pair with fatigue exceptions and pay disputes. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR08-SRC → OVE-HR08-CAP01 → OVE-HR08-VS01 → OVE-HR08-REQ01/02 → OVE-HR08-ADR01 → OVE-HR08-EXP01 → OVE-HR08-T01 → OVE-HR08-KPI01. **OVE-HR08-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/c556c0e3eb984141b0048e15fd290830); fetched revision 2026-09-03T20:09:17.030Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Time and Operations Case — Persona-Led Architecture Lab**  
	All characters and events are fictional.

## Case Mission
> **Build accurate, fair, privacy-aware, and safety-led workforce time operations.**
OmniEnergy must manage offshore rotations, refinery shifts, control-room coverage, maintenance call-outs, field travel, retail schedules, project time, overtime, premiums, leave, and fatigue limits. Paper, terminals, spreadsheets, and local systems create payroll and compliance risk.
## Fictional Lead Persona
### Vikram Deshpande — Global Workforce Time Product Director
Vikram must pilot SAP SuccessFactors Time Tracking and Time Off for a refinery and an offshore maintenance population. During a shutdown, repeated excessive-hour alerts appear, but production leaders request overrides to maintain output.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Vikram Deshpande
 | Global Workforce Time Product Director
 | Owns policy, architecture, integration, adoption, and value.

 | Monika Reed
 | Shutdown Maintenance Supervisor
 | Needs staffing flexibility during critical work.

 | Idris Bello
 | Maintenance Technician Persona
 | Needs correct premiums, rest protection, and transparent corrections.

 | Claire Martin
 | Labor Relations and Privacy Counsel
 | Challenges excessive tracking and unlawful overrides.

 | Akira Tan
 | Payroll Integration Lead
 | Requires approved, complete, and reconciled time inputs.

## Transformation Dilemma
Should OmniEnergy enforce one global time model or create governed variants by workforce pattern and country? Vikram must balance accuracy, operational flexibility, safety, privacy, collective agreements, and payroll deadlines.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Least-intrusive capture, lawful rules, rest protection, transparent correction, and global governance.
- **Portfolio:** Schedules, clocking, travel, standby, overtime, premiums, absence, approvals, and analytics.
- **Program:** Pilot refinery and offshore populations before broader workforce patterns.
### V2 — Value
- **Platform:** Time Tracking, Time Off, Employee Central, scheduling, payroll, devices, and analytics.
- **Product:** Worker timesheet, manager exception workspace, rule catalog, and labor-capacity dashboard.
- **Process:** Schedule → Capture → Validate → Approve → Correct → Payroll → Cost → Analyze.
### V3 — Victory
- **People:** Workers, supervisors, payroll, labor relations, HSE, HR, and operations planners.
- **Practice:** Rule governance, exception ownership, correction audit, fatigue review, and payroll reconciliation.
- **Project:** Run plant and offshore pilots through multiple payroll cycles.
### V4 — Venture
Use trusted time data for capacity planning, fatigue prevention, project costing, workforce scheduling, and service optimization.
## Decision Scenes
- **Fatigue risk:** Monika requests an override after repeated excessive hours.
- **Privacy challenge:** Claire questions location tracking for field workers.
- **Pay dispute:** Idris reports missing call-out and hazard premiums.
- **Payroll cutoff:** Akira finds late, duplicate, and unapproved records.
## 12-Stream Architecture Assignment
Connect workforce strategy, worker journeys, time processes, schedule and attendance data, Time applications, device/payroll integrations, technology, security, privacy, analytics, AI-supported exceptions, change, and value.
## Capstone Deliverables
1. Workforce-pattern and rule inventory
2. Global standard and localization matrix
3. Worker and manager journey maps
4. Schedule, clocking, overtime, premium, and absence architecture
5. Device, location, biometric, and privacy assessment
6. Fatigue and working-time control model
7. Correction, audit, and dispute process
8. Payroll and scheduling integration blueprint
9. Pilot and scale roadmap
10. Accuracy, safety, compliance, utilization, and trust dashboard
## Victory Measures
- Improved time and payroll-input accuracy
- Lower missed-punch and correction rates
- Reduced reconciliation effort
- Improved rest and working-time compliance
- Better labor utilization
- No increase in fatigue or privacy risk
## Assessment Checkpoint
Learners act as Vikram’s Workforce Time Architecture Team. They must resolve the shutdown conflict while defending lawful, explainable variants for offshore, refinery, field, retail, and corporate populations.
> 
	**Final Challenge:** How should Vikram protect workers and payroll accuracy while preserving the flexibility required for critical energy operations?

