# OVE-HR02b — Workforce readiness and onboarding

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR02b

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P04, OVE-P13. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Priya Menon — Global Energy Workforce Readiness Director.

### A — Understand (master 01–04)
**Mission:** **Transform onboarding into a governed workforce-readiness system for energy operations.**
At OmniEnergy, a new worker may need payroll registration, medical fitness clearance, offshore credentials, PPE, site induction, devices, identity, travel, accommodation, safety learning, export-control approval, and physical access before productive work begins. Document completion alone does not equal readiness.

**Personas and proposed decision rights:**
- **OVE-HR02b-P01 — Priya Menon, Global Workforce Readiness Director:** Owns the accepted-offer-to-90-day experience and readiness outcome. Proposed domain design owner; sponsor approves funding.
- **OVE-HR02b-P02 — Thomas Reid, Offshore Installation Manager:** Cannot mobilize workers without verified safety and travel prerequisites. Domain counterpart; validate authority during discovery.
- **OVE-HR02b-P03 — Leila Hassan, New Hire Persona — Process Engineer:** Needs clear tasks, equipment, access, mentoring, and role expectations. Domain counterpart; validate authority during discovery.
- **OVE-HR02b-P04 — Grace Liu, Identity and Equipment Service Owner:** Needs complete data and timely events for provisioning. Domain counterpart; validate authority during discovery.
- **OVE-HR02b-P05 — Rafael Pinto, HSE Assurance Director:** Requires auditable proof before restricted work authorization. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Should onboarding remain an HR process, be owned by individual sites, or become a cross-functional workforce-readiness product? Priya must create one coherent experience while supporting employees, contractors, transfers, rehires, graduates, and mobile workers.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR02b-CAP01 capability group:** Readiness orchestration; induction assurance; early-tenure support. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR02b-VS01 value stream:** Accepted offer → prepare → verify readiness → supervised work → assess → integrate. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** readiness case; task dependency; credential expiry; equipment; badge; manager sign-off. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Onboarding coordinates tasks; IAM provisions authorized access; HSE verifies competence; HR readiness never substitutes for permit-to-work authority.

**Architecture decision OVE-HR02b-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR02b-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR02b-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR02b-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Day-one failure:** Eighteen refinery operators lack verified induction, eleven badges are inactive, and six payroll records are incomplete.
- **Offshore mobilization:** Thomas must fill a rotation, but two workers lack current credentials.
- **Journey overload:** Leila receives 37 unsequenced tasks from seven functions.
- **Early attrition:** New engineers report weak mentoring and unclear first-90-day expectations.

**OVE-HR02b-T01 test portfolio:** Expired offshore credential; 37 unsequenced tasks; inactive badge; missing payroll record; postponed start date. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Priya Menon — Global Energy Workforce Readiness Director; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR02b-KPI01:** Day-one readiness = starters with every applicable prerequisite verified / starters; report productivity separately by role. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR02b-SRC → OVE-HR02b-CAP01 → OVE-HR02b-VS01 → OVE-HR02b-REQ01/02 → OVE-HR02b-ADR01 → OVE-HR02b-EXP01 → OVE-HR02b-T01 → OVE-HR02b-KPI01. **OVE-HR02b-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/2727efa28ad34c078eeab152a5b510a6); fetched revision 2026-09-03T20:08:03.678Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Onboarding Case — Persona-Led Architecture Lab**  
	All characters and events are fictional.

