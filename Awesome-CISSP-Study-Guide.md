# CISSP Study Guide

*Managerial Concepts • Risk Management • Governance • Security Models*

A consolidated resource covering the managerial mindset, risk and governance frameworks, legal and regulatory requirements, security controls, asset security, and the formal security models.

## Contents

| № | Section | What It Covers |
| :---: | :---- | :---- |
| **01** | The CISSP Manager Mindset | Priorities, accountability vs. responsibility, due care and due diligence |
| **02** | Test-Taking Vocabulary | Golden words to favor and brown words to avoid |
| **03** | Security and Risk Management (Domain 1) | CIA triad, risk formula and responses, quantitative metrics, NIST RMF |
| **04** | Governance and Documentation Hierarchy | Policies, standards, baselines, procedures, guidelines |
| **05** | Legal, Regulatory, and Privacy Requirements | GDPR, the regulation table, Privacy Shield, intellectual property, ethics |
| **06** | Security Control Categories | Control types and functional classifications |
| **07** | Asset Security (Domain 2) | Data roles, classification, sanitization, transit security |
| **08** | Formal Security Models | Bell-LaPadula, Biba, Clark-Wilson |
| **09** | Exam Specifics | Computerized Adaptive Testing and official references |

## 01 — The CISSP Manager Mindset

Security is a business enabler, not just a technical constraint. Senior management and the Board of Directors are ultimately accountable and responsible for the organization's security posture.

