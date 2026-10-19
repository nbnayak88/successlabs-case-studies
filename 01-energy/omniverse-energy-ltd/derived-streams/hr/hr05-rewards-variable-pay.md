# OVE-HR05 — Compensation and variable pay

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR05

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P08, OVE-P03. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Rhea Narayanan — Global Rewards Transformation Director.

### A — Understand (master 01–04)
**Mission:** **Reward sustainable energy performance while protecting safety, equity, compliance, and affordability.**
OmniEnergy uses inconsistent salary structures, local spreadsheets, scarce-skill premiums, site allowances, shift payments, sales incentives, and executive plans. Some incentives favor production volume without adequately reflecting safety, emissions, quality, customer outcomes, or long-term asset performance.

**Personas and proposed decision rights:**
- **OVE-HR05-P01 — Rhea Narayanan, Global Rewards Transformation Director:** Owns reward philosophy, architecture, fairness, controls, and value. Proposed domain design owner; sponsor approves funding.
- **OVE-HR05-P02 — Marco Silva, Downstream Business President:** Wants strong differentiation for high financial performance. Domain counterpart; validate authority during discovery.
- **OVE-HR05-P03 — Amina Yusuf, Pay Equity and Inclusion Lead:** Finds unexplained variation in engineering and trading roles. Domain counterpart; validate authority during discovery.
- **OVE-HR05-P04 — Kenji Mori, Refinery Employee Council Representative:** Requires understandable and negotiated frontline reward rules. Domain counterpart; validate authority during discovery.
- **OVE-HR05-P05 — Olivia Chen, Group Financial Controller:** Needs budget discipline, accrual accuracy, and audit evidence. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** How much should OmniEnergy standardize globally while preserving market differences, collective agreements, statutory requirements, mobility, offshore premiums, and critical-skill flexibility? Which outcomes should legitimately influence pay?

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR05-CAP01 capability group:** Reward policy; eligibility; merit planning; incentive calculation; equity review. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR05-VS01 value stream:** Budget → eligibility → recommendation → equity and safety review → approve → publish → reconcile. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** pay range; currency; eligible service segment; goal weight; achievement; payout; approval. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Compensation plans base-pay changes; Variable Pay calculates governed incentives; payroll calculates and pays net entitlements; finance owns accrual controls.

**Architecture decision OVE-HR05-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR05-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR05-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR05-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Safety gate:** Marco argues that financial targets justify full incentive payout.
- **Pay equity:** Amina identifies unexplained gender and location differences.
- **Local negotiation:** Kenji challenges the global frontline incentive formula.
- **Financial control:** Olivia finds inconsistent accruals and late executive exceptions.

**OVE-HR05-T01 test portfolio:** Safety breach despite margin target; employee transfers mid-period; reverse metric; FX change; over-budget exception; statement-to-payroll mismatch. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Rhea Narayanan — Global Rewards Transformation Director; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR05-KPI01:** Approved-to-paid reconciliation = matched approved award amounts / total approved award amounts; pair with unexplained pay differences and planning time. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR05-SRC → OVE-HR05-CAP01 → OVE-HR05-VS01 → OVE-HR05-REQ01/02 → OVE-HR05-ADR01 → OVE-HR05-EXP01 → OVE-HR05-T01 → OVE-HR05-KPI01. **OVE-HR05-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/819f9685247e4f8e87e4f6367d26426c); fetched revision 2026-09-03T20:09:17.154Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Rewards Case — Persona-Led Architecture Lab**  
	All characters and scenarios are fictional.

## Case Mission
> **Reward sustainable energy performance while protecting safety, equity, compliance, and affordability.**
OmniEnergy uses inconsistent salary structures, local spreadsheets, scarce-skill premiums, site allowances, shift payments, sales incentives, and executive plans. Some incentives favor production volume without adequately reflecting safety, emissions, quality, customer outcomes, or long-term asset performance.
## Fictional Lead Persona
### Rhea Narayanan — Global Rewards Transformation Director
Rhea must implement SAP SuccessFactors Compensation and Variable Pay across 42 countries. Her first test occurs when a refinery exceeds output and margin targets but records a serious safety breach and an emissions-control failure during the same performance period.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Rhea Narayanan
 | Global Rewards Transformation Director
 | Owns reward philosophy, architecture, fairness, controls, and value.

 | Marco Silva
 | Downstream Business President
 | Wants strong differentiation for high financial performance.

 | Amina Yusuf
 | Pay Equity and Inclusion Lead
 | Finds unexplained variation in engineering and trading roles.

 | Kenji Mori
 | Refinery Employee Council Representative
 | Requires understandable and negotiated frontline reward rules.

 | Olivia Chen
 | Group Financial Controller
 | Needs budget discipline, accrual accuracy, and audit evidence.

## Transformation Dilemma
How much should OmniEnergy standardize globally while preserving market differences, collective agreements, statutory requirements, mobility, offshore premiums, and critical-skill flexibility? Which outcomes should legitimately influence pay?
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Pay equity, transparency, safety and ethics gates, local compliance, auditability, and affordability.
- **Portfolio:** Base pay, merit, variable pay, allowances, retention, statements, equity, payroll, and analytics.
- **Program:** Harmonize job structures and pilot salaried and frontline populations.
### V2 — Value
- **Platform:** Compensation, Variable Pay, Performance, Employee Central, Payroll, Finance, and analytics.
- **Product:** Manager worksheet, employee statement, equity review, incentive scorecard, and reward dashboard.
- **Process:** Budget → Eligibility → Recommendation → Equity review → Approval → Statement → Payroll → Reconciliation.
### V3 — Victory
- **People:** Employees, managers, HR, Finance, employee councils, payroll, and reward committees.
- **Practice:** Guidelines, safety gates, equity analysis, exception governance, audit, and communication.
- **Project:** Pilot one refinery and one renewable professional population.
### V4 — Venture
Use rewards to support energy-transition skills, internal mobility, critical-role retention, sustainability, innovation, and new service models.
## Decision Scenes
- **Safety gate:** Marco argues that financial targets justify full incentive payout.
- **Pay equity:** Amina identifies unexplained gender and location differences.
- **Local negotiation:** Kenji challenges the global frontline incentive formula.
- **Financial control:** Olivia finds inconsistent accruals and late executive exceptions.
## 12-Stream Architecture Assignment
Connect reward strategy, employee and manager experience, planning and payout processes, job and pay data, Compensation applications, payroll and finance integration, security, analytics, AI controls, adoption, and value.
## Capstone Deliverables
1. Global reward philosophy
2. Country and workforce localization matrix
3. Job, grade, range, allowance, and eligibility architecture
4. Balanced incentive scorecards with safety and ESG gates
5. Pay-equity and exception-control model
6. Compensation-to-payroll and Finance integration map
7. Manager and employee communication journeys
8. Pilot and scale roadmap
9. Reward governance calendar
10. Affordability, fairness, retention, accuracy, and trust dashboard
## Victory Measures
- Reduced planning-cycle time
- Budget and accrual accuracy
- Fewer unexplained pay-equity differences
- Improved critical-skill retention
- Lower payroll adjustments
- Improved employee understanding and trust
## Assessment Checkpoint
Learners act as Rhea’s Reward Committee and must decide the refinery payout, resolve equity findings, defend global/local design choices, and prove payroll and financial control.
> 
	**Final Challenge:** How should Rhea reward high performance when financial success conflicts with safety, sustainability, and fairness?

