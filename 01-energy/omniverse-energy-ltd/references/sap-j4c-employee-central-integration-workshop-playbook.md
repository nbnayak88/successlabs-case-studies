**Disclaimer:** *All AI-generated outputs are draft materials and must be reviewed and validated by a qualified consultant before use in the project.*

# SAP J4C Outcome for Employee Central — Integration Workshop Playbook

**OmniVerse Energy Ltd. | SAP Activate Explore | Consultant preparation guide | 7 November 2026 | v1.0**

## 1. Meeting purpose and evidence baseline

Use this playbook as the EC consultant's working script for the six interface reviews shown in the supplied screenshot: Finance, P2P, O2C, Manufacturing, Warehouse and Asset Management. It extends [SAP J4C Outcome for Employee Central](source-and-assumptions.md) and the [HR01 source case](../derived-streams/hr/hr01-workforce-foundation.md).

**Confirmed:** Employee Central implementation and Explore-stage preparation, as stated by the user; the six workshop topics and dependency concerns in the screenshot. **Unconfirmed:** actual target products/editions/releases, SAP Scope Item IDs, architecture, APIs, middleware, dates, appointed business owners, contractual scope and service levels. The screenshot is a scoping matrix, not an approved interface specification. Questions, example tests, ownership proposals and timings below are proposed preparation content. Record actual answers and evidence before approving a design.

The fictional case has 68,000 employees in 42 countries; this is enterprise scale, not a confirmed rollout population. Anika Sharma, Farah Al-Mansoori, Michael Torres, Samuel Okoro and Mei Wong are source personas, not verified meeting attendees. Existing candidate deltas about local fields/workflows, duplicate employments, missing effective dates, certification profiles and termination access remain unvalidated.

**Consultant outcome:** leave each workshop with a business use case, object ownership, source/target contract, agreed temporal behavior, security controls, error/recovery ownership, test criteria and a dated action list. “Send employee data to module X” is insufficient.

## 2. What to say and ask first

**Opening script:** “I represent the Employee Central design. Let us start with the business action your system must perform, the workforce facts it needs, and the evidence that the action completed. We will agree ownership, dates, exceptions and controls before selecting an interface.”

Ask these five questions before discussing a technology:
1. Which business activity fails today, who experiences the impact, and can you show one synthetic example?
2. What is the exact receiving system and object, and who can demonstrate its standard behavior?
3. Which fact is authoritative in EC, which in your system, and which belongs to another owner?
4. When must the fact become effective, and what happens while delivery or processing is incomplete?
5. Who can accept the end-to-end outcome, and what evidence will they use?

**Close with:** “Please read back the agreed source, target, ownership, timing, failure route and acceptance criteria. Which open point blocks design approval, who owns it, and by when will we resolve it?”

## 3. Workshop sequence, participants and preparation

| Workshop | Focus | Prerequisite | Essential customer decision-maker | EC preparation |
|---|---|---|---|---|
| WS00 | Shared identity, object ownership, lifecycle and integration conventions | Landscape inventory | HR, IT/integration and IAM owners | Organization model; identity options; lifecycle scenarios |
| WS01-FIN | Cost-center master and workforce assignments | WS00; finance reference model | Finance/CO owner | Cost-center/legal-entity questions and effective dates |
| WS02-P2P | Purchasing responsibility and approvals | WS00; Finance dependencies where relevant | Procurement/workflow owner | Transfer/manager/termination scenarios |
| WS03-O2C | Customer-facing workforce roles | WS00 | Sales/customer-service owner | Role changes and handover scenarios |
| WS04-MFG | Plant workforce and safety boundaries | WS00; approved reference mappings | Production and HSE owners | Position/location and certification boundary |
| WS05-WH | Warehouse resources, users and access | WS00; target WMS identified | Warehouse and IAM owners | Location/worker lifecycle examples |
| WS06-AM | Maintenance resources and work authorization | WS00; permit/qualification ownership | Maintenance and HSE owners | Technician/contractor lifecycle examples |
| WS07 | Cross-interface design readback and test plan | WS01–06 outputs | Business process owners + IT | Consolidated contract and unresolved decision list |

Actual dates, named appointments and time zone: **TBD — PM to confirm**. Finance should precede dependent assignment designs; do not assume P2P/O2C/MFG/WH/AM are separate direct EC feeds. They may consume shared workforce or IAM data.

### D−5 business days: request from attendees

- [ ] Business owners: two routine and two exception cases, volumes, cutoff times, service impact, business rules and sign-off authority.
- [ ] Non-SF consultants: target process diagram, standard object model, release/edition, required fields, reference dependencies and demonstration script.
- [ ] Integration experts: existing interface inventory, standard integration-content candidates, supported API documentation, monitoring and recovery design.
- [ ] Technical users: sanitized payloads, sample errors, authorization model, environment readiness and target business-success evidence.
- [ ] SMEs: qualification/permit, finance approval, delegation, segregation-of-duties and contractor policies as applicable.
- [ ] EC consultant: relevant data-model/workflow/RBP baseline; synthetic hire, transfer, rehire, concurrent employment, leave and termination records.
- [ ] PM: decision-maker attendance, action log, calendar and acceptance route; identify unavailable inputs before the meeting.

