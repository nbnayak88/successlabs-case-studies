# OVE-HR02a — Talent acquisition

[HR studio](README.md) · [Enterprise master](../../../master/README.md)

## Canonical HR expansion — OVE-HR02a

**Version:** 1.0, 2026-10-19. **Evidence:** original fictional source + new illustrative design. **Enterprise sponsors:** OVE-P01, OVE-P04. **Master anchors:** OVE-M03, M09–M12, M15–M20 (full IDs use OVE-M prefix). **Lead:** Arjun Malhotra — Global Talent Acquisition Product Owner.

### A — Understand (master 01–04)
**Mission:** **Build a fast, fair, skills-led recruiting engine for the global energy transition.**
OmniEnergy needs petroleum engineers, refinery operators, offshore technicians, renewable-project managers, grid specialists, data scientists, cybersecurity professionals, and future leaders. Long vacancies constrain asset reliability and renewable growth, while inconsistent selection practices create candidate, fairness, and compliance risks.

**Personas and proposed decision rights:**
- **OVE-HR02a-P01 — Arjun Malhotra, Global TA Product Owner:** Owns recruiting outcomes, platform, governance, and candidate trust. Proposed domain design owner; sponsor approves funding.
- **OVE-HR02a-P02 — Sofia Bennett, Renewables Growth President:** Needs 200 project and engineering hires before construction begins. Domain counterpart; validate authority during discovery.
- **OVE-HR02a-P03 — Kwesi Boateng, Offshore Operations Director:** Requires certified workers for rotational and hazardous environments. Domain counterpart; validate authority during discovery.
- **OVE-HR02a-P04 — Elena Markovic, Responsible AI and Privacy Counsel:** Challenges opaque screening and unnecessary candidate data. Domain counterpart; validate authority during discovery.
- **OVE-HR02a-P05 — Noor Rahman, Candidate Persona — Grid Engineer:** Expects clear requirements, timely communication, and fair assessment. Domain counterpart; validate authority during discovery.

Source character names are retained and namespaced. HR07 Meera Iyer is distinct from OVE-P14; HR10 Carlos Mendes is distinct from OVE-P09. Shared names do not establish shared identity.

### B — Direction (master 05–08)
**Strategic dilemma:** Should OmniEnergy centralize recruiting, preserve business-led hiring, or establish a federated talent-acquisition product model? Arjun must balance urgent staffing, scarce skills, internal mobility, regional labor markets, diversity, assessment quality, and candidate experience.

**Discovery questions:** Which worker population and business decision are affected? Which source record proves the problem? Who approves country variants? What must remain safe during a failed handoff? What evidence would make us reject our preferred design?

**Options:** retain and control existing local practice; impose a uniform template; or use a common core with justified local variants. Compare worker impact, control coverage, delivery effort and reversibility. No option is approved merely by appearing here.

### C — Architecture (master 09–12)
**OVE-HR02a-CAP01 capability group:** Demand authorization; candidate assessment; offer governance. These are abilities; the following sequence is a value stream, not a capability hierarchy.

**OVE-HR02a-VS01 value stream:** Demand → approve requisition → attract → assess → select → accept. Define a stakeholder-valued exit criterion at each stage before detailed process modeling.

**Information objects:** requisition; candidate; assessment evidence; consent/purpose; offer version. Record attribute owner, authoritative source, purpose, access, retention, effective date and quality rule.

**Application responsibility:** Recruiting owns candidate and requisition states; finance authorizes funded positions; EC creates employment through a governed handoff.

**Architecture decision OVE-HR02a-ADR01 (proposed):** maintain explicit ownership and governed handoffs rather than uncontrolled copies. HR12 owns transport/recovery patterns; this domain owns its business rules and acceptance. Identity, data, UX and infrastructure views reference the shared [architecture boundaries](operating-standard.md).

### D — Transformation (master 13–16)
**OVE-HR02a-REQ01:** every in-scope business change has a unique case/event reference, authorized decision, effective date and traceable downstream outcome. **OVE-HR02a-REQ02:** a rejected or delayed change remains visible to an accountable owner; a silent drop cannot count as completion. Define domain-specific fields above before build.

