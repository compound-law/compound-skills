---
name: data-processing-agreement
description: 'Review framework for GDPR-compliant data processing agreements. Covers Art. 28 requirements, sub-processor management, and cross-border transfers.'
---


## Overview

This skill guides the review of data processing agreements (Auftragsverarbeitungsvertrage, AVV) under **Art. 28 GDPR**. Whenever a controller engages a processor to handle personal data on its behalf, a written DPA is mandatory (Art. 28 Abs. 3 GDPR). Failure to execute a compliant DPA constitutes an independent GDPR violation subject to fines up to EUR 10 million or 2% of global annual turnover (**Art. 83 Abs. 4 lit. a GDPR**). Use this skill when onboarding new vendors, auditing existing processor relationships, or reviewing DPAs presented by service providers. Key provisions include **Art. 28** (processor obligations), **Art. 32** (security of processing), **Art. 44-49** (international transfers), and **§ 62 BDSG** (additional German requirements for public bodies).

In practice, most DPAs are drafted by the processor and presented on a take-it-or-leave-it basis. The reviewing lawyer must identify non-negotiable mandatory content, flag deviations from GDPR requirements, and assess whether the overall allocation of risk and responsibility is acceptable for the controller client. German supervisory authorities -- particularly the state data protection commissioners (LfDI) and the Federal Commissioner (BfDI) -- have issued detailed guidance and have imposed fines specifically for defective DPAs.


## Systematic Review

### Step 1: Threshold Question -- Processor or Joint Controller?

Before reviewing the DPA, confirm that the relationship is actually one of controller-processor (Auftragsverarbeitung) rather than joint controllership (Art. 26 GDPR) or independent controllership.

- **Controller-processor test:** The processor acts solely on the controller's instructions and has no autonomous decision-making authority over the purposes and means of processing. If the processor determines its own purposes (e.g., using the data for product improvement, analytics, or its own marketing), the relationship may be one of independent or joint controllership.
- **Indicators of joint controllership (Art. 26 GDPR):** Both parties jointly determine the purposes and means of processing. The CJEU has adopted a broad interpretation (C-210/16, Wirtschaftsakademie Schleswig-Holstein; C-40/17, Fashion ID). In practice, platform providers, analytics services, and advertising networks often qualify as joint controllers rather than processors.
- **Consequence of misclassification:** If the relationship is misclassified as processing when it is in fact joint controllership, the DPA does not satisfy the Art. 26 requirement for a joint controller arrangement, and both parties are in breach.

**Flag as risk:**
- Processor uses controller's data for its own analytics, benchmarking, or AI training -- potential joint controller relationship
- No clear instruction framework -- the processor determines processing parameters autonomously
- Multi-party data flows where the roles are not clearly delineated (e.g., platform ecosystems)

### Step 2: Mandatory Content (Art. 28 Abs. 3 GDPR)

The DPA must specify the core parameters of the processing relationship and include all mandatory processor obligations. Any omission renders the DPA non-compliant.

- **Processing parameters (Art. 28 Abs. 3 S. 1):** The DPA must specify: (a) the subject-matter and duration of processing, (b) the nature and purpose of processing, (c) the type of personal data processed (e.g., name, email, health data, financial data), and (d) the categories of data subjects (e.g., employees, customers, website visitors). Vague descriptions like "personal data processed in connection with the services" are insufficient.
- **Processor obligations (Art. 28 Abs. 3 lit. a-h):**
  - **(a) Documented instructions:** Processing only on documented instructions from the controller. The processor must inform the controller if an instruction infringes the GDPR (Art. 28 Abs. 3 S. 3).
  - **(b) Confidentiality:** All persons authorised to process personal data must be subject to confidentiality obligations (contractual or statutory).
  - **(c) Security measures:** Implementation of appropriate technical and organisational measures under Art. 32 GDPR.
  - **(d) Sub-processing conditions:** Compliance with the sub-processor requirements of Art. 28 Abs. 2 and 4.
  - **(e) Data subject rights assistance:** The processor must assist the controller in responding to data subject requests (access, rectification, erasure, portability, restriction, objection).
  - **(f) Security and DPIA assistance:** Support the controller with obligations under Art. 32-36 (security, breach notification, data protection impact assessment).
  - **(g) Deletion or return:** At the controller's choice, delete or return all personal data after the end of the services, and delete existing copies unless EU or member state law requires retention.
  - **(h) Audit and inspection:** Make available to the controller all information necessary to demonstrate compliance and allow for and contribute to audits, including inspections by the controller or an auditor mandated by the controller.