Do not request passwords, secrets, live personal data or real employee payloads for this public teaching repository.

## 4. Repeatable detailed workshop agenda

**Proposed 3-hour session per area**, followed by a 90-minute technical clinic if mappings cannot be resolved. Relative times avoid inventing a booked date.

| Time | Duration | Activity | Owner | Output |
|---|---|---|---|---|
| T+00–15 | 15 min | Confirm use cases, scope, systems and decision authority | Business Lead + EC consultant | Business outcome and boundaries |
| T+15–35 | 20 min | Show As-Is and one failed business scenario | Business user + target consultant | Evidence and pain-point baseline |
| T+35–60 | 25 min | Demonstrate target standard process and required workforce objects | Non-SF functional consultant | Verified standard dependency |
| T+60–85 | 25 min | Agree authoritative data, keys and mappings | EC + target consultant + data owner | Object/field ownership |
| T+85–95 | 10 min | Break | Facilitator | — |
| T+95–120 | 25 min | Resolve dates, retro/future changes and in-flight work | Business SME + EC consultant | Temporal rules |
| T+120–145 | 25 min | Review delivery, access, errors, replay and reconciliation | Integration + technical + IAM | Operational contract |
| T+145–165 | 20 min | Run exception scenarios; define acceptance and classification | Business owner + consultants | Test and delta records |
| T+165–180 | 15 min | Read back decisions, dissent, actions and approval conditions | PM + Business Lead | Signed/conditional minutes |

| Technical clinic time | Duration | Activity | Owner | Output |
|---|---|---|---|---|
| T+00–30 | 30 min | Inspect object/field mapping and actual supported API semantics | EC + target developer | Mapping draft and evidence |
| T+30–55 | 25 min | Walk through sample messages, dates and error categories | Integration lead | Contract and failure handling |
| T+55–75 | 20 min | Verify security, monitoring, replay and reconciliation | IT + IAM + operations | Control/runbook draft |
| T+75–90 | 15 min | Assign unresolved proof tasks and review date | Architect + PM | Design gate actions |

Jointly deliver each session with an experienced SAP consultant/partner and customer business lead. Understand the As-Is; have the business lead execute the standard process rather than only watch slides.

## 5. Shared questions to ask every interface team

| ID | Ask whom | Exact question | Capture before leaving |
|---|---|---|---|
| C01 | Business Lead | What is the measurable business consequence if this update is late, wrong or absent? | Impact, priority and business acceptance owner |
| C02 | Target consultant | Show the target standard process and the actual object/field that consumes this data. | Product/release; object; standard behavior evidence |
| C03 | Data steward | Who creates, changes and retires each object/attribute? Is any direction bidirectional, and how are conflicts prevented? | Attribute-level authority and precedence |
| C04 | EC + target SME | Which person, employment, assignment and login keys are required? How do rehire and concurrent employment behave? | Crosswalk and key lifecycle |
| C05 | Business + target SME | Are employees, contingent workers, agency staff and contractors all required? Which source owns each population? | Population filter and authoritative source |
| C06 | Integration lead | Is there a supported standard integration for this precise landscape? Can consumers reuse a shared feed? | Package/version; fit evidence; architecture alternative |
| C07 | Technical lead | Is the target expecting full history, a dated snapshot or deltas? Can it hold future time slices? | Extraction/target temporal contract |
| C08 | Business + EC | What happens for future hires, rescinded terminations, backdated transfers and corrected effective dates? | Event-specific business rules |
| C09 | Integration lead | How do initial load, delta checkpoint, overlap, ordering and duplicate handling work? | No-loss/no-duplicate proof |
| C10 | Target technical SME | Does acknowledgement prove delivery only or completed business processing? Where is rejection visible? | Technical versus business acknowledgement |
| C11 | Operations | Who detects, owns and resolves source, mapping, reference-data, transport and target errors? | Ownership and escalation by error class |
| C12 | Operations + business | What are the agreed latency, cutoff, recovery and backlog targets? What happens during outage? | Measurable targets; all values TBD until agreed |
| C13 | IAM/security | Which facts trigger an access review, and which system grants/removes authorization? | Separation of HR facts, accounts and permissions |
| C14 | Privacy owner | Which fields are necessary? What retention, masking, regional transfer and log-access controls apply? | Minimum payload and approved evidence handling |
| C15 | Test lead + business | How do we reconcile source, accepted, rejected and pending outcomes at an as-of date? | Test assertions, report and sign-off evidence |

**EC technical prompts:** identify relevant objects such as person identifiers, employment identifiers, Job Information, effective start date, sequence where applicable, event reason, legal entity, position, location, manager and cost center. Treat these as conceptual candidates; validate exact API names, availability, permissions and target mappings. Do not send salary, national identifiers or other sensitive fields merely because they exist.

**Questions to challenge unclear answers**
- “Real time”: What maximum delay can the business accept, measured from which event to which confirmed outcome?
- “Standard”: Which package/API and version demonstrate that behavior in this landscape?
- “Same employee ID”: Same person, employment, assignment, business partner or login? Show a concurrent-employment case.
- “Successful”: Was the message delivered, the target object updated, or the user able to complete the business task?
- “EC will handle it”: Which EC object/rule owns that responsibility, and what remains owned by IAM, learning, HSE or the target module?