**OVE-HR02a-EXP01 — delivery experiment:** use synthetic data for one representative population and one contrasting workforce/country variant. Establish the baseline, replay the decision scenes below, compare outcomes and collect worker feedback. Progress: discovery → stakeholder simulation → capability/value-stream design → architecture decision → experiment → evidence/outcomes. Learners may loop back when evidence changes the question.

**Gates:** design owner accepts rules and source ownership; sponsor accepts business scope; payroll/HSE/security accept applicable controls; pilot owner demonstrates failure recovery; Finance accepts any value claim. Scale only after documented acceptance. Funding and delivery dates remain TBD; source timelines are learning assumptions.

### E — Execute and assure (master 17–19)
**Scenario-specific decision scenes from the source:**
- **Speed versus evidence:** Sofia asks to shorten selection for 200 urgent hires.
- **AI fairness:** Progression rates fall for one candidate group after automated recommendations are introduced.
- **Safety-critical quality:** Kwesi finds that agency candidates lack validated offshore credentials.
- **Candidate trust:** Noor receives contradictory communications and no explanation of the assessment stage.

**OVE-HR02a-T01 test portfolio:** 200 urgent hires with missing credentials; duplicate applicant; withdrawn consent; adverse recommendation challenged by human reviewer. For each test capture input, expected result, actual result, evidence reference, owner and pass/fail. **Status: designed, not executed.** A failed critical safety/pay/access case blocks release; resolve defects and rerun affected paths. Record fallback and recovery ownership.

**Simulation:** act as Arjun Malhotra — Global Talent Acquisition Product Owner; open with the first decision scene. Reveal source details only after useful questions. Challenge unsupported claims, request a counter-option and finish with an explicit decision and evidence request. Score discovery 20, capability/value 20, traceability 20, risk/trade-offs 15, communication 15, closure 10. Learner STAR responses are hypothetical.

### F — Evidence and outcomes (master 20–22)
**OVE-HR02a-KPI01:** Time-to-fill = accepted-offer date minus approved-requisition date; pair with credential-validation and candidate-fairness measures. Owner: domain lead unless specified; cadence: proposed pilot review and monthly follow-up. Establish denominator, exclusions, as-of date and baseline before setting a numeric target. Original source “Victory Measures” are targets, not achievements.

**Trace:** source OVE-HR02a-SRC → OVE-HR02a-CAP01 → OVE-HR02a-VS01 → OVE-HR02a-REQ01/02 → OVE-HR02a-ADR01 → OVE-HR02a-EXP01 → OVE-HR02a-T01 → OVE-HR02a-KPI01. **OVE-HR02a-EV01 is an evidence slot, not observed evidence.** No executed test, live tenant implementation, certification, ROI or realized operational outcome is asserted.

**Review pack:** discovery brief, persona simulation transcript, stage/capability matrix, requirements and ADR, synthetic test results, worker feedback, outcome ledger and decision to stop/redesign/scale. Markdown is the published format; PPT/Gamma/Yoodli assets are not yet published.