> **★ Key Tip**
> Watch [Why you will pass the CISSP](https://www.youtube.com/watch?v=v2Y6Zog8h2A) numerous times as you begin your study, throughout your study, and especially before the exam. I watched the old and new version, [How to Pass the CISSP Exam Like a Pro: Your Complete Strategy Guide | Destination Certification](https://www.youtube.com/watch?v=gKe88tIeVYo&t=7s), at least 10 times in the 48 hours leading up to my exam.

### Priorities

- **Business First:** Business goals and objectives win.
  - If a question or situation asks for the primary driver of security, look for Business Strategy, Business Goals, or Business Objectives in the answer and in real life.
- **Law vs. Business:** In any conflict between legal requirements and business interests, the law always wins.

### Accountability vs. Responsibility

| Concept | Who Holds It | Key Rule |
| :---- | :---- | :---- |
| **Accountability** | Senior management, who must provide the resources and authority for security. | Always singular. |
| **Responsibility** | Individuals, held to account for their actions through training and sign-offs. | Can be many. |

### The "Reasonable Man" Standard

Security professionals must exercise both:

| Standard | Definition |
| :---- | :---- |
| **Due Care** | Acting as a reasonable person would in a similar situation — the reasonable person standard. Before the event/decision. |
| **Due Diligence** | Evaluating risks and doing the thing. A specific form of due care; the assigned individual completes the task in an accurate and timely manner. After the event/decision. |

## 02 — Test-Taking Vocabulary: Golden and Brown Words

Success on the CISSP exam often depends on identifying the "managerial" answer. Use the following vocabulary guide to evaluate options.

| Category | ★ Words to Favor ("Golden Words") | ✕ Words to Avoid ("Brown Words") |
| :---- | :---- | :---- |
| **Business Focus** | Business Strategy, Business Goals, Impact, Organization | IT, Peer, Certification/Accreditation |
| **Risk Focus** | Risk, Business Risk, Acceptable, Appropriate | Eliminate (risk can't be eliminated), Reject or Ignore Risk |
| **Process** | Change Management, Documentation | Always/Everyone (absolutes are usually wrong) |
| **Responsibility** | Accountability, Classification, Senior Management | International security standards (rarely the answer) |

> **★ Key Tips**
> If a specific word in a question is used in only one of the provided answers, pay close attention to that answer. If all the answers represent a technical, or fix it response, and one doesn't, pay close attention to that answer.

## 03 — Security and Risk Management (Domain 1)

### The CIA Triad

| Pillar | What It Preserves |
| :---- | :---- |
| **Confidentiality** | Preventing unauthorized access to systems and information. |
| **Integrity** | Preventing unauthorized modification of information. Mnemonic: the "I" in the Biba model stands for Integrity (see Section 08). |
| **Availability** | Ensuring systems and data are accessible. |

### Risk Management Frameworks and Processes

Risk is defined by the formula:

> **Risk = Threat × Vulnerability × Likelihood**

| Term | Definition |
| :---- | :---- |
| **Vulnerability** | A weakness in an asset — defined strictly. |
| **Threat** | A potential danger that might exploit a vulnerability. |
| **Risk (Inherent, Total)** | The risk level before any controls or safeguards are applied. |
| **Residual Risk** | The risk remaining after countermeasures are implemented. |

**The Four Risk Responses**

| | Response | What It Means |
| :---: | :---- | :---- |
| ▼ | **Mitigate** | Implement cost-effective controls. |
| ✓ | **Accept** | Live with the risk (requires a cost-benefit analysis; do not spend $100k to protect a $50k asset). |
| → | **Transfer** | Shift risk to a third party (e.g., insurance). |
| ✕ | **Avoid** | Stop the activity causing the risk. |

> **✕ Not a Valid Response**
> Never Reject or Ignore risk. Risk can never be entirely eliminated — only mitigated, accepted, transferred, or avoided.

**Quantitative Risk Assessment Metrics**

| Term | Meaning | Formula |
| :---: | :---- | :---: |
| **AV** | Asset Value — the dollar value of the resource. | — |
| **EF** | Exposure Factor — the percentage of asset value lost when a threat occurs. | — |
| **SLE** | Single Loss Expectancy — the cost of one loss. | AV × EF |
| **ARO** | Annualized Rate of Occurrence — how many losses occur per year. | — |
| **ALE** | Annual Loss Expectancy — the cost of losses per year. | SLE × ARO |

> **★ Exam Tip**
> Work the chain in order: AV × EF = SLE, then SLE × ARO = ALE. SLE is the cost of a single loss; ALE is the cost per year. Know how to work an example of this confidently.

**NIST Risk Management Framework (RMF)**

The process follows the **PCSIAAM** mnemonic:

1. **Prepare:** Initialize the risk management process.
2. **Categorize:** Determine the sensitivity of the information system.
3. **Select:** Choose the initial set of baseline security controls.
4. **Implement:** Document and deploy the controls.
5. **Assess:** Verify that controls are operating correctly.
6. **Authorize:** Senior management accepts the risk and allows operations.
7. **Monitor:** Continuously track control effectiveness.

## 04 — Governance and Documentation Hierarchy

Documentation must be binding and structured to provide clear direction to the organization.

| Document Type | Mandatory? | Description |
| :---- | :---: | :---- |
| **Policy** | Yes | High-level, broad statements of intent. They **never** contain technical specifications. |
| **Standards** | Yes | Compulsory rules that dictate specific hardware or software usage. These **do** contain technical specs. |
| **Baselines** | Yes | The minimum level of security required across the organization. |
| **Procedures** | Yes | Step-by-step actions for performing specific tasks. |
| **Guidelines** | No | Non-binding recommendations or operational guides. |

## 05 — Legal, Regulatory, and Privacy Requirements

### GDPR (General Data Protection Regulation)

Key principles for protecting personal data:

- **Lawful Processing:** Data must be processed legally.
- **Right to be Informed:** Organizations must identify themselves and explain why they need the data.
- **Right to Access/Rectification:** Users can see their data and must be allowed to correct it.
- **Right to Erasure:** Also known as the "Right to be Forgotten."
- **Data Portability:** Consumers can request a copy of their data.
- **Breach Notification:** Mandatory notification within **72 hours**.

> **✕ Superseded**
> Privacy Shield is no longer valid.

### Regulations, Laws, and Standards

Know what each regulation covers — and know what is **not** a law.

| Regulation | What It Covers | Status |
| :---- | :---- | :---: |
| **GLBA** | Consumer financial information. | Law |
| **HIPAA** | PHI. Three covered entities — providers, clearinghouses, and insurance plans — plus their business associates. | Law |
| **SOX** | Publicly traded company financial reporting. | Law |
| **FERPA** | Student education records. | Law |
| **FISMA** | Government contractors. | Law |
| **GISRA** | Precursor to FISMA. Expired November 2002. | Law |
| **PCI DSS** | Payment card information. | **NOT a law** |
| **Economic Espionage Act** | Trade secrets. | Law |
| **Lanham Act** | Trademark protection. | Law |
| **Glass-Steagall Act** | Banking. A common red herring. | Law |

> **★ Exam Notes**
> PCI DSS is a contractual industry standard, not a law. Glass-Steagall pops up as a red herring in practice exams — it concerns banking, not information security. GISRA came before FISMA and expired in November 2002.

### Intellectual Property

| Protection | What It Protects | Remember As |
| :---- | :---- | :---- |
| **Copyright** | Protects "original works of authorship" — creative works, including software code. | Creative works |
| **Trademark** | Protects unique designs, names, or symbols. Internationally protected. | Names, logos, symbols |
| **Patent** | Protects tangible inventions. | Inventions |
| **Trade Secrets** | Confidential business information (e.g., recipes). Protected indefinitely as long as it remains secret — internal only. | Internal confidentiality |

### ISC2 Code of Ethics

In cases of conflict, follow these canons in strict order of priority. Who may bring a complaint differs by canon.

| Canon | Canon Text | Who May File a Complaint |
| :---: | :---- | :---- |
| **I** | Protect society, the commonwealth, and the infrastructure. | Anyone |
| **II** | Act honorably, honestly, justly, responsibly, and legally. | Anyone |
| **III** | Provide diligent and competent services to principals. | Only an employer or contractor |
| **IV** | Advance and protect the profession. | Any certified or licensed professional |

## 06 — Security Control Categories

Controls are classified by how they are implemented and the function they perform.

### Common Control Types

| | Control Type | Function |
| :---: | :---- | :---- |
| ≡ | **Directive** | Instructions on rules of behavior (e.g., policy). |
| ⚑ | **Deterrent** | Discouraging policy violations (e.g., warning signs). |
| ■ | **Preventative** | Proactively stopping unwanted activity (e.g., locks). |
| ❖ | **Compensating** | Making up for a deficiency in another control. |
| ✹ | **Detective** | Discovering and alerting on unwanted activity after it occurs. |
| ✎ | **Corrective** | Fixing a problem post-incident. |
| ↻ | **Recovery** | Restoring conditions to normal (e.g., Disaster Recovery Plan). |

### Functional Classifications

| | Classification | Scope |
| :---: | :---- | :---- |
| ≡ | **Administrative** | Management-oriented (policies, background checks, training). |
| ⌂ | **Physical** | Facility protection (locks, lights, alarms). |
| ◆ | **Logical/Technical** | Digital restrictions (access controls, encryption). |
| § | **Regulatory** | Mandated by law. |

## 07 — Asset Security (Domain 2)

### Roles and Responsibilities

| Role | Typically | Duty |
| :---- | :---- | :---- |
| **Data Owner** | Senior management | Accountable for data protection and classification. |
| **Data Custodian** | An administrator | Responsible for implementing and maintaining the controls set by the Data Owner. |
| **Data Processor** | Users or entities | Access and process the data. |

### Data Life Cycle and Protection

- **Classification:** Data must be located and labeled properly based on "need to know."
- **Retention:** Policies must define minimum and maximum periods for data storage.

**Sanitization — Increasing Severity**

| | Method | What It Does |
| :---: | :---- | :---- |
| ● | **Clearing** | Non-invasive data removal (deletion/rewriting). |
| ●● | **Purging** | Rendering data recovery infeasible (e.g., degaussing, overwriting 7 times). |
| ●●● | **Destruction** | Physical shredding, chemical treatment, or incineration. |

**Transit Security**

| Method | Behavior |
| :---- | :---- |
| **Link Encryption** | Performed by service providers; encrypts routing data but may expose data at nodes. |
| **End-to-End Encryption** | Performed by the user (e.g., SSL/TLS, IPSec); routing data remains unencrypted. |

## 08 — Formal Security Models

| | Model | Protects | Rules |
| :---: | :---- | :---- | :---- |
| ★ | **Bell-LaPadula** | Confidentiality | **Simple Property:** No read up. **Star (\*) Security Property:** No write down. |
| ◆ | **Biba** | Integrity | **Simple Integrity Axiom:** No read down. **Star (\*) Integrity Axiom:** No write up. |
| ❖ | **Clark-Wilson** | Integrity | Access is granted through programs, never directly to the data. Enforced by the access control triple. |

> **↻ Mirror Image**
> Bell-LaPadula and Biba are opposites. Bell-LaPadula protects confidentiality (no read up, no write down — keeping secrets from leaking downward). Biba protects integrity (no read down, no write up — keeping bad data from corrupting upward).

### Clark-Wilson Access Control Triple

Under Clark-Wilson, a user never touches the data directly. Access runs through a program.

**User → Transformation Procedure → Constrained Data Item**

- **User:** the subject requesting access.
- **Transformation Procedure:** the program through which access is performed.
- **Constrained Data Item:** the protected data the procedure acts on.

## 09 — Exam

The CISSP exam uses Computerized Adaptive Testing (CAT) and will stop anytime between after question 100, and question 150.

> **→ Official References**
> - [https://www.isc2.org/exams/before-your-exam#heading-2](https://www.isc2.org/exams/before-your-exam#heading-2)
> - [https://www.isc2.org/register-for-exam/exam-scoring-faqs](https://www.isc2.org/register-for-exam/exam-scoring-faqs)

> **★ Tips**
> - Write the risk management formulas down on your scratchpad as soon as you accept the ISC2 NDA.
> - Write other quick tips to yourself that you are worried you will forget once the questions start.
> - Understand risk management frameworks, and processes. If only time for one - study the high level processes of the NIST RMF.