## 6. Finance workshop — WS01-FIN

**Purpose:** Cost-center ownership, assignment validity and effective-date handoff.  
**Invite:** Finance/CO lead, cost-center steward, EC consultant, payroll control, integration lead, finance authorization SME.  
**Bring:** Synthetic cost-center create/change/close records; company/controlling-area map; employee assignment histories; period/cutoff calendar; source/target examples.  
**Decision to secure:** Approve object authority, unique keys, validity handling, dependency sequence, costing boundary and finance acceptance owner.

| Question ID | Ask whom | Question to ask | Required answer / evidence |
|---|---|---|---|
| FIN-01 | Business | Which workforce decisions require cost-center data: primary assignment, costing allocation, approval ownership or reporting? Who signs each use? | Business use and owner |
| FIN-02 | Business | Who owns creation, closure, blocking and validity changes of cost centers? What happens to workers assigned to a closing cost center? | Lifecycle policy |
| FIN-03 | Functional | Which actual Finance system, edition and release owns the object? Are controlling area plus cost-center code needed for uniqueness across systems? | Source and key design |
| FIN-04 | Functional | How do company code, EC legal entity and controlling area map? Can one EC legal entity use several source instances? | Mapping and exceptions |
| FIN-05 | Functional | Does EC require only primary cost center or an approved cost-distribution design? Which downstream system owns actual financial postings? | Assignment versus posting boundary |
| FIN-06 | Functional | How should a future-dated closure, retroactive transfer or corrected assignment affect existing employee histories and open periods? | Temporal business rules |
| FIN-07 | Integration | Which supported cost-center replication content fits the actual landscape? Which direction is needed for cost-center master versus employee assignment? | Separate interface contracts |
| FIN-08 | Integration | Must cost centers arrive before employment assignments? How will missing references be held, repaired and replayed? | Dependency control |
| FIN-09 | Technical | How are validity dates, leading zeros, source IDs, language-dependent labels and responsible-person references transformed? | Field-level mapping |
| FIN-10 | Technical | What proves target business acceptance beyond message delivery? How will source and target records reconcile at an agreed as-of date? | Reconciliation design |
| FIN-11 | SME | Does an EC manager or cost-center responsible person automatically obtain spending authority? Which finance approval controls remain separate? | Authorization boundary |
| FIN-12 | SME | Who approves an emergency reassignment at payroll/period cutoff, and who verifies the resulting finance and payroll impacts? | Exception accountability |

**Scenario walkthroughs:** Future-dated cost-center creation before worker transfer; closure with active assignments; identical codes in two controlling areas; late-arriving master; retroactive transfer in a closed finance period. For each, ask the business user to explain the desired action, the functional consultant to demonstrate target standard, the integration expert to trace the message and the SME to accept the control result.

**Readback:** Approve object authority, unique keys, validity handling, dependency sequence, costing boundary and finance acceptance owner. Record actual owners, timing, chosen pattern and remaining evidence; do not classify as Fit solely because an API exists.

## 7. Procure-to-Pay / Procurement workshop — WS02-P2P

**Purpose:** Worker and approver changes affecting purchasing authority.  
**Invite:** Procurement lead, purchasing workflow consultant, requisitioners, delegation/SoD SME, IAM, integration lead.  
**Bring:** Approval matrix; purchasing-role ownership; delegation policy; synthetic open requisition/service-entry examples; SoD controls; target identity model.  
**Decision to secure:** Approve approval ownership, delegation rules, in-flight reassignment, minimum workforce fields and SoD/access controls.

| Question ID | Ask whom | Question to ask | Required answer / evidence |
|---|---|---|---|
| P2P-01 | Business | Which purchasing actions depend on worker data: requisition, approval, receipt, service entry or purchasing-group responsibility? | Action/population map |
| P2P-02 | Business | What must happen to open requisitions and approvals when an employee transfers, takes leave or leaves the company? | In-flight work rules |
| P2P-03 | Business | Who appoints substitutes, for what dates, and who removes delegated authority? | Delegation governance |
| P2P-04 | Functional | Are approvals derived from EC manager, cost-center owner, target workflow teams, purchasing organization or a maintained responsibility matrix? | Approval source of truth |
| P2P-05 | Functional | Are spend thresholds, purchasing groups and release strategies maintained outside EC? Which workforce attributes are genuinely necessary? | Minimal data contract |
| P2P-06 | Functional | Can one worker hold roles across company codes or purchasing organizations? How are concurrent employment and local identities distinguished? | Cross-entity rules |
| P2P-07 | Integration | Is there a direct EC-to-procurement feed, a shared workforce feed, or an IAM-mediated flow? Which target object is actually consumed? | Dependency topology |
| P2P-08 | Integration | How will worker status, manager changes and delegation dates reach workflow evaluation without creating conflicting copies? | Update and precedence rules |
| P2P-09 | Technical | What identifier links EC employment, target employee/business partner if required, and login? Show the actual target model. | Identity crosswalk |
| P2P-10 | Technical | What happens if identity exists but procurement authorization is not ready, or worker replication succeeds but workflow assignment fails? | Partial-failure recovery |
| P2P-11 | SME | Who prevents self-approval and incompatible duties? Does a new EC job/manager value trigger review rather than auto-grant? | SoD and approval control |
| P2P-12 | SME | For terminated contractors, which source owns end dates and who verifies both purchasing access removal and reassignment of pending work? | Contractor control |

