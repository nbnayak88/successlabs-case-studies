# OVE-HR01 — Workforce foundation

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR01

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P05. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Anika Sharma — Global Employee Central Transformation Director.

### A — Understand (master 01–04)
**Mission:** **Build one trusted workforce foundation for a safer, smarter, and more sustainable energy enterprise.**
OmniEnergy employs 68,000 people across upstream operations, refineries, power plants, LNG terminals, retail networks, renewable projects, and corporate functions in 42 countries. Fragmented worker, organization, position, and location data now threatens payroll accuracy, workforce planning, identity provisioning, contractor governance, and safety-critical access.

**Personas and proposed decision rights:**
- **OVE-HR01-P01 — Anika Sharma, Global EC Transformation Director:** Accountable for architecture, adoption, value, and global/local decisions. Proposed domain design owner; sponsor approves funding.
- **OVE-HR01-P02 — Michael Torres, Texas Refinery Director:** Needs accurate positions, certifications, and access without production disruption. Domain counterpart; validate authority during discovery.
- **OVE-HR01-P03 — Farah Al-Mansoori, Middle East HR Country Lead:** Protects localization, labor, nationalization, and data-residency requirements. Domain counterpart; validate authority during discovery.
- **OVE-HR01-P04 — Samuel Okoro, Identity and OT Security Lead:** Requires rapid provisioning and deprovisioning across IT and operational sites. Domain counterpart; validate authority during discovery.
- **OVE-HR01-P05 — Mei Wong, Global Payroll Control Head:** Will approve migration only after employee and job data reconcile. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** The Executive Workforce Council must choose among three approaches:
1. Deploy one rapid global template.
2. Migrate business units independently.
3. Establish a federated global core with governed local extensions.
Anika must recommend the operating model, data ownership, foundation-object design, position architecture, release sequence, controls, and evidence required to proceed.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR01-CAP01 capability group:** Person and employment stewardship; organization governance; position control. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR01-VS01 value stream:** Hire → validate → assign → authorize → maintain → retire. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** person ID; employment ID; effective date; legal entity; position; event reason. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** EC owns approved employment facts; learning owns competence evidence; IAM owns accounts; site safety owns restricted-work authorization.

**Architecture decision OVE-HR01-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR01-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR01-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR01-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Global/local conflict:** Farah requests 31 local fields and nine approval variants. Classify mandatory, configurable, and obsolete requirements.
- **Data-quality crisis:** Mei identifies duplicate employments and missing effective dates two weeks before cutover.
- **Safety access risk:** Michael discovers positions without required certification profiles.
- **Termination failure:** Samuel finds that a terminated contractor still has refinery access.

**OVE-HR01-T01 test portfolio:** Rehire with an existing person ID; concurrent employment; backdated transfer; terminated contractor; duplicate source records. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Anika Sharma — Global Employee Central Transformation Director; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR01-KPI01:** Critical-record completeness = complete critical records / in-scope records; owner: Anika; baseline to establish. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR01-SRC → OVE-HR01-CAP01 → OVE-HR01-VS01 → OVE-HR01-REQ01/02 → OVE-HR01-ADR01 → OVE-HR01-EXP01 → OVE-HR01-T01 → OVE-HR01-KPI01. **OVE-HR01-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/358d96630bf44787b59ec0b1b389eb46); fetched revision 2026-09-10T07:36:21.714Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Workforce Transformation Case — Persona-Led Architecture Lab**  
	All organizations, characters, events, figures, and decisions in this learning case are fictional.

## Case Mission
> **Build one trusted workforce foundation for a safer, smarter, and more sustainable energy enterprise.**
OmniEnergy employs 68,000 people across upstream operations, refineries, power plants, LNG terminals, retail networks, renewable projects, and corporate functions in 42 countries. Fragmented worker, organization, position, and location data now threatens payroll accuracy, workforce planning, identity provisioning, contractor governance, and safety-critical access.
## Fictional Lead Persona
### Anika Sharma — Global Employee Central Transformation Director
Anika has 18 months to establish SAP SuccessFactors Employee Central as OmniEnergy’s governed workforce system of record. She must balance a global data model with country law, joint-venture requirements, union agreements, offshore rotations, refinery safety, and renewable-project growth.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Anika Sharma
 | Global EC Transformation Director
 | Accountable for architecture, adoption, value, and global/local decisions.

 | Michael Torres
 | Texas Refinery Director
 | Needs accurate positions, certifications, and access without production disruption.

 | Farah Al-Mansoori
 | Middle East HR Country Lead
 | Protects localization, labor, nationalization, and data-residency requirements.

 | Samuel Okoro
 | Identity and OT Security Lead
 | Requires rapid provisioning and deprovisioning across IT and operational sites.

 | Mei Wong
 | Global Payroll Control Head
 | Will approve migration only after employee and job data reconcile.

