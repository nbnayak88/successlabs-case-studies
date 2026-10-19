# OVE-HR06 — Learning and internal mobility

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR06

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P09, OVE-P04. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Dr. Kabir Sen — Chief Learning, Skills, and Mobility Architect.

### A — Understand (master 01–04)
**Mission:** **Convert learning activity into verified capability, safe work, and visible career opportunity.**
OmniEnergy must reskill its workforce for renewables, battery storage, hydrogen, digital twins, AI, OT cybersecurity, advanced maintenance, ESG, and customer energy services. Training records are fragmented, certifications expire unnoticed, and employees cannot easily see pathways from traditional energy roles into emerging careers.

**Personas and proposed decision rights:**
- **OVE-HR06-P01 — Dr. Kabir Sen, Chief Learning and Mobility Architect:** Owns skills strategy, academies, governance, mobility, and impact. Proposed domain design owner; sponsor approves funding.
- **OVE-HR06-P02 — Hannah Weber, Refinery Technician Persona:** Wants a credible pathway into hydrogen operations. Domain counterpart; validate authority during discovery.
- **OVE-HR06-P03 — Diego Alvarez, HSE and Work Authorization Director:** Requires verified competence before restricted work. Domain counterpart; validate authority during discovery.
- **OVE-HR06-P04 — Yuki Sato, Renewable Energy Academy Lead:** Needs rapid, expert-reviewed future-skill pathways. Domain counterpart; validate authority during discovery.
- **OVE-HR06-P05 — Sarah Mensah, Finance Business Partner:** Challenges learning investments without operating evidence. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Should OmniEnergy prioritize compliance, role proficiency, energy-transition academies, or mobility first? Kabir must create an integrated portfolio without weakening safety or flooding employees with disconnected courses.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR06-CAP01 capability group:** Skills assessment; learning pathways; competence verification; mobility. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR06-VS01 value stream:** Skill demand → gap → explore → practice → assess → verify → deploy. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** skill; proficiency evidence; assessor; credential expiry; opportunity; work authorization. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** LMS owns learning records; qualified assessors validate competence; HSE authorizes restricted work; marketplace recommends opportunities.

**Architecture decision OVE-HR06-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR06-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR06-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR06-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Completion versus competence:** Hannah completes online modules but lacks practical evidence.
- **Work authorization failure:** A delayed certification feed creates unsafe eligibility.
- **Rapid content demand:** Yuki wants new AI and hydrogen courses before expert review.
- **Value challenge:** Sarah asks whether learning improves downtime, incidents, mobility, or project delivery.

**OVE-HR06-T01 test portfolio:** Online completion without practical assessment; expired credential; delayed feed; unreviewed hydrogen content; inaccessible learning. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Dr. Kabir Sen — Chief Learning, Skills, and Mobility Architect; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR06-KPI01:** Time-to-verified-competence = verification date minus pathway start; record successful practical assessment rather than completion alone. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR06-SRC → OVE-HR06-CAP01 → OVE-HR06-VS01 → OVE-HR06-REQ01/02 → OVE-HR06-ADR01 → OVE-HR06-EXP01 → OVE-HR06-T01 → OVE-HR06-KPI01. **OVE-HR06-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/f3e53d3a136849b1978ce0646d40988f); fetched revision 2026-09-03T23:23:37.248Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Learning and Mobility Case — Persona-Led Architecture Lab**  
	All characters and events are fictional.

## Case Mission
> **Convert learning activity into verified capability, safe work, and visible career opportunity.**
OmniEnergy must reskill its workforce for renewables, battery storage, hydrogen, digital twins, AI, OT cybersecurity, advanced maintenance, ESG, and customer energy services. Training records are fragmented, certifications expire unnoticed, and employees cannot easily see pathways from traditional energy roles into emerging careers.
## Fictional Lead Persona
### Dr. Kabir Sen — Chief Learning, Skills, and Mobility Architect
Kabir must connect SAP SuccessFactors Learning with Opportunity Marketplace and trusted skills evidence. His immediate concern is a technician who completed online training but was granted restricted-work eligibility without a recorded practical assessment.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Dr. Kabir Sen
 | Chief Learning and Mobility Architect
 | Owns skills strategy, academies, governance, mobility, and impact.

 | Hannah Weber
 | Refinery Technician Persona
 | Wants a credible pathway into hydrogen operations.

 | Diego Alvarez
 | HSE and Work Authorization Director
 | Requires verified competence before restricted work.

 | Yuki Sato
 | Renewable Energy Academy Lead
 | Needs rapid, expert-reviewed future-skill pathways.

 | Sarah Mensah
 | Finance Business Partner
 | Challenges learning investments without operating evidence.

## Transformation Dilemma
Should OmniEnergy prioritize compliance, role proficiency, energy-transition academies, or mobility first? Kabir must create an integrated portfolio without weakening safety or flooding employees with disconnected courses.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Verified evidence, learning in work, accessible opportunity, content ownership, and no certification without competence.
- **Portfolio:** Mandatory learning, role pathways, future skills, credentials, academies, projects, mentoring, and mobility.
- **Program:** Pilot maintenance-to-hydrogen and field-service-to-renewables pathways.
### V2 — Value
- **Platform:** SuccessFactors Learning, Opportunity Marketplace, Employee Central, Performance, Succession, and analytics.
- **Product:** Role pathway, credential, learning academy, opportunity profile, and manager skills dashboard.
- **Process:** Demand → Skill gap → Learning → Practice → Assessment → Verification → Opportunity → Deployment.
### V3 — Victory
- **People:** Learners, managers, experts, instructors, HSE, talent teams, and academy owners.
- **Practice:** Content lifecycle, assessment standards, credential review, skill validation, and impact measurement.
- **Project:** Pilot two transition pathways and measure proficiency, mobility, safety, and retention.
### V4 — Venture
Build expert communities, partner academies, portable credentials, project marketplaces, and a skills-powered energy workforce ecosystem.
## Decision Scenes
- **Completion versus competence:** Hannah completes online modules but lacks practical evidence.
- **Work authorization failure:** A delayed certification feed creates unsafe eligibility.
- **Rapid content demand:** Yuki wants new AI and hydrogen courses before expert review.
- **Value challenge:** Sarah asks whether learning improves downtime, incidents, mobility, or project delivery.
## 12-Stream Architecture Assignment
Connect capability strategy, learner journeys, learning and mobility processes, skills and certification data, LMS and Marketplace applications, work-authorization integration, security, analytics, AI recommendations, adoption, and value.
## Capstone Deliverables
1. Enterprise skills strategy
2. Priority energy-transition capability map
3. Role-to-skill-to-learning pathways
4. Assessment, credential, and work-authorization architecture
5. Opportunity Marketplace and mobility design
6. Content ownership and lifecycle model
7. Learner, manager, expert, and instructor journeys
8. Academy and partner ecosystem roadmap
9. Learning integration blueprint
10. Compliance, proficiency, mobility, retention, and impact dashboard
## Victory Measures
- Sustained certification compliance
- Faster verified time-to-competency
- Measurable critical-skill-gap closure
- Increased internal mobility
- Improved safety and operational outcomes
- Higher retention in transition pathways
## Assessment Checkpoint
Learners act as Kabir’s Energy Capability Academy Team. They must prove how learning evidence becomes safe work authorization, career movement, and measurable business capability.
> 
	**Final Challenge:** How should Kabir help experienced energy workers move into future roles without confusing course completion with verified capability?