**Scenario walkthroughs:** Approver terminates with pending requisitions; transfer across purchasing organizations; delegate expires during approval; duplicate manager update replay; contractor end date precedes account removal. For each, ask the business user to explain the desired action, the functional consultant to demonstrate target standard, the integration expert to trace the message and the SME to accept the control result.

**Readback:** Approve approval ownership, delegation rules, in-flight reassignment, minimum workforce fields and SoD/access controls. Record actual owners, timing, chosen pattern and remaining evidence; do not classify as Fit solely because an API exists.

## 8. Order-to-Cash / Sales workshop — WS03-O2C

**Purpose:** Workforce responsibility changes affecting customer-facing roles.  
**Invite:** Sales lead, sales operations SME, SD/workflow consultant, customer service representative, IAM, integration lead.  
**Bring:** Sales-role and coverage matrix; synthetic open transaction; territory/account ownership policy; workforce-to-target identifier sample; target role configuration.  
**Decision to secure:** Approve workforce versus customer-relationship ownership, target object, handover rules, access review and recovery.

| Question ID | Ask whom | Question to ask | Required answer / evidence |
|---|---|---|---|
| O2C-01 | Business | Which customer-facing roles require employee identity: sales employee, service owner, approver or account-team participant? | Role/use-case inventory |
| O2C-02 | Business | What happens to open orders, quotations, credit/discount approvals and customer cases when responsibility changes? | Continuity rules |
| O2C-03 | Business | Who approves customer/account reassignment, and can it differ from the HR reporting hierarchy? | Business responsibility authority |
| O2C-04 | Functional | Which actual target employee/workforce/business-partner object is needed, and which sales relationships remain target-owned? | Object boundary |
| O2C-05 | Functional | How are sales organization, distribution channel, division and territory determined? Are these target business assignments rather than EC organization fields? | Mapping without false equivalence |
| O2C-06 | Functional | How do leave, global assignment, concurrent employment and return-to-work affect coverage? | Lifecycle exception rules |
| O2C-07 | Integration | Does the target consume a common workforce feed or a separate integration? Who consumes the replicated identifier after delivery? | Actual consumer path |
| O2C-08 | Integration | How are future responsibility changes coordinated with employee effective dates and scheduled customer handovers? | Temporal orchestration |
| O2C-09 | Technical | How is person/employment identity matched without using email as an immutable key? How are email changes handled? | Identifier design |
| O2C-10 | Technical | Can a replay create duplicate partner/role relationships, and how are rejected assignments reconciled? | Idempotency and reconciliation |
| O2C-11 | SME | Who authorizes access to customer data and commercial approvals? Which permissions must remain separate from HR job titles? | Access and commercial control |
| O2C-12 | SME | What is the manual fallback if the responsible worker is unavailable but an energy customer requires urgent service? | Continuity and audit |

**Scenario walkthroughs:** Sales owner terminates with open orders; future territory transfer; email changes without duplicate identity; failed role assignment after successful worker load; temporary delegate expires. For each, ask the business user to explain the desired action, the functional consultant to demonstrate target standard, the integration expert to trace the message and the SME to accept the control result.

**Readback:** Approve workforce versus customer-relationship ownership, target object, handover rules, access review and recovery. Record actual owners, timing, chosen pattern and remaining evidence; do not classify as Fit solely because an API exists.

## 9. Manufacturing / Production workshop — WS04-MFG

**Purpose:** Worker assignment versus production and safety authorization.  
**Invite:** Production lead, plant scheduler, manufacturing/MES consultant, HSE, learning/qualification owner, Michael Torres as fictional site counterpart, IAM, integration lead.  
**Bring:** Plant/position/work-center mapping; synthetic shift and lifecycle records; qualification ownership; site access escalation; offline operating policy.  
**Decision to secure:** Approve EC/production/time/learning/HSE/IAM boundaries, offline behavior and independent safety authorization.

| Question ID | Ask whom | Question to ask | Required answer / evidence |
|---|---|---|---|
| MFG-01 | Business | Which shop-floor activities need workforce information: assignment, supervisor identification, labor confirmation or operator login? | Operational use cases |
| MFG-02 | Business | Which plant activities must stop or use an approved fallback when worker facts or qualification evidence are unavailable? | Safety/continuity rule |
| MFG-03 | Business | Which employee, agency worker and contractor populations operate at the plant, and who is authoritative for each? | Population and source ownership |
| MFG-04 | Functional | How do EC location, position and organizational assignment relate to plant, work center, shift and production resource? Which are separate objects? | Mapping and non-equivalences |
| MFG-05 | Functional | Who owns shifts, capacity, attendance and labor confirmations? Are any time/attendance solutions in scope separately from EC? | Scheduling/time boundary |
| MFG-06 | Functional | What happens to in-flight production work after transfer, termination or a backdated correction? | Transaction continuity |
| MFG-07 | Integration | Which actual ERP, MES, IAM and site-access systems need which attributes? Avoid assuming one EC feed serves every consumer. | Consumer-specific contracts |
| MFG-08 | Integration | How are effective changes sequenced against shift boundaries, local time zones and offline/edge systems? | Time and distribution rules |
| MFG-09 | Technical | How will messages distinguish HR employment status from operator account status and safety authorization? | Separate status semantics |
| MFG-10 | Technical | What detects stale local copies, failed site deliveries and partial acknowledgements across plants? | Monitoring and recovery |
| MFG-11 | SME | Who owns certification evidence, expiry and restricted-work permission? Can a position exist without current competence? | Qualification/safety authority |
| MFG-12 | SME | How is a safety-critical access revocation handled if the normal replication path is unavailable? Who verifies physical-site enforcement? | Emergency control and proof |

