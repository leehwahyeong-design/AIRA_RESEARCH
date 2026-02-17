# Security Pattern Library — Structural Patterns for Financial Infrastructure

**Scope:** Publicly known industry standards and structural patterns only. No internal architecture speculation, cryptographic implementation detail, key generation algorithms, or infrastructure deployment detail.

**Format per pattern:** Pattern Name | Purpose | Where it applies | Risk if missing | Common design mistake

---

## 1. Identity & Authentication

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Strong Identity Binding and Multi-Factor Authentication |
| **Purpose** | Ensure that access to the system is granted only to correctly identified parties, and that a single compromised factor (e.g. password) is insufficient to gain access. |
| **Where it applies** | All entry points where a human or system is identified and authenticated: user logins, API access, administrative interfaces, and system-to-system calls. |
| **Risk if missing** | Impersonation, account takeover, and unauthorized access to funds or sensitive data. Single-factor compromise leads to full access. |
| **Common design mistake** | Treating MFA as optional for high-privilege or high-value actions; reusing the same “second factor” across multiple systems so that one compromise affects all. |

---

## 2. Authorization & Role Segregation

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Least-Privilege and Segregation of Duties |
| **Purpose** | Limit what each identity can do to the minimum necessary for their role, and ensure that sensitive or high-impact actions require multiple distinct roles so no single party can complete them alone. |
| **Where it applies** | Access control layer for applications, APIs, administrative tools, and operational procedures. Applies to both human roles and system/service identities. |
| **Risk if missing** | Over-privileged users or services can abuse access; a single compromised role can authorize payments, change configuration, or exfiltrate data without a second checkpoint. |
| **Common design mistake** | Granting broad roles “for convenience”; combining approval and execution in one role; or leaving legacy roles in place when responsibilities change. |

---

## 3. Key Custody Concept

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Key Lifecycle Separation and Access Control |
| **Purpose** | Ensure that cryptographic material used to protect assets or data is created, stored, used, and retired under controlled conditions, with clear separation between who can use keys and who can destroy or rotate them. |
| **Where it applies** | Conceptual layer governing how keys are generated, stored, accessed, rotated, and revoked—not the algorithms, but the organizational and procedural boundaries. |
| **Risk if missing** | Key compromise or misuse; inability to revoke or rotate without operational impact; single point of failure if one party holds both use and recovery rights. |
| **Common design mistake** | Concentrating key creation, storage, and usage in one team or system; treating key backup and recovery as an afterthought; no clear ownership for key lifecycle. |

---

## 4. Ledger Integrity

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Immutability and Consistency of Financial Records |
| **Purpose** | Ensure that records of value movement and balances cannot be altered or deleted after acceptance, and that all participants see a consistent view of the same state at settlement. |
| **Where it applies** | Logical layer where transactions are recorded, committed, and made final—including ledgers, settlement systems, and any system that represents money or entitlements. |
| **Risk if missing** | Undetected tampering, double-spend, or reconciliation failures; disputes that cannot be resolved by a single source of truth; regulatory and audit findings. |
| **Common design mistake** | Allowing “corrections” that overwrite history instead of posting compensating entries; no clear definition of finality; weak or missing reconciliation against an authoritative ledger. |

---

## 5. Audit Logging

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Tamper-Evident, Complete, and Attributable Audit Trail |
| **Purpose** | Produce a durable record of who did what, when, and in what context, so that actions can be reconstructed for compliance, dispute resolution, and incident investigation. |
| **Where it applies** | All layers where security-relevant or business-critical actions occur: authentication, authorization decisions, transaction submission, configuration changes, and access to sensitive data. |
| **Risk if missing** | Inability to prove or disprove actions; failed audits; inability to attribute incidents or abuse to a specific identity or time window. |
| **Common design mistake** | Logging only success or only failure; allowing operators to alter or delete logs; missing correlation identifiers so that related events cannot be tied together. |

---

## 6. Deployment Control

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Controlled and Traceable Change Deployment |
| **Purpose** | Ensure that changes to software or configuration are introduced in a controlled way, with approval, traceability, and the ability to roll back, so that unauthorized or faulty changes do not go live. |
| **Where it applies** | Process and control layer governing how code and configuration move from development through testing to production—conceptual, not deployment tooling detail. |
| **Risk if missing** | Rogue or mistaken changes in production; no accountability for what was deployed when; inability to revert quickly after a bad release. |
| **Common design mistake** | Bypassing approval or testing for “urgent” changes; single person able to deploy without a second approval; no immutable record of what was deployed. |

---

## 7. Incident Detection

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Continuous Monitoring and Anomaly Awareness |
| **Purpose** | Detect deviations from expected behavior—whether technical, transactional, or behavioral—so that incidents and attacks can be identified and escalated in time to limit impact. |
| **Where it applies** | Observability and security monitoring layer: access patterns, transaction patterns, system health, and behavioral indicators across the platform. |
| **Risk if missing** | Delayed or missed detection of intrusions, fraud, or outages; reliance on external parties to report issues; inability to scope or contain an incident. |
| **Common design mistake** | Relying only on threshold alerts without behavioral or contextual signals; no clear ownership for triage and escalation; alerts that are ignored due to noise. |