**Flag as risk:**
- Any mandatory element from Art. 28 Abs. 3 lit. a-h missing entirely
- Processing purpose described in vague terms that could permit scope creep
- No obligation to process only on documented instructions -- this is the foundational element of the processor relationship
- Confidentiality obligation limited to "reasonable efforts" rather than a binding commitment
- No obligation to inform the controller if an instruction infringes the GDPR

### Step 3: Sub-Processor Management (Art. 28 Abs. 2, 4 GDPR)

The processor must not engage another processor (sub-processor) without prior authorization from the controller. Sub-processor management is one of the most contested areas in DPA negotiations.

- **Authorization model:** Two options exist -- (a) specific prior written authorization for each named sub-processor, or (b) general written authorization with a notification and objection mechanism.
- **Sub-processor list:** The processor should provide a current list of all sub-processors, including their names, locations, and the processing activities they perform. Many cloud providers maintain sub-processor lists on their websites -- verify that the DPA references this list and requires it to be kept up to date.
- **Change notification for general authorization:** Where general authorization is used, the processor must inform the controller of intended additions or replacements of sub-processors, giving the controller an opportunity to object. The notification period must be reasonable -- 14-30 days is market standard. Shorter periods (e.g., 7 days) or deemed-consent mechanisms (silence equals consent) are problematic.
- **Objection right and consequences:** If the controller objects, the processor should be required to either refrain from engaging the sub-processor or propose alternatives. If no resolution is reached, the controller should have a right to terminate the DPA (and the underlying services agreement) without penalty within a reasonable period. Clauses that make termination the controller's only remedy -- without any transition period or data migration support -- are one-sided.
- **Back-to-back obligations (Art. 28 Abs. 4 GDPR):** The processor must impose the same data protection obligations on sub-processors as contained in the DPA. This includes all substantive requirements: documented instructions, confidentiality, security, sub-sub-processing, data subject assistance, audit rights, and deletion/return.
- **Liability for sub-processor failures:** Under Art. 28 Abs. 4 S. 2 GDPR, the processor remains fully liable to the controller for the performance of the sub-processor's obligations. The DPA should not attempt to limit this statutory liability allocation.

**Flag as risk:**
- No sub-processor list provided or list is outdated
- Objection period shorter than 14 days or objection right is illusory (deemed consent if no objection)
- No back-to-back contract requirement for sub-processors
- Controller's only remedy upon objection is immediate contract termination with no transition period
- Processor disclaims liability for sub-processor failures despite Art. 28 Abs. 4 S. 2 GDPR

### Step 4: International Transfer Mechanisms (Art. 44-49 GDPR)

If personal data is transferred outside the EEA (to the processor, a sub-processor, or data storage infrastructure), verify the legal basis for each transfer.

- **Adequacy decision (Art. 45 GDPR):** Check whether the recipient country or territory has a valid adequacy decision. Current adequacy decisions include: Japan, South Korea, UK, Canada (commercial organizations), Argentina, Israel, New Zealand, Switzerland, Uruguay, and the US (under the EU-US Data Privacy Framework, DPF, adopted 10 July 2023).
- **Standard Contractual Clauses (SCCs):** The current SCCs were adopted by Commission Implementing Decision 2021/914. Confirm the correct module: **Module 2** (Controller-to-Processor) or **Module 3** (Processor-to-Sub-processor). Verify that **Annex I** (parties, data transfers, competent supervisory authority) and **Annex II** (technical and organisational measures) are fully completed with specific, factual details -- not placeholder text.
- **Transfer Impact Assessment (TIA):** Post-Schrems II (CJEU, C-311/18), parties relying on SCCs must assess whether the recipient country's legal framework provides essentially equivalent protection. The assessment must consider surveillance laws, access by public authorities, effective remedies, and the specific circumstances of the transfer. If the assessment reveals inadequate protection, supplementary measures (encryption, pseudonymization, split processing) must be implemented.
- **US transfers under the Data Privacy Framework:** The DPF adequacy decision (10 July 2023) covers transfers to US organizations that have self-certified under the DPF. Verify the recipient's active certification status at dataprivacyframework.gov. If the recipient is not certified, SCCs plus TIA remain necessary.
- **Binding Corporate Rules (Art. 47 GDPR):** An alternative for intra-group transfers, requiring approval by the lead supervisory authority in cooperation with other concerned authorities.