**Scenario walkthroughs:** Transfer across plants at shift change; certification expires while employment remains active; termination during interface outage; missing position qualification profile; delayed message reaches offline site. For each, ask the business user to explain the desired action, the functional consultant to demonstrate target standard, the integration expert to trace the message and the SME to accept the control result.

**Readback:** Approve EC/production/time/learning/HSE/IAM boundaries, offline behavior and independent safety authorization. Record actual owners, timing, chosen pattern and remaining evidence; do not classify as Fit solely because an API exists.

## 10. Warehouse Management workshop — WS05-WH

**Purpose:** Worker roles, location and access boundary.  
**Invite:** Warehouse lead, EWM or actual warehouse-system consultant, shift supervisor, resource/labor SME, RF administrator, HSE, IAM, integration lead.  
**Bring:** Warehouse target/version; resource/user/employee mapping; RF provisioning flow; warehouse assignment matrix; synthetic open tasks; equipment authorization policy.  
**Decision to secure:** Approve target object/resource ownership, RF/IAM path, warehouse mapping, open-task handoff and equipment authorization.

| Question ID | Ask whom | Question to ask | Required answer / evidence |
|---|---|---|---|
| WH-01 | Business | Which warehouse tasks need worker data: RF login, picking, packing, goods movement, supervision or labor reporting? | Task/population map |
| WH-02 | Business | What happens to open warehouse tasks and handling responsibilities when a worker leaves mid-shift? | Task reassignment policy |
| WH-03 | Business | Which contractors or temporary staff lack EC records, and what system owns their authoritative identity and end date? | Non-EC source boundary |
| WH-04 | Functional | Is the target embedded EWM, decentralized EWM or another WMS? Which release and landscape are actually deployed? | Target and deployment evidence |
| WH-05 | Functional | Are warehouse resource, RF user, business user and employee separate objects? Who creates and maps each? | Target object model |
| WH-06 | Functional | How do EC location and job relate to warehouse number, activity area, queue and resource group? Which assignments stay warehouse-owned? | Ownership and mapping |
| WH-07 | Integration | Can a common workforce/IAM integration support the need, or is a WMS-specific interface justified? | Reuse versus new interface |
| WH-08 | Integration | How are future transfers, concurrent work across warehouses and inactive records applied without dropping valid assignments? | Temporal/multiple-assignment rules |
| WH-09 | Technical | Who provisions RF/device access, and what happens when worker creation succeeds but resource or authorization creation fails? | Partial-failure control |
| WH-10 | Technical | How are stale sessions, shared devices and local caches handled on termination? What evidence shows target enforcement? | Session/access proof |
| WH-11 | SME | Who owns forklift/regulated-equipment qualifications and expiry? A job title or replicated employee record cannot alone grant equipment authority. | Competence boundary |
| WH-12 | SME | How can a supervisor safely reassign work during an outage without granting excessive access or losing audit history? | Operational fallback |

**Scenario walkthroughs:** Worker transfers warehouse with open tasks; RF account active after termination; valid employment but expired equipment qualification; duplicate replay creates no second resource; target outage at shift start. For each, ask the business user to explain the desired action, the functional consultant to demonstrate target standard, the integration expert to trace the message and the SME to accept the control result.

**Readback:** Approve target object/resource ownership, RF/IAM path, warehouse mapping, open-task handoff and equipment authorization. Record actual owners, timing, chosen pattern and remaining evidence; do not classify as Fit solely because an API exists.

## 11. Asset Management / Maintenance workshop — WS06-AM

**Purpose:** Maintenance-role assignments versus competence and work authorization.  
**Invite:** Maintenance lead, planner, PM/EAM consultant, permit-to-work/HSE owner, qualification owner, Michael Torres as fictional site counterpart, IAM, integration lead.  
**Bring:** Maintenance resource/work-center map; open-order examples; mobile/offline model; contractor source inventory; competence/permit policy; emergency escalation.  
**Decision to secure:** Approve maintenance resource model, qualification/permit authority, mobile recovery, contractor boundaries and transaction continuity.