**Source:** [preserved Notion case](https://app.notion.com/p/d6d16db9507b453fa4cbad6eaeec9eeb); fetched revision 2026-09-03T20:08:03.582Z. Original 9P4V journey and research remain below in GitHub and unchanged above this appendix in Notion. Standards mappings are educational, not compliance certification. See [source/conflict register](source-register.md).


---
## Original source research — preserved snapshot
Source alias “OmniEnergy” is retained below; canonical enterprise identity is OmniVerse Energy Ltd. Source product selections and outcomes remain fictional assumptions.


> 
	**Applied Energy Talent Acquisition Case — Persona-Led Architecture Lab**  
	All characters and scenarios are fictional and designed for professional learning.

## Case Mission
> **Build a fast, fair, skills-led recruiting engine for the global energy transition.**
OmniEnergy needs petroleum engineers, refinery operators, offshore technicians, renewable-project managers, grid specialists, data scientists, cybersecurity professionals, and future leaders. Long vacancies constrain asset reliability and renewable growth, while inconsistent selection practices create candidate, fairness, and compliance risks.
## Fictional Lead Persona
### Arjun Malhotra — Global Talent Acquisition Product Owner
Arjun must fill 450 safety-critical and scarce-skill roles within six months while redesigning recruitment through SAP SuccessFactors Recruiting. He must improve speed without allowing hiring managers, agencies, or AI-supported tools to weaken job relevance, transparency, or human accountability.
## Character Ecosystem

 | Character
 | Role
 | Position and concern

 | Arjun Malhotra
 | Global TA Product Owner
 | Owns recruiting outcomes, platform, governance, and candidate trust.

 | Sofia Bennett
 | Renewables Growth President
 | Needs 200 project and engineering hires before construction begins.

 | Kwesi Boateng
 | Offshore Operations Director
 | Requires certified workers for rotational and hazardous environments.

 | Elena Markovic
 | Responsible AI and Privacy Counsel
 | Challenges opaque screening and unnecessary candidate data.

 | Noor Rahman
 | Candidate Persona — Grid Engineer
 | Expects clear requirements, timely communication, and fair assessment.

## Transformation Dilemma
Should OmniEnergy centralize recruiting, preserve business-led hiring, or establish a federated talent-acquisition product model? Arjun must balance urgent staffing, scarce skills, internal mobility, regional labor markets, diversity, assessment quality, and candidate experience.
## 9P4V Transformation Journey
### V1 — Vision
- **Policy:** Skills-first, position-led, explainable, inclusive, privacy-aware, and human-controlled selection.
- **Portfolio:** Workforce demand, career sites, sourcing, pipelines, assessments, interviews, offers, analytics, and AI controls.
- **Program:** Prioritize offshore, refinery, renewable, digital, and graduate hiring waves.
### V2 — Value
- **Platform:** SAP SuccessFactors Recruiting, Employee Central, assessments, scheduling, CRM, analytics, and onboarding integration.
- **Product:** Requisition, candidate journey, talent community, hiring-manager workspace, and recruiting decision products.
- **Process:** Demand → Position → Requisition → Attraction → Screening → Interview → Offer → Hire → Onboarding.
### V3 — Victory
- **People:** Recruiters, hiring managers, assessors, HR business partners, privacy, DEI, and candidates.
- **Practice:** Structured scorecards, response SLAs, adverse-impact reviews, consent, audit, and source-quality management.
- **Project:** Pilot renewable engineering and offshore maintenance before scaling.
### V4 — Venture
Build alumni communities, apprenticeships, university partnerships, internal-first matching, contingent-talent networks, and reusable energy skills intelligence.
## 12-Stream Architecture Assignment
Connect workforce demand, candidate journeys, recruiting processes, job and skills data, Recruiting applications, assessment and onboarding integrations, security, privacy, analytics, AI assurance, adoption, and measurable hiring value.
## Decision Scenes
- **Speed versus evidence:** Sofia asks to shorten selection for 200 urgent hires.
- **AI fairness:** Progression rates fall for one candidate group after automated recommendations are introduced.
- **Safety-critical quality:** Kwesi finds that agency candidates lack validated offshore credentials.
- **Candidate trust:** Noor receives contradictory communications and no explanation of the assessment stage.
## Capstone Deliverables
1. Talent Acquisition Vision Canvas
2. Scarce-role workforce-demand map
3. Candidate personas and journey maps
4. Position-led requisition architecture
5. Structured selection and interview scorecards
6. Responsible-AI and adverse-impact controls
7. Recruiting-to-onboarding integration blueprint
8. 180-day critical-hiring plan
9. Recruiter and manager adoption model
10. Speed, quality, fairness, experience, and retention dashboard
## Victory Measures
- Reduced critical-role time-to-fill and vacancy cost
- Higher qualified-candidate conversion
- Improved offer acceptance and early retention
- Increased internal-fill and diverse-slate rates
- Audited selection consistency
- Improved candidate and hiring-manager experience
## Roadmap
1. Baseline critical demand, funnels, sources, and candidate pain points.
2. Standardize job architecture, requisitions, scorecards, and approvals.
3. Configure Recruiting and priority integrations.
4. Pilot two scarce-role families.
5. Measure fairness, quality, speed, and adoption.
6. Scale talent communities and skills-based matching.
## Assessment Checkpoint
Learners act as Arjun’s Talent Acquisition Architecture Squad. A strong design demonstrates that autonomous recruitment means intelligent orchestration and reduced administration—not automated employment decisions.
> 
	**Final Challenge:** How should Arjun meet urgent energy-workforce demand while preserving fairness, safety, candidate dignity, and accountable hiring decisions?

