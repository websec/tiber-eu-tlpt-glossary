# TIBER-EU / TLPT Glossary and Team Structure

This document summarizes the terms and team setup required to run a Threat-Led Penetration Test (TLPT) or Red Teaming exercise under the **TIBER-EU Framework**.

## Glossary of Terms

### Core concepts
- **TIBER-EU**: Threat Intelligence-Based Ethical Red Teaming. A uniform, high-quality standard for intelligence-led red team tests on live production systems.  
- **TLPT**: Threat-Led Penetration Test. TLPT requirements are implemented using the TIBER-EU testing process so entities can meet DORA TLPT obligations in a controlled way.  
- **CIF**: Critical or Important Function. Functions and supporting ICT systems that form the scope for testing.  
- **Flag**: Concrete target to be reached in a scenario.  
- **Leg-up**: Pre-agreed assistance from the Control Team to the Red Team to enable progress when needed.  
- **Scenario-X**: Optional scenario in the TTIR set, in addition to scenarios covering availability, integrity, and confidentiality.  
- **TTP**: Tactics, Techniques and Procedures.  
- **TI**: Threat Intelligence.  
- **OSINT**: Open-Source Intelligence.  
- **HUMINT**: Human Intelligence.  
- **Codename**: Required pseudonym for the entity used in documentation and multi-party communications.

### Teams and stakeholders
- **TCT**: TIBER Cyber Team. Authority team that implements and facilitates TIBER, trains Test Managers, and helps ensure a uniform, high-quality test.  
- **TM**: Test Manager. Member of the TCT assigned to your test. Validates deliverables, ensures compliance, and can invalidate a test for recognition if mandatory requirements are not met.  
- **CT**: Control Team. Small, trusted internal group that governs the test end-to-end, manages risk, coordinates with TM, TIP, and RTT, and can halt the test if needed.  
- **CTL**: Control Team Lead. Accountable lead for scope, scenarios, risk controls, approvals, and coordination.  
- **BT**: Blue Team. All staff and relevant third parties not in the CT and unaware of the test during preparation and active testing.  
- **TIP**: Threat Intelligence Provider. **External** provider that delivers the Targeted Threat Intelligence Report and scenarios, and works with RTT.  
- **RTT**: Red Team Testers. Execute the attack scenarios and produce the Red Team Test Report. **External preferred**. Internal RTT only in exceptional cases and only with TM approval.  
- **CSP**: Critical Service Provider. Third-party ICT or other critical provider that may be in scope.  
- **TKC**: TIBER-EU Knowledge Centre. ECB hub that supports TIBER implementations and training.

### Key deliverables
- **SSD**: Scope Specification Document. CIFs, supporting systems, and preliminary flags.  
- **GTL**: Generic Threat Landscape. Sector-level threat landscape that complements TTIR. Recommended, not mandatory.  
- **TTIR**: Targeted Threat Intelligence Report. Entity-tailored threat landscape and selected scenarios. Must include at least three end-to-end scenarios that cover availability, integrity, and confidentiality, and may include an optional Scenario-X.  
- **RTTP**: Red Team Test Plan. Communication and reporting, allowed and forbidden TTPs, risk controls, scenarios, detailed attack paths with expected leg-ups, and schedule for in, through, out phases.  
- **RTTR**: Red Team Test Report. Issued by RTT at the end of the test.  
- **BTTR**: Blue Team Test Report. BT maps its actions alongside RTT’s timeline using the RTTR.  
- **TSR**: Test Summary Report. Produced by the entity and shared with the authority.  
- **Attestation**: Issued by the authority to validate the true and fair conduct of the test for recognition.

## Team structure

| Team | Full name | What it is | Composition | Internal or external | Responsibilities | Primary deliverables |
|---|---|---|---|---|---|---|
| **TCT** | TIBER Cyber Team | Authority team that implements and facilitates TIBER and trains TMs | Authority staff, includes TMs and subject matter experts | External (authority) | Maintain implementation, facilitate tests, liaise with other TCTs and TKC | Attestation process support |
| **TM** | Test Manager | Authority representative assigned to the test | TM plus alternate from TCT | External (authority) | Validate deliverables, ensure the test follows mandatory requirements, escalate when needed, can invalidate recognition | Validations leading to Attestation |
| **CT** | Control Team | Governs the test and manages risk | Select, trusted internal members with escalation authority | Internal | Plan and manage end-to-end test, define scope and flags, procure TIP and RTT, manage risk, approve leg-ups, can halt the test | SSD, Initiation docs, Risk Management Doc, TSR |
| **CTL** | Control Team Lead | Accountable head of the CT | Senior manager | Internal | Finalize scope and scenarios, coordinate TIP and RTT and authorities, keep management informed, maintain secrecy | SSD sign-off, Initiation docs |
| **BT** | Blue Team | Regular defensive staff and relevant third parties not in the CT | SOC, IT, operations, CSP staff as applicable | Internal (unaware during test) | Defend as usual without prior knowledge, later participate in replay and Purple Teaming, produce BTTR | BTTR |
| **TIP** | Threat Intelligence Provider | Delivers entity-tailored threat intelligence and scenarios | External provider | External (mandatory) | Collect and analyze TI, produce TTIR, collaborate with RTT throughout testing | TTIR |
| **RTT** | Red Team Testers | Execute attack scenarios and report results | External team, internal only with TM approval | External preferred | Create RTTP, execute scenarios aiming to reach flags, report RTTR | RTTP, RTTR |
| **CSP** | Critical Service Provider | Critical third-party provider in scope | Third-party | External | Provide input for scope, may be included in testing where applicable | Input to SSD |
| **TKC** | TIBER-EU Knowledge Centre | ECB knowledge hub | ECB experts | External | Training for authorities and TMs, best practices, coordination | Guidance and training materials |

## Key rules under TIBER-EU

- **Only the CT is informed about the test details and timings. The BT remains unaware during preparation and active testing.**  
- **Use a codename for the entity in documentation and multi-party communications.**  
- **TIP must be external. RTT should be external. Internal RTT is only allowed in exceptional cases with prior TM approval and must meet the same standards.**  
- **Active red-teaming allocates a minimum of 12 weeks for the testing step so all attack phases can be executed and flags reached.**  
- **Mandatory end-phase activities**: Replay on production where possible, Purple Teaming, 360-degree feedback, remediation plan, TSR to authority, and Attestation by the authority.  

## Process snapshot

1. **Preparation**: Notification, initiation, scoping, procurement. Produce Initiation docs and SSD.  
2. **Threat Intelligence**: TIP produces TTIR with selected scenarios that cover availability, integrity, confidentiality, optionally Scenario-X.  
3. **Red Team testing**: RTT produces RTTP and executes active testing to reach flags.  
4. **Closure**: RTT issues RTTR. BT prepares BTTR from RTTR. Replay and Purple Teaming occur. Entity produces remediation plan and TSR. Authority issues Attestation.
