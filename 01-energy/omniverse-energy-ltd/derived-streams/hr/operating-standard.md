# HR operating and learning standard

**OVE-HR-STD01 · Proposed educational design · 2026-10-19.** Inherits [enterprise case standard](../../../../standards/master-case-study-standard.md). Six themes cover all 22 master sections through linked enterprise context; domain cases do not recreate enterprise facts.

## Distinct architecture responsibilities
| View | Owns in the HR case | Does not own |
|---|---|---|
| Enterprise | Strategy, portfolio alignment, governance | Domain configuration |
| Business | Capabilities, value stages, decision rights | Message transport |
| Data | Meaning, source ownership, quality, retention, lineage | User journey layout |
| Application | Service and record responsibilities | Interface implementation |
| Technology | Platform/runtime standards | Physical capacity topology |
| AI | Grounding, evaluations, human oversight, model lifecycle | Unapproved employment decisions |
| Security | Identity controls, privacy enforcement, trust boundaries | Domain eligibility policy |
| UI/UX | Inclusive journeys, accessibility, low-connectivity patterns | Authoritative employment status |
| Infrastructure | Availability, capacity, networks, recovery environments | Business process ownership |
| Integration | Contracts, event order, retries, acknowledgements, reconciliation | Conflicting master-data decisions |
| Domain | Eligibility, proration, effective dating, pay/time/talent rules | Enterprise-wide platform selection |
| Industry | Energy roles, critical skills, operations and HSE context | Country legal sign-off |

These are ownership boundaries with governed interfaces, not a claim that real architecture concerns never intersect.

## Shared contracts and safety
Employment record ≠ account ≠ badge ≠ competence ≠ permit to work. HR status changes trigger governed requests; operations/HSE retain authorization for restricted work. No cloud HR recommendation directly commands plant controls.

Each event contract records source owner, event ID, employment/person ID, effective time, version, correlation ID, allowed fields, target acknowledgement and reconciliation outcome. Handle duplicate delivery, out-of-order events, rehires, backdated changes, dead letters and replay. Numeric latency/SLA requires criticality and measured evidence; no universal five-minute guarantee.

Benefits example: approved life event → eligibility/effective-date validation → authorized benefit change → country payroll input → acknowledgement → employee/amount reconciliation. Test post-cutoff and backdated cases; agree correction/retro treatment and communicate timing. No unverified standard SAP latency or proration behavior is asserted.

## Standards crosswalk and limits
| Reference | Artifact use | Evidence status |
|---|---|---|
| TOGAF / ArchiMate | Linked architecture views, decisions and roadmap | Public Open Group guide index checked; no proprietary content reproduced |
| BIZBOK | Distinguish abilities, stages and stakeholders | Conceptual mapping inherited from master; not clause-level validation |
| IIBA BABOK / Business Analysis Standard | Need-to-requirement-to-test traceability | Public standard page checked |
| DAMA-DMBOK | Data owner, quality, lineage and stewardship | Conceptual mapping, not certification |
| COBIT | Decision accountability and assurance gates | Conceptual mapping, not assessment |
| ISO/IEC security, quality and AI standards | Control/evidence backlog for qualified review | No clause conformity or jurisdictional compliance asserted |
| NIST AI RMF | Govern, Map, Measure, Manage in HR11 | Public framework checked |

Public references checked 2026-10-19: [Open Group guides](https://www.opengroup.org/togaf/series-guides), [IIBA requirements/designs](https://www.iiba.org/knowledgehub/the-business-analysis-standard/4-implementing-business-analysis/4-4-understanding-requirements-and-designs/), [NIST AI RMF core](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/). These inform original learning designs; they do not validate software feature availability, local law or production compliance.

## Living learning loop
Use the six-stage discovery-to-outcome pathway in each case. Start with a real question, role-play conflicting needs, model only what helps the decision, run a reversible synthetic experiment, inspect evidence, and repeat. A failed hypothesis is a useful learning result. Score artifacts for reasoning and traceability, not quantity of slides or tool features.