---

## 8. Isolation & Kill-Switch Concept

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Blast-Radius Limitation and Emergency Circuit Breaker |
| **Purpose** | Limit the scope of any single component or credential so that a compromise or failure does not affect the entire system, and provide a controlled way to halt or isolate a subsystem in an emergency. |
| **Where it applies** | Conceptual design of boundaries between components, environments, and tenants; and the existence of procedures and controls to stop or isolate a part of the system without bringing down the whole. |
| **Risk if missing** | One compromise or failure cascades to the full platform; no way to stop a runaway process or isolate a compromised segment without a full outage. |
| **Common design mistake** | Shared credentials or trust across all components; no predefined kill-switch or isolation procedure; kill-switch that requires the same compromised path it is meant to stop. |

---

## 9. Data Retention & Evidence Preservation

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Retention by Obligation and Integrity of Preserved Data |
| **Purpose** | Retain data for the period required by law or policy, and ensure that preserved data is not altered or lost so it can serve as evidence in disputes, investigations, or regulatory requests. |
| **Where it applies** | Policy and control layer governing what data is retained, for how long, where it is stored, and who can access or delete it—applies to transactional, audit, and compliance data. |
| **Risk if missing** | Legal or regulatory non-compliance; inability to produce evidence when required; loss of evidence due to overwrite or deletion. |
| **Common design mistake** | Retaining data without a clear retention schedule; allowing operational deletion to override legal hold; no separation between operational access and evidence preservation. |

---

## 10. Supply Chain Security

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Trust and Integrity of Third-Party Components and Services |
| **Purpose** | Understand and manage the risk that external software, libraries, or services introduce, so that compromise or defect in a supplier does not become a critical vulnerability in the platform. |
| **Where it applies** | Conceptual layer covering selection, approval, and ongoing assurance of third-party code, services, and vendors that touch the financial or security boundary. |
| **Risk if missing** | Introduction of vulnerable or malicious components; dependency on a single supplier with no alternative; no visibility into what is in use or updated. |
| **Common design mistake** | Trusting “brand name” or convenience without verification; no process to track and update dependencies; critical functions depending on an unvetted or unmaintained component. |

---

## 11. Insider Threat Mitigation

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Detection and Limitation of Abuse by Trusted Parties |
| **Purpose** | Reduce the likelihood and impact of misuse by employees or partners who have legitimate access, through visibility, limits, and separation so that no single insider can unilaterally cause major harm. |
| **Where it applies** | Access control, monitoring, and procedural layer: who can access what, what is logged, how approvals work, and how anomalies in trusted-user behavior are treated. |
| **Risk if missing** | Theft, fraud, or sabotage by insiders; no early signal of misuse; over-reliance on trust without verification. |
| **Common design mistake** | Assuming insiders are fully trusted and not monitoring or constraining their actions; single person able to move funds or change critical configuration; no rotation or review of long-standing privileged access. |

---

## 12. Cross-System Trust Boundary

| Attribute | Description |
|-----------|-------------|
| **Pattern Name** | Explicit Trust Boundaries Between Systems and Domains |
| **Purpose** | Define where one system’s trust domain ends and another begins, and what assertions (e.g. identity, integrity) are required to cross that boundary, so that integration does not implicitly extend trust where it should not. |
| **Where it applies** | Conceptual boundary between internal subsystems, between the platform and partners, and between the platform and external users or networks—governing what is assumed vs. what is verified at the boundary. |
| **Risk if missing** | A compromised or malicious downstream system is trusted as if it were internal; credentials or data passed across boundaries without re-validation; unclear accountability when a breach occurs at the boundary. |
| **Common design mistake** | Treating “internal” and “external” as the only boundary and ignoring internal segmentation; accepting assertions from a partner without verifying; no clear contract for what each side must guarantee at the boundary. |

---

## Summary Matrix

| # | Pattern Area | Core Purpose (one line) |
|---|----------------|-------------------------|
| 1 | Identity & Authentication | Ensure access only for correctly identified parties with more than one factor. |
| 2 | Authorization & Role Segregation | Limit and split privileges so no single role can complete high-impact actions alone. |
| 3 | Key Custody Concept | Control key lifecycle and separate use from recovery/destruction. |
| 4 | Ledger Integrity | Keep financial records immutable and consistent as single source of truth. |
| 5 | Audit Logging | Maintain tamper-evident, complete, attributable record of actions. |
| 6 | Deployment Control | Introduce changes in a controlled, traceable, reversible way. |
| 7 | Incident Detection | Detect anomalies and security events in time to respond. |
| 8 | Isolation & Kill-Switch | Limit blast radius and enable emergency halt or isolation. |
| 9 | Data Retention & Evidence Preservation | Retain and preserve data for obligation and evidence. |
| 10 | Supply Chain Security | Manage risk from third-party components and services. |
| 11 | Insider Threat Mitigation | Detect and limit misuse by trusted parties. |
| 12 | Cross-System Trust Boundary | Define and enforce explicit trust at boundaries. |

---

All patterns are stated at a conceptual level. No implementation, cryptographic, or deployment instructions are implied.