**Flag as risk:**
- Data transferred to a non-EEA country without any identified legal basis
- SCCs used but Annex I and Annex II details not completed or completed with generic text
- No TIA conducted despite transfer to a country without an adequacy decision
- US recipient not certified under the EU-US Data Privacy Framework despite reliance on the adequacy decision
- Sub-processor located in a third country not disclosed in the sub-processor list

### Step 5: Technical and Organisational Measures (Art. 32 GDPR)

The DPA should contain or reference specific TOMs appropriate to the risk level of the processing activities. German supervisory authorities have emphasised that generic, boilerplate TOMs do not satisfy the GDPR.

- **Pseudonymization and encryption (Art. 32 Abs. 1 lit. a):** Check for specific commitments: encryption at rest (AES-256 or equivalent), encryption in transit (TLS 1.2+), and pseudonymization of personal data where processing does not require direct identification.
- **Confidentiality, integrity, availability, resilience (Art. 32 Abs. 1 lit. b):** Measures must address: access controls (role-based, least privilege), network security (firewalls, intrusion detection), physical security of data centers, business continuity and disaster recovery, and data segregation between clients.
- **Regular testing (Art. 32 Abs. 1 lit. d):** Procedures for regularly testing, assessing, and evaluating the effectiveness of TOMs. This includes penetration testing, vulnerability scanning, security audits, and employee training.
- **Incident recovery (Art. 32 Abs. 1 lit. c):** Measures for rapid restoration of access to personal data after a physical or technical incident. Check for committed recovery time objectives (RTOs) and recovery point objectives (RPOs).
- **Level of specificity:** The TOMs must be specific enough to be verifiable. "Industry-standard security measures" or "appropriate technical measures" without further detail fail the Art. 32 requirement. Best practice: a separate annex with a structured breakdown by category (access control, cryptography, data center security, employee measures, incident response).

**Flag as risk:**
- TOMs are entirely generic or boilerplate, not reflecting actual processing activities
- No commitment to encryption at rest or in transit for sensitive data categories
- No procedure for regular security testing or penetration testing
- Recovery time and recovery point objectives not defined
- TOMs not updated since the original DPA execution despite changes in technology or threat landscape

### Step 6: Audit Rights (Art. 28 Abs. 3 lit. h GDPR)

The controller has a statutory right to audit the processor. This right cannot be waived, but its practical exercise is frequently restricted in processor-drafted DPAs.

- **Advance notice:** A reasonable advance notice period (14-30 days) is acceptable. Periods exceeding 30 days are excessive and may prevent timely audits.
- **Frequency:** Limitation to one routine audit per year is common and generally acceptable, provided the controller retains the right to additional audits for cause (e.g., following a data breach, supervisory authority inquiry, or credible complaint).
- **Auditor selection:** Clauses requiring the controller to use the processor's chosen auditor undermine independence. The controller should have the right to appoint its own auditor, subject to reasonable confidentiality commitments and non-compete restrictions (the auditor should not be a competitor of the processor).
- **Cost allocation:** Market practice varies. Processors frequently require the controller to bear audit costs. This is acceptable for routine audits, but if the audit reveals material non-compliance, costs should shift to the processor.
- **Acceptable alternatives:** Third-party certifications (ISO 27001, SOC 2 Type II) and standardised audit reports can supplement -- but not replace -- the controller's audit right. The DPA should allow the controller to accept such reports in lieu of a physical audit while preserving the right to conduct its own audit when circumstances require it.

**Flag as risk:**
- Audit right limited to reviewing the processor's self-certification or summary reports only
- No additional audit right in the event of a data breach or supervisory authority inquiry
- All audit costs borne by the controller regardless of audit findings
- Processor may refuse audit on "business confidentiality" grounds without adequate limitation
- Audit right effectively nullified through cumulative procedural restrictions

### Step 7: Data Breach Notification, Deletion, and Liability

Confirm the post-breach and post-termination obligations and assess the internal liability allocation.

