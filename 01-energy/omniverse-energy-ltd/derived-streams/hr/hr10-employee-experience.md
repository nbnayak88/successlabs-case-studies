# OVE-HR10 — Digital employee experience

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR10

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P10. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Neha Varma — Digital Employee Experience Director.

### A — Understand (master 01–04)
**Mission:** **Create one inclusive digital front door for the rig, refinery, power plant, wind farm, retail station, field, and office.**
OmniEnergy employees navigate multiple portals, credentials, help channels, policy repositories, and mobile tools. Critical communications reach desk workers more reliably than shift and field populations, while common leave, payslip, schedule, learning, and support journeys create avoidable effort.

**Personas and proposed decision rights:**
- **OVE-HR10-P01 — Neha Varma, Digital Employee Experience Director:** Owns experience strategy, platform, accessibility, adoption, and value. Proposed domain design owner; sponsor approves funding.
- **OVE-HR10-P02 — Carlos Mendes, Refinery Shift Operator Persona:** Needs quick, accessible services during appropriate paid work time. Domain counterpart; validate authority during discovery.
- **OVE-HR10-P03 — Aisha Noor, Wind-Farm Technician Persona:** Needs reliable mobile and low-connectivity access. Domain counterpart; validate authority during discovery.
- **OVE-HR10-P04 — Laura Fischer, Global Communications Lead:** Needs targeted reach without notification overload. Domain counterpart; validate authority during discovery.
- **OVE-HR10-P05 — Ben Okafor, HR Service Delivery Owner:** Wants efficient self-service with human support for complex cases. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Should OmniEnergy organize the experience around systems, shared services, or employee journeys? Neha must create one coherent front door while supporting mobile, shift, offshore, multilingual, accessible, and low-connectivity contexts.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR10-CAP01 capability group:** Journey orchestration; accessible services; employee listening. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR10-VS01 value stream:** Need → discover service → authenticate → act → track → resolve → feedback. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** service case; journey; language; accessibility need; notification priority; feedback. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Experience front door orchestrates existing services; service owner resolves cases; safety channels remain authoritative for emergency instructions.

**Architecture decision OVE-HR10-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR10-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR10-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR10-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Frontline reach:** Carlos misses a safety-critical message.
- **Mobile friction:** Aisha cannot complete tasks with intermittent connectivity.
- **Notification overload:** Laura’s corporate campaigns compete with operational alerts.
- **Service inclusion:** Ben proposes automation for cases that require empathy and expertise.

**OVE-HR10-T01 test portfolio:** Low connectivity; inaccessible task; conflicting alerts; private device constraints; complex case needing human empathy. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Neha Varma — Digital Employee Experience Director; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR10-KPI01:** Task success = completed intended journeys / attempted journeys; segment frontline and office cohorts and record assisted success. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR10-SRC → OVE-HR10-CAP01 → OVE-HR10-VS01 → OVE-HR10-REQ01/02 → OVE-HR10-ADR01 → OVE-HR10-EXP01 → OVE-HR10-T01 → OVE-HR10-KPI01. **OVE-HR10-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/4478c40a55784c019fef4b2ed83b9a1d); fetched revision 2026-09-03T20:10:14.910Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Employee Experience Case — Persona-Led Architecture Lab**  
	All characters and events are fictional.

## Case Mission
> **Create one inclusive digital front door for the rig, refinery, power plant, wind farm, retail station, field, and office.**
OmniEnergy employees navigate multiple portals, credentials, help channels, policy repositories, and mobile tools. Critical communications reach desk workers more reliably than shift and field populations, while common leave, payslip, schedule, learning, and support journeys create avoidable effort.
## Fictional Lead Persona
### Neha Varma — Digital Employee Experience Director
Neha must pilot a role-aware employee experience platform for a refinery and a renewable field-service region. A safety communication reaches 96% of corporate employees but only 43% of shift workers; mobile users repeatedly abandon leave and payslip tasks.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Neha Varma
 | Digital Employee Experience Director
 | Owns experience strategy, platform, accessibility, adoption, and value.

 | Carlos Mendes
 | Refinery Shift Operator Persona
 | Needs quick, accessible services during appropriate paid work time.

 | Aisha Noor
 | Wind-Farm Technician Persona
 | Needs reliable mobile and low-connectivity access.

 | Laura Fischer
 | Global Communications Lead
 | Needs targeted reach without notification overload.

 | Ben Okafor
 | HR Service Delivery Owner
 | Wants efficient self-service with human support for complex cases.

## Transformation Dilemma
Should OmniEnergy organize the experience around systems, shared services, or employee journeys? Neha must create one coherent front door while supporting mobile, shift, offshore, multilingual, accessible, and low-connectivity contexts.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Frontline-first, mobile-first, accessible, multilingual, role-aware, secure, and human-supported.
- **Portfolio:** Communications, tasks, knowledge, search, HR service, time, pay, learning, safety, and listening.
- **Program:** Pilot high-volume journeys for refinery operators and field technicians.
### V2 — Value
- **Platform:** Work Zone or experience platform, SuccessFactors, identity, service management, knowledge, communications, and analytics.
- **Product:** Operator home, technician mobile hub, manager workspace, knowledge experience, and service journey.
- **Process:** Discover → Understand → Complete task → Track status → Receive support → Provide feedback.
### V3 — Victory
- **People:** Employees, managers, content owners, communications, service teams, accessibility experts, and champions.
- **Practice:** Content lifecycle, notification governance, search improvement, accessibility testing, journey analytics, and feedback closure.
- **Project:** Improve five priority journeys and prove equitable adoption.
### V4 — Venture
Evolve the digital front door into an intelligent workforce-experience and workplace-services ecosystem.
## Decision Scenes
- **Frontline reach:** Carlos misses a safety-critical message.
- **Mobile friction:** Aisha cannot complete tasks with intermittent connectivity.
- **Notification overload:** Laura’s corporate campaigns compete with operational alerts.
- **Service inclusion:** Ben proposes automation for cases that require empathy and expertise.
## 12-Stream Architecture Assignment
Connect experience strategy, personas, journeys, content and service processes, profile and interaction data, experience applications, identity and service integrations, security, analytics, AI search, change, and value.
## Capstone Deliverables
1. Workforce persona portfolio
2. Moments-that-matter journey maps
3. Digital-front-door information architecture
4. Priority task and service blueprints
5. Mobile, offline, multilingual, and accessibility standards
6. Content, search, notification, and ownership model
7. Identity and integration architecture
8. Assisted-service and escalation design
9. Champion-led rollout roadmap
10. Reach, completion, resolution, accessibility, adoption, and trust dashboard
## Victory Measures
- Increased active use across every persona
- Higher self-service completion and search success
- Faster request resolution
- Reduced routine inquiries
- Improved frontline communication reach
- Improved accessibility and employee trust
## Assessment Checkpoint
Learners act as Neha’s Employee Experience Design Studio. They must redesign the failed safety communication and mobile journeys while showing how equitable access, ownership, support, and continuous improvement will be sustained.
> 
	**Final Challenge:** How should Neha create one digital workforce experience that remains genuinely usable across radically different energy-work environments?