| Question ID | Ask whom | Question to ask | Required answer / evidence |
|---|---|---|---|
| AM-01 | Business | Which maintenance activities need worker facts: planning, technician assignment, labor confirmation, contractor scheduling or approval? | Use-case and population inventory |
| AM-02 | Business | What happens to open maintenance orders and urgent breakdown work when a technician transfers or terminates? | Operational continuity |
| AM-03 | Business | Who is authoritative for contractor identity, engagement end date and site availability? | Contractor ownership |
| AM-04 | Functional | How do EC position/location relate to planner group, maintenance work center, plant and technician resource? Which target attributes are maintained locally? | Object mapping and responsibility |
| AM-05 | Functional | Does the system need employee identity only, or competence/availability from other sources? Do not infer competence from a position. | Consumer data needs |
| AM-06 | Functional | How are labor confirmations and financial postings handled after a retroactive employment change? | Historical transaction rule |
| AM-07 | Integration | Which targets consume the data: ERP EAM, mobile maintenance, scheduling, contractor platform or permit system? | Consumer inventory |
| AM-08 | Integration | What sequence ensures a worker exists before maintenance assignment, while qualification approval remains independently controlled? | Dependency and authorization sequence |
| AM-09 | Technical | How are mobile/offline caches invalidated and failed terminations escalated? | Offline access control |
| AM-10 | Technical | Which identifiers persist across rehire, contract renewal and multiple assignments without merging different people? | Identity lifecycle |
| AM-11 | SME | Who issues, suspends and revokes permit-to-work, electrical switching or confined-space authorization? Which evidence and expiry govern access? | Safety decision ownership |
| AM-12 | SME | Can an urgent maintenance exception proceed during integration failure? Who approves, logs and later reconciles it without bypassing safety gates? | Controlled emergency process |

**Scenario walkthroughs:** Terminated technician retains offline access; rehire with old identity; assignment without current qualification; transfer with open maintenance order; emergency repair during replication failure. For each, ask the business user to explain the desired action, the functional consultant to demonstrate target standard, the integration expert to trace the message and the SME to accept the control result.

**Readback:** Approve maintenance resource model, qualification/permit authority, mobile recovery, contractor boundaries and transaction continuity. Record actual owners, timing, chosen pattern and remaining evidence; do not classify as Fit solely because an API exists.

## 12. Shared object ownership and integration boundary worksheet

Starting hypotheses below are for validation, not approved design. One object can have different authoritative attributes; decide at attribute level.

| Data / responsibility | Proposed authority to validate | Consumer / direction to explore | Meeting decision |
|---|---|---|---|
| Employee person/employment facts | EC for approved in-scope populations | Workforce consumers, possibly through shared replication | Actual source/filter/keys TBD |
| Contractor facts | EC, contractor platform or other source — unconfirmed | IAM and operational consumers | Establish source by worker category |
| Cost-center master | Finance master-data owner | Finance → EC where applicable | Key, validity, package and source instance |
| Worker cost-center assignment | EC if approved design | EC → relevant target | Primary assignment versus distribution |
| Target employee/workforce/business-partner representation | Target functional owner | Supported workforce replication path if required | Target model and prerequisites |
| Accounts and business permissions | IAM + target authorization owners | HR facts inform controlled account/role processes | Grant/revoke workflow and evidence |
| Purchasing/sales responsibility | Respective business function | May consume workforce changes | Local responsibility rules and delegation |
| Production/work-center/warehouse/maintenance resource | Respective operational owner | Only required workforce facts consumed | No assumed 1:1 mapping from EC position |
| Competence evidence | Learning/qualification owner | HSE/operations where authorized | Qualification source, validity and correction |
| Permit/restricted-work authorization | Site HSE/permit owner | Operational enforcement | EC employment status alone is insufficient |

## 13. Interface contract and field-mapping templates

Complete one contract per real message flow. Several workshops may share one interface; one workshop may need multiple interfaces. Internal references IF-xx are project labels, not SAP Scope Item IDs.

| Contract attribute | Required answer | Accountable reviewer |
|---|---|---|
| Interface ID, name, process and consumer | Unique ID; module; business action; standard scope/process ID if verified | Solution Architect |
| Scope and population | Countries/entities; worker categories; exclusions; release | Business owner |
| Source/target and object | Actual systems, editions, releases and object models | Source/target leads |
| Authority and direction | Attribute owner; one-way/bidirectional; conflict precedence | Data owner |
| Trigger and extraction | Event/poll/batch; full/snapshot/delta; initial-load boundary | Integration lead |
| Keys and mapping | Person/employment/target keys; code crosswalk; validation | EC + target leads |
| Temporal behavior | Effective date, future slices, retro corrections, sequence/time zone | Business + functional leads |
| Dependency and ordering | Reference data; identity; grants; dependent target operations | Architect |
| Performance and timing | Normal/peak volume, latency, cutoff and recovery targets | Business + operations |
| Errors and reconciliation | Error classes; retries; duplicate prevention; business acknowledgement | Integration operations |
| Security and privacy | Authentication pattern, service permissions, field minimization, retention | Security/privacy owner |
| Delivery and acceptance | Environments, deployment owner, tests, sign-off and runbook | Customer IT + business |

| Field-map ID | Business meaning | Source object/field | Target object/field | Key / format / length | Effective-date rule | Mapping / default / null behavior | Validation / rejection | Owner | Evidence |
|---|---|---|---|---|---|---|---|---|---|
| MAP-01 | To complete from actual contract | TBD | TBD | TBD | TBD | No silent defaults; agree null versus unchanged | TBD | TBD | Synthetic source and target samples |