## Transformation Dilemma
The Executive Workforce Council must choose among three approaches:
1. Deploy one rapid global template.
2. Migrate business units independently.
3. Establish a federated global core with governed local extensions.
Anika must recommend the operating model, data ownership, foundation-object design, position architecture, release sequence, controls, and evidence required to proceed.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Global core/local compliance, effective dating, minimum necessary data, human accountability, and safety by design.
- **Portfolio:** Foundation objects, employee data, position management, workflows, security, integrations, migration, and analytics.
- **Program:** Design authority, country waves, data remediation, testing, adoption, and value governance.
### V2 — Value
- **Platform:** Employee Central, Position Management, SAP BTP, Integration Suite, identity, payroll, and analytics.
- **Product:** Employee record, organization model, manager workspace, position control, and workforce-data products.
- **Process:** Hire, rehire, transfer, promotion, global assignment, leave, restructuring, and termination.
### V3 — Victory
- **People:** HR product teams, data owners, country leads, managers, payroll, security, safety, and worker representatives.
- **Practice:** Data-quality gates, design standards, release controls, reconciliation, audit, and value reviews.
- **Project:** Pilot India renewables, Texas refining, and one corporate population before regional scale.
### V4 — Venture
Use the trusted workforce core to enable skills intelligence, talent mobility, workforce planning, AI-supported services, contractor ecosystems, and energy-transition capability building.
## 12-Stream Architecture Assignment
Learners must connect:
1. Business outcomes and workforce capabilities
2. Hire-to-retire processes
3. Employee and manager experience
4. Person, employment, job, position, and organization data
5. Employee Central application design
6. Payroll, identity, safety, learning, and finance integration
7. Cloud and environment strategy
8. Role-based permissions, privacy, and audit
9. Workforce analytics and data quality
10. Responsible automation and AI
11. Change, consultation, and adoption
12. Benefits, KPIs, and value realization
## Decision Scenes
- **Global/local conflict:** Farah requests 31 local fields and nine approval variants. Classify mandatory, configurable, and obsolete requirements.
- **Data-quality crisis:** Mei identifies duplicate employments and missing effective dates two weeks before cutover.
- **Safety access risk:** Michael discovers positions without required certification profiles.
- **Termination failure:** Samuel finds that a terminated contractor still has refinery access.
## Capstone Deliverables
1. Executive Workforce Core Brief
2. Corporate and succession data models
3. Legal Entity → Business Unit → Division → Department → Location design
4. Position hierarchy and job architecture
5. Global/local decision matrix
6. Hire-to-retire process and event map
7. RBP, privacy, payroll, and safety-control matrix
8. Migration, cutover, fallback, and hypercare plan
9. Adoption and stakeholder strategy
10. Victory dashboard and evidence register
## Victory Measures
- 98% critical workforce-record completeness
- 95% governed-position coverage
- 90% automated downstream provisioning
- 50% reduction in lifecycle-processing time
- Zero material payroll or safety-access failures at cutover
- Sustained manager adoption and employee-data trust
## 18-Month Roadmap
1. **Discover:** inventory systems, objects, interfaces, controls, and country requirements.
2. **Design:** approve the global model, variants, workflows, RBP, and integration standards.
3. **Build:** configure, cleanse, migrate, integrate, and test.
4. **Pilot:** release to representative energy populations with command-center support.
5. **Scale:** deploy by risk-based country and business waves.
6. **Optimize:** add skills, planning, automation, and continuous data-quality management.
## Assessment Checkpoint
A strong solution treats Employee Central as an enterprise workforce-control system—not merely an HR database. Learners must defend Anika’s recommendation before a simulated Global Design Authority and show the impact of every major decision on workers, managers, payroll, safety, identity, compliance, and business value.
> 
	**Final Challenge:** How should Anika create one trusted workforce foundation without disrupting pay, access, energy operations, local compliance, or employee trust?