- **Breach notification (Art. 33 Abs. 2 GDPR):** The processor must notify the controller of a personal data breach **without undue delay** after becoming aware of it. Check the specific notification timeline in the DPA -- "72 hours" mirrors the controller's obligation to the supervisory authority and is a reasonable processor commitment. Longer periods (e.g., "within 5 business days") may leave the controller unable to meet its own 72-hour deadline.
- **Content of breach notification:** The notification should include the nature of the breach, categories and approximate number of affected data subjects, likely consequences, and measures taken or proposed to address the breach.
- **Data return or deletion (Art. 28 Abs. 3 lit. g GDPR):** At the controller's choice upon termination, the processor must delete or return all personal data and delete existing copies. Written certification of deletion should be provided within a defined period (30 days is standard).
- **Retention after termination:** The processor may retain data beyond termination only to the extent required by EU or member state law. Processing for the processor's own purposes (analytics, product improvement) is prohibited.
- **Liability allocation (Art. 82 GDPR):** GDPR provides for joint and several liability toward data subjects. The internal allocation between controller and processor should be addressed in the DPA. Processors frequently seek to cap liability at the annual contract value or exclude consequential damages. Such caps may undermine the controller's ability to recover regulatory fines resulting from processor breaches.
- **Indemnification for regulatory fines:** German courts generally permit contractual indemnification for regulatory fines, but enforceability remains debated where the fine penalises the indemnified party's own negligence. Include a clear allocation: the processor should indemnify the controller for fines resulting from processor breaches; the controller bears fines resulting from its own compliance failures.

**Flag as risk:**
- No deletion obligation or no certification of deletion
- Breach notification timeline exceeds what is needed for the controller to meet its 72-hour obligation
- Processor retains data after termination for "analytics" or "product improvement"
- Processor liability capped at one month's fees, leaving the controller exposed to fines potentially reaching millions
- No provision for indemnification of regulatory fines caused by processor breach


## Special Scenarios

### SaaS Provider DPAs

SaaS DPAs are typically non-negotiable. Focus on:

- **Sub-processor proliferation:** Large SaaS providers may list dozens of sub-processors. Verify that the list is current and that the change notification mechanism provides genuine opportunity to object.
- **Data location:** Confirm whether data is stored exclusively within the EEA or also in third countries. "EU data residency" options may be available for an additional fee.
- **Encryption and access:** Verify whether the provider can access unencrypted customer data and under what circumstances. Bring-your-own-key (BYOK) or hold-your-own-key (HYOK) encryption may mitigate access risks.
- **Data portability on exit:** The DPA should guarantee data export in standard formats within a defined period after termination.

### Group-Internal DPAs

Intra-group processing (e.g., shared service centers, centralized HR systems) still requires a DPA. The GDPR does not provide a group privilege. Additional considerations:

- **Binding Corporate Rules** may serve as both the transfer mechanism and the processor compliance framework, but a separate DPA is still required.
- **Multiple controllers:** If several group entities share a processor, consider a multi-party DPA or ensure each entity has its own DPA reflecting its specific processing activities.

### German Public Sector (§ 62 BDSG)

Public bodies in Germany must comply with additional requirements under § 62 BDSG, which supplements Art. 28 GDPR with specific provisions for the public sector. These include enhanced documentation obligations and stricter requirements for processing within the scope of Directive (EU) 2016/680 (law enforcement data protection).


## Limitations of This Skill

This skill provides a structured preliminary assessment. In the following cases, engaging a lawyer is necessary:

- **Negotiation of DPA terms** with major cloud providers or SaaS vendors, particularly where the standard DPA is materially deficient
- **Transfer impact assessments** requiring analysis of third-country surveillance laws and supplementary measures
- **Data breach response** where the processor's breach creates controller notification obligations under Art. 33/34 GDPR
- **Supervisory authority proceedings** or audits targeting the processor relationship
- **Complex multi-party processing structures** involving joint controllers, multiple processors, and sub-processors across jurisdictions
- **Sector-specific requirements** for financial services (BaFin guidance on outsourcing, MaRisk AT 9), healthcare (§ 203 StGB professional secrecy), or telecommunications (§ 3 TTDSG)

Compound is happy to assist with the review, negotiation, and drafting of DPAs that meet GDPR and BDSG requirements.