- [ ] Validate reference-data precedence and code mapping without stripping significant leading zeros.
- [ ] Define how field clearing differs from omitted/no-change fields.
- [ ] Document future records, corrected history, deleted/rescinded events and same-day multiple changes where applicable.
- [ ] Confirm target support for time slices before selecting an EC extraction mode.
- [ ] Establish idempotency using actual business keys/message semantics, not an assumed universal API feature.
- [ ] Test pagination, rate limits, retries, checkpoints and recoverability against the chosen API and volumes.
- [ ] Record technical receipt and business acceptance separately.
- [ ] Validate APIs and integration packages against actual deployment; do not assume CompoundEmployee, OData, events, MDI or a particular middleware is automatically the correct choice.

## 14. Cross-module test portfolio and acceptance evidence

These are proposed scenarios, not executed tests. Numeric SLAs and acceptable tolerances must be agreed; critical access/safety exceptions require explicit accountable decisions.

| Test | Trigger / edge case | Expected outcome to agree and prove | Business evidence / reviewer |
|---|---|---|---|
| INT-T01 | New hire references cost center not yet available | Dependency is visible; no silent default assignment; replay after approved correction | Worker/reference reconciliation; Finance + HR |
| INT-T02 | Future-dated transfer across entities/sites | Target applies at agreed effective time; relevant old/new responsibilities handled | Dated assignment and authorization evidence |
| INT-T03 | Backdated correction after posting/pay cutoff | Approved historic correction behavior; no uncontrolled rewrite of posted transactions | Finance/payroll exception approval |
| INT-T04 | Rehire with previous person identity | Existing person correctly linked; employment and target authorization handled separately | Identity crosswalk; HR + IAM |
| INT-T05 | Concurrent employments | Valid assignments preserved; one change does not disable unrelated active employment | Person/employment comparison |
| INT-T06 | Termination with open procurement/sales tasks | Account/access handling and business handover both complete per policy | Target work-item reassignment + access evidence |
| INT-T07 | Rescinded/future termination | Corrected event reaches target; reinstatement/grants follow approved review | Source history + target status |
| INT-T08 | Duplicate or out-of-order message | No duplicate person/resource or stale overwrite; exception visible | Message trace + target state |
| INT-T09 | Transport receipt succeeds, target rejects business data | Business rejection reported; record remains unresolved until corrected | Target rejection and owner ticket |
| INT-T10 | Missing/expired qualification | Employment may remain active; restricted work follows independent safety controls | Learning/HSE decision evidence |
| INT-T11 | Contractor not mastered in EC | Correct authoritative source drives lifecycle; record is not invented in EC | Contractor source/target crosswalk |
| INT-T12 | Outage across shift boundary/offline target | Agreed escalation/fallback; backlog replay reconciled; critical site access action verified | Operations/site log and recovery report |
| INT-T13 | Payload contains unnecessary sensitive fields | Mapping restricts fields and evidence/log exposure to approved purpose | Security/privacy review |
| INT-T14 | Full load followed by delta | No missing interval or double processing; source/accepted/rejected/pending population reconciles | Checkpoint and count/key report |
| INT-T15 | Cost-center deletion/blocking or manager removed | Consumers follow agreed business rules; unresolved relationships remain visible | Finance/workflow owner acceptance |

For each executed test record: contract/version, synthetic input, source effective date and change timestamp, expected result, actual result, correlation reference, target business result, pass/fail, defect, recovery evidence, reviewer and date. A successful middleware message does not prove warehouse login removal or a safe operational outcome.

## 15. Workshop capture, FtS decisions and Cloud ALM traceability

| Record ID | Workshop / question | Business need and evidence | Source → target / object | Classification | MoSCoW | Decision / alternative | Business approver | Delivery owner | Due date | Test / Cloud ALM link | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|
| OVE-INT-001 | TBD — populate during meeting | TBD — do not pre-approve | TBD | Pending assessment | TBD | TBD | TBD | TBD | TBD | TBD | Open |