## Case Mission
> **Transform onboarding into a governed workforce-readiness system for energy operations.**
At OmniEnergy, a new worker may need payroll registration, medical fitness clearance, offshore credentials, PPE, site induction, devices, identity, travel, accommodation, safety learning, export-control approval, and physical access before productive work begins. Document completion alone does not equal readiness.
## Fictional Lead Persona
### Priya Menon — Global Energy Workforce Readiness Director
Priya has six months to pilot SAP SuccessFactors Onboarding for a Gujarat refinery and a North Sea offshore operation. She must coordinate recruiting, HR, payroll, IT, security, HSE, facilities, learning, travel, and managers across multiple worker types.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Priya Menon
 | Global Workforce Readiness Director
 | Owns the accepted-offer-to-90-day experience and readiness outcome.

 | Thomas Reid
 | Offshore Installation Manager
 | Cannot mobilize workers without verified safety and travel prerequisites.

 | Leila Hassan
 | New Hire Persona — Process Engineer
 | Needs clear tasks, equipment, access, mentoring, and role expectations.

 | Grace Liu
 | Identity and Equipment Service Owner
 | Needs complete data and timely events for provisioning.

 | Rafael Pinto
 | HSE Assurance Director
 | Requires auditable proof before restricted work authorization.

## Transformation Dilemma
Should onboarding remain an HR process, be owned by individual sites, or become a cross-functional workforce-readiness product? Priya must create one coherent experience while supporting employees, contractors, transfers, rehires, graduates, and mobile workers.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Global minimum readiness, local compliance, frontline-first design, accessibility, and no work without prerequisites.
- **Portfolio:** Preboarding, identity, payroll, equipment, HSE, learning, manager readiness, and 30/60/90-day ramp-up.
- **Program:** Pilot refinery and offshore personas, then scale by risk and workforce pattern.
### V2 — Value
- **Platform:** SuccessFactors Onboarding, Employee Central, identity, learning, payroll, access, case, and analytics platforms.
- **Product:** New-hire journey, manager workspace, readiness dashboard, mentor experience, and exception command center.
- **Process:** Accepted offer → Preboarding → Provisioning → Day one → Certification → Role ramp-up → 90-day proficiency.
### V3 — Victory
- **People:** New hires, managers, mentors, HR, HSE, IT, payroll, security, and service owners.
- **Practice:** Task ownership, SLAs, readiness gates, exception reviews, journey analytics, and monthly quality governance.
- **Project:** Simulate onboarding failures before pilot release and measure readiness for three cycles.
### V4 — Venture
Reuse event-driven journeys for contractors, cross-site transfers, international assignments, acquisitions, partner workers, and large project mobilizations.
## Decision Scenes
- **Day-one failure:** Eighteen refinery operators lack verified induction, eleven badges are inactive, and six payroll records are incomplete.
- **Offshore mobilization:** Thomas must fill a rotation, but two workers lack current credentials.
- **Journey overload:** Leila receives 37 unsequenced tasks from seven functions.
- **Early attrition:** New engineers report weak mentoring and unclear first-90-day expectations.
## 12-Stream Architecture Assignment
Connect business readiness, employee journeys, onboarding processes, worker and readiness data, Onboarding applications, identity/payroll/HSE integrations, mobile technology, security, analytics, AI-supported guidance, change, and value.
## Capstone Deliverables
1. Persona-based preboarding and 0–90-day journeys
2. Global minimum standard and local-variation matrix
3. Readiness object, event, task, and ownership architecture
4. HSE, medical, access, privacy, and compliance controls
5. Manager and mentor playbooks
6. Exception and escalation command center
7. Onboarding integration blueprint
8. Pilot and scale roadmap
9. New-hire communication design
10. Readiness, proficiency, experience, and retention dashboard
## Victory Measures
- Above 95% verified day-one readiness
- Above 98% mandatory-learning compliance
- Reduced equipment, identity, payroll, and access exceptions
- Faster time-to-proficiency
- Lower first-90-day attrition
- Improved new-hire and manager experience
## Assessment Checkpoint
Learners act as Priya’s Workforce Readiness Design Team and must distinguish administrative completion from safe, productive readiness. Every dependency requires an owner, rule, evidence source, exception path, and outcome measure.
> 
	**Final Challenge:** How should Priya ensure every new worker is safe, equipped, connected, paid, welcomed, and productive—without creating an unmanageable global process?