Keep business requirement separate from chosen implementation. Follow the classification convention in the [existing plan](source-and-assumptions.md#10-classification-decision-tree): Fit, Partial Fit, Gap; apply Out of Scope/Deferred through explicit scope decisions. Unknown is pending assessment. Validate the actual EC-supported extension mechanism; S/4HANA Private Edition development is not an EC in-core option.

1. Link the requirement to the scoped process in SAP Cloud ALM where available.
2. Record question ID, source evidence, business outcome, actual source/target and named owner.
3. Record classification rationale, MoSCoW, dependencies and architecture decision.
4. Link approved work to delivery/configuration items, tests and defects using supported tenant capabilities.
5. Store additional metadata in governed descriptions/documents if not a native field.
6. Preserve the trace: source scene/question → requirement → interface contract → field mapping → delivery item → test → business acceptance.
7. Reconcile tracker and Cloud ALM; do not claim Cloud ALM has been updated by publishing this document.

**After each workshop**
- [ ] Publish proposed minutes within one business day and request factual corrections; this is a recommended project cadence.
- [ ] Name one accountable business approver and one delivery owner for every decision/action.
- [ ] Review unresolved source/target, identity, timing, security and safety questions before design approval.
- [ ] Mark assumptions, dissent and conditional acceptance visibly.
- [ ] PM schedules the design-readback date and escalation for overdue blocking decisions.

## 16. Ownership and escalation rules

| Decision / issue | Accountable role to appoint | EC consultant's responsibility | Escalate when |
|---|---|---|---|
| Business process fit and in-flight work | Relevant business process owner | Explain EC lifecycle facts; document requirement | No owner or conflicting required outcomes |
| EC data model/effective dating | EC design owner | Assess configuration and source-event behavior | Requirement contradicts agreed global model |
| Target object/transaction behavior | Target functional owner | Challenge unsupported field/object assumptions | No demonstrated target standard |
| Integration pattern and dependencies | Solution/integration architect | Supply EC constraints and mappings | Unsupported pattern or inconsistent contracts |
| Target account and access control | IAM/target authorization owner | Provide approved HR lifecycle facts | Revocation failure or excessive permissions |
| Qualifications and restricted work | HSE/permit/qualification owners | Preserve application responsibility boundaries | Safety-critical evidence or enforcement missing |
| Cutoff and finance/payroll reconciliation | Finance/payroll control owners | Confirm assignment history and source corrections | Pay/posting integrity affected |
| Scope, funding and schedule | PM/design authority under agreed governance | Present evidence, alternatives and dependencies | Unapproved build or cross-workstream commitment |

For critical site-access or safety failures, follow the approved operational incident route immediately; a workshop action log is not an emergency response mechanism. Names and response times remain TBD until appointed.

## 17. Personal meeting checklist for the EC consultant

**Before**
- [ ] Understand the business use case and target standard; prepare synthetic employee and reference records.
- [ ] Bring questions C01–15 and the relevant domain table; nominate a scribe.
- [ ] Confirm functional, business, integration, technical and SME attendance.
- [ ] Highlight pending evidence: actual system, target object, IDs, population, time behavior and decision authority.

**During**
- [ ] Start with business actions; ask the non-SF consultant to show the target process.
- [ ] Distinguish person, employment, login, resource and authorization.
- [ ] Walk through normal, future, retroactive, duplicate, failure and termination cases.
- [ ] Ask who confirms business completion; record the evidence, not only the proposed API.
- [ ] Read back ownership and conditions; avoid committing a date/effort before dependency assessment.

**After**
- [ ] Complete the contract, mapping and decision records.
- [ ] Reconcile shared feeds across all six areas; prevent duplicated interfaces and contradictory ownership.
- [ ] Obtain process, data, security, operational and architecture reviews as applicable.
- [ ] Baseline accepted decisions; schedule demonstrations/tests for unresolved assumptions.

## 18. Verified SAP references and how to use them

Links checked through SAP search on 7 November 2026; applicability depends on the actual product/release. These references support technical investigation, not an OmniVerse architecture selection.

| Reference | Workshop use |
|---|---|
| [Cost-center replication — SAP Cloud Integration configuration](https://help.sap.com/docs/SAP_SUCCESSFACTORS_EMPLOYEE_CENTRAL_INTEGRATION_TO_SAP_BUSINESS_SUITE/225ab53c0b2c4cb69345d34c2d96a18a/configuration-of-sap-cloud-integration-for-cost-center-replication) | Evaluate standard S/4HANA → EC cost-center content for the relevant landscape |
| [Replication of Cost Centers to Employee Central](https://help.sap.com/docs/successfactors-employee-central-integration-to-business-suite/replicating-cost-centers-from-sap-s-4hana-on-premise-to-employee-central/bb7e969144c5496a82d30b378fb13761.html) | Investigate business logic and lifecycle prerequisites for this documented scenario |
| [Workforce person replication considerations — SAP KBA 2813743](https://userapps.support.sap.com/sap/support/knowledge/en/2813743) | Ask which workforce integration channel applies to the actual S/4HANA Public Edition scope; do not generalize to other editions |
| [Introduction to the CompoundEmployee API](https://help.sap.com/docs/successfactors-employee-central/employee-central-compound-employee-api/introduction-to-compoundemployee-api?locale=en-US) | Understand employee-data extraction where this API is selected |
| [Effective-dated and period-based delta response](https://help.sap.com/docs/successfactors-employee-central/employee-central-compound-employee-api/query-response-for-effective-dated-and-period-based-delta-transmission) | Validate date/history expectations with the integration expert |
| [Period-based delta transmission](https://help.sap.com/docs/successfactors-employee-central/employee-central-compound-employee-api/period-based-delta-transmission-with-compoundemployee-api?locale=en-US) | Investigate consumers unable to process future time slices; confirm actual requirements |
| [SAP Cloud ALM implementation process](https://help.sap.com/docs/CloudALM/877c96cf971648b09ee0d0a64f7f4fef/8075da7928e64d96bd043b8e5f268adf.html) | Link workshop requirements to scoped processes and follow-on implementation evidence |

**Architecture alignment:** separate business decisions, data authority, application responsibility and integration transport; maintain traceability and evidence suitable for TOGAF/BABOK thinking, DAMA data stewardship and COBIT governance. This is educational alignment, not standards certification or a legal/compliance determination.
