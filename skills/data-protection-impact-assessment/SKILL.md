---
name: data-protection-impact-assessment
description: 'When a DPIA is mandatory under Art. 35 GDPR, how to conduct and document one — with a structured assessment framework for Germany.'
---


A **Data Protection Impact Assessment** (DPIA, German: *Datenschutz-Folgenabschätzung*, DSFA) is a mandatory review under **Art. 35 GDPR** when a processing operation is likely to result in a high risk to the rights and freedoms of natural persons. The DPIA must be completed **before the processing begins** — not retrospectively. Failing to carry out a required DPIA is itself a standalone GDPR violation, subject to fines of up to **EUR 10 million or 2% of global annual turnover** under Art. 83(4)(a) GDPR.

This skill guides the systematic conduct and documentation of a DPIA. It applies to both new processing operations and material changes to existing systems — in particular AI-driven processes, biometric data, video surveillance, profiling, and employee data. For AI systems classified as high-risk under the **EU AI Act**, the DPIA under Art. 35 GDPR must be carried out separately from, but may be jointly documented with, the Fundamental Rights Impact Assessment (FRIA) under **Art. 27 AI Act** (→ [AI Act Compliance Check](/en-DE/skills/ai-act-compliance/)).


## Overview

This skill provides a structured assessment framework for the Data Protection Impact Assessment under Art. 35 GDPR. The key legal provisions are **Art. 35** (DPIA obligation), **Art. 36** (prior consultation when high residual risk remains), **Art. 5** (data protection principles: purpose limitation, data minimisation, storage limitation), **Art. 25** (data protection by design and by default), and **BDSG § 67** for specific processing situations in the German public sector. The appointed Data Protection Officer (DPO), if one exists, must be consulted in every case under Art. 35(2) GDPR.

A DPIA is not a one-time document — it is a **living process**. Material changes to the processing or its context require an update. German supervisory authorities, including the Federal Commissioner for Data Protection and Freedom of Information (BfDI) and the state commissioners (Landesbeauftragte für Datenschutz, LfDI), can request DPIA documentation at any time.


## Systematic Assessment

### Step 1: Is a DPIA required?

The first step is the threshold question: does the planned processing trigger the DPIA obligation under Art. 35 GDPR?

- **Art. 35(3) GDPR mandatory cases:** A DPIA is always required for: (a) systematic and extensive profiling with legal or similarly significant effect, (b) large-scale processing of special category data under Art. 9 GDPR (health, biometric, ethnic origin, religion, political opinion) or data on criminal convictions under Art. 10 GDPR, and (c) systematic monitoring of publicly accessible areas on a large scale.
- **DSK Muss-Liste (German DPA mandatory list):** Germany's Data Protection Conference (Datenschutzkonferenz, DSK) has published a positive list of processing types that always require a DPIA in Germany. These include: video surveillance with biometric identification, credit or insurance risk scoring, tracking of employee behaviour via apps or wearables, large-scale processing of genetic or biometric data, and centralised health data processing.
- **Three-criteria test (WP 248, Article 29 Working Party):** A DPIA is strongly indicated when **two or more** of the following criteria apply: scoring or profiling, automated decisions with significant effect, systematic monitoring, sensitive data categories, large-scale processing, data combination or matching, vulnerable groups (minors, employees, patients, criminal suspects), innovative technology, third-country transfers with reduced legal protection.
- **Material changes:** Changes to existing processing that materially increase the risk level re-trigger the DPIA obligation — for example, switching cloud providers, integrating an AI analytics system, or expanding to new data categories.

**Risk flags:**
- Two or more criteria met under the three-criteria test, but DPIA rejected
- Large-scale processing of sensitive data categories without a DPIA assessment
- Material system change without a fresh DPIA evaluation
- Workplace monitoring system deployed without a DPIA and without works council involvement (§ 87(1)(6) BetrVG — Germany's Works Constitution Act, which grants the works council co-determination rights over technical monitoring of employees)

### Step 2: Description of the processing operation (Art. 35(7)(a) GDPR)

The DPIA opens with a systematic description of the processing operation. Without a precise description, the risk cannot be assessed.

- **Purposes and legal bases:** Define all processing purposes and assign each a legal basis under Art. 6 GDPR. For special categories, identify the applicable exception under Art. 9(2) GDPR and, where relevant, BDSG §§ 22 and 26.
- **Data flow diagram:** Document all data flows: collection sources, internal routing, external recipients (including processors and joint controllers), third-country transfers, and deletion paths.
- **Data categories and data subject groups:** List all processed data categories — with particular flagging of sensitive categories — and all data subject groups. Vulnerable groups warrant special attention: minors, employees (structural power imbalance), patients, and criminal suspects.
- **Recipients and processors:** Every external recipient must be identified. For each processor, a compliant **[Data Processing Agreement (DPA) under Art. 28 GDPR](/en-DE/skills/data-processing-agreement/)** must be in place; third-country transfers require documentation of the transfer mechanism (Standard Contractual Clauses, adequacy decision).
- **Retention periods:** Define concrete deletion or blocking schedules for each data category, with the applicable basis (statutory retention obligation, legitimate business interest, consent).

**Risk flags:**
- Processing purposes vague or incompletely documented
- No data flow diagram; third-party access not identified
- Processor engaged without a compliant DPA
- Retention periods undefined or unrealistically long

### Step 3: Necessity and proportionality (Art. 35(7)(b) GDPR)

Assess whether the processing is limited to what is necessary (data minimisation under Art. 5(1)(c) GDPR) and whether the chosen means are proportionate to the intended purposes.

- **Data minimisation:** Are only the data actually required for the specific purpose being processed? Common failures: over-broad user profiles, real-time location tracking without operational need, long-term storage for hypothetical future requests.
- **Purpose limitation (Art. 5(1)(b) GDPR):** Test whether intended onward processing is compatible with the original collection purpose using the Art. 6(4) compatibility criteria: link between purposes, nature of data, consequences for data subjects, and safeguards applied. Incompatible onward processing requires a fresh, independent legal basis.
- **Less intrusive alternatives:** Have less invasive alternatives been considered and documented? Pseudonymisation instead of plain-text data, aggregated analytics instead of individual tracking, opt-in instead of opt-out. Document why the chosen method is preferable.
- **Employee data:** Processing of employee data requires a stricter proportionality review under BDSG § 26. Monitoring measures must be necessary, appropriate, and reasonable for employees.

**Risk flags:**
- More data collected than required without a documented justification
- Onward processing to new purposes without a compatibility test under Art. 6(4) GDPR
- No assessment of less intrusive alternatives documented
- Employee surveillance measures without a BDSG § 26 proportionality review

### Step 4: Risk identification and assessment (Art. 35(7)(c) GDPR)

The core of the DPIA is the structured risk analysis. Risks must be assessed from the **data subject's perspective** — not the organisation's.

- **Risk scenarios:** Identify concrete scenarios in which the processing could cause significant harm to data subjects:
  - **Unauthorised access:** data breach, hacking, insider abuse
  - **Unintended modification:** data loss, data corruption
  - **Unlawful processing:** purpose creep, algorithmic discrimination, profiling abuse
  - **Identity theft / reputational damage:** exposure of sensitive attributes or biometric data
  - **Decision consequences:** credit denial, hiring rejection, insurance exclusion through flawed automated decisions
- **Risk matrix:** Score each scenario by **likelihood** (high/medium/low) × **severity** (high/medium/low). Scenarios with high likelihood or high severity are addressed first.
- **Existing measures:** Existing technical and organisational measures (TOMs) must feed into the assessment — what matters for Art. 35 purposes is the **residual risk** after TOMs are applied.
- **AI-specific factors:** For AI-driven processing, additional risk factors apply: algorithmic bias, lack of explainability or interpretability, model drift, and privacy risks arising at the model design stage (Privacy by Design under Art. 25 GDPR).

**Risk flags:**
- Assessment conducted from the organisation's perspective rather than the data subject's
- Only abstract risks identified, without concrete scenarios scored for likelihood and severity
- No bias analysis for AI-driven decisions
- Risk analysis ignores known vulnerabilities or prior security incidents

### Step 5: Risk mitigation measures (Art. 35(7)(d) GDPR)

For each identified risk, document appropriate mitigation measures.

- **Technical measures:** Encryption at rest (AES-256) and in transit (TLS 1.2+), pseudonymisation, role-based access controls (RBAC), logging and auditing, penetration testing, data masking in development and test environments, secure deletion procedures.
- **Organisational measures:** Staff training, data protection policies, need-to-know principle, incident response procedures, DPO involvement, up-to-date record of processing activities under Art. 30 GDPR.
- **Contractual measures:** Compliant DPAs with all processors, appropriate third-country transfer mechanisms (Standard Contractual Clauses, adequacy decision), contractual audit rights over service providers.
- **Residual risk:** After all measures are applied, assess the remaining residual risk. If **high residual risk** persists, **prior consultation with the competent supervisory authority (Art. 36 GDPR) is mandatory**. The authority issues a written response within eight weeks (extendable to six months).
- **Works council (Betriebsrat):** For employee data processing that engages the works council's co-determination rights under § 87(1)(6) BetrVG, involve the works council in parallel. A works council agreement (Betriebsvereinbarung) can simultaneously serve as proportionality documentation.

**Risk flags:**
- TOMs are generic and not linked to the specific risks identified in Step 4
- Residual risk rated low without justification
- Art. 36 prior consultation skipped despite high residual risk
- Works council not involved in co-determination-relevant monitoring or analytics measures


## Special Scenarios

### AI systems and automated decisions

AI-driven processing operations typically satisfy two or more criteria of the three-criteria test and therefore almost always trigger the DPIA obligation.

- **High-risk AI under the AI Act (Annex III):** The DPIA under Art. 35 GDPR and the FRIA under Art. 27 AI Act are **separate instruments** and must be conducted independently. Joint documentation is permissible provided all requirements of both frameworks are fully met (→ [AI Act Compliance Check](/en-DE/skills/ai-act-compliance/)).
- **Automated individual decisions (Art. 22 GDPR):** Decisions based solely on automated processing that have a legal or similarly significant effect — credit denial, insurance tariff, job application screening — are only lawful under narrow conditions and always require a DPIA.
- **Profiling in employment:** AI-based performance evaluation or predictive hiring decisions trigger both the DPIA obligation and works council co-determination rights under § 87 BetrVG. Both processes must run in parallel.

### Video surveillance and biometric data

- **Video surveillance with biometric identification:** Always DPIA-required under the DSK Muss-Liste and Art. 35(3)(b) GDPR.
- **Basic CCTV (no biometrics):** A DPIA is required when systematically monitoring publicly accessible areas on a large scale (Art. 35(3)(c) GDPR). BDSG § 4 imposes additional requirements, including a balancing-of-interests test and duty to post notices.
- **Occupational health data:** Workplace health promotion programmes, sick-leave data analysis, or biometric access systems always require a DPIA, a legal basis under Art. 9(2) GDPR, and compliance with BDSG § 26(3).

### Third-country data transfers

Transfers of high-risk processing data to countries without an adequacy decision — particularly the USA without EU-US Data Privacy Framework certification, China, and Russia — must be addressed within the DPIA: document the transfer risk and the applicable transfer mechanism (Standard Contractual Clauses, Transfer Impact Assessment under Schrems II). A missing or deficient Transfer Impact Assessment combined with a third-country transfer significantly elevates residual risk.


## How Compound handles a DPIA engagement

When you engage Compound to conduct or review a Data Protection Impact Assessment, the process follows a structured six-step approach:

1. **Initial consultation** — scope the processing operation, carry out a preliminary DPIA assessment, and align on the review scope.
2. **Data flow workshop** — map the complete data flows together with your technical and business teams.
3. **Risk analysis** — structured identification and scoring of risks from the data subject perspective, including scenario-specific analysis for your processing situation.
4. **Measures plan** — a prioritised risk mitigation roadmap tailored to your technical and organisational infrastructure.
5. **DPIA document** — full documentation with residual risk assessment and a prior consultation recommendation under Art. 36 GDPR where applicable.
6. **Ongoing support** — annual review and event-driven updates for material changes to the processing or the regulatory framework.


## Limitations of this skill

This skill provides a structured preliminary assessment. Engaging a lawyer is necessary in the following cases:

- **Art. 36 prior consultation:** When high residual risk remains after all measures, consultation with the competent supervisory authority (the LfDI of the relevant German state, or the BfDI) is mandatory. Compound can assist throughout this process, including preparation of consultation materials.
- **AI high-risk systems:** The intersection of DPIA (Art. 35 GDPR), FRIA (Art. 27 AI Act), and technical documentation obligations (Art. 11, Annex IV AI Act) requires legal coordination across both frameworks.
- **Cross-border processing:** Data flows across multiple EU Member States may engage the One-Stop-Shop mechanism under Art. 56 GDPR, with the lead supervisory authority of the controller's main establishment.
- **Law enforcement data (BDSG § 62, Directive 2016/680):** A separate legal regime applies in place of Art. 35 GDPR for processing by competent authorities for law enforcement purposes.
- **Works council disputes:** Conflicts over co-determination rights relating to data-relevant monitoring or analytics measures require specialist employment and data protection counsel.

Compound is happy to assist with the conduct, documentation, and review of Data Protection Impact Assessments — both as an initial assessment and as ongoing compliance support.


## Frequently Asked Questions on Data Protection Impact Assessments

### When is a Data Protection Impact Assessment mandatory under GDPR?

A DPIA is mandatory under Art. 35 GDPR whenever a processing operation is likely to result in a high risk to the rights and freedoms of natural persons. This applies in particular to large-scale processing of special category data (such as health or biometric data), systematic profiling with significant effect, and systematic monitoring of publicly accessible areas on a large scale. Germany's DSK has published a mandatory list (Muss-Liste) identifying specific processing types that always trigger a DPIA under German law.

### What must a DPIA contain?

Under Art. 35(7) GDPR, a DPIA must include at minimum: (1) a systematic description of the intended processing including purposes and legal bases, (2) an assessment of the necessity and proportionality of the processing, (3) an assessment of the risks to the rights and freedoms of data subjects, and (4) the planned mitigation measures including safeguards, security measures, and procedures to protect personal data.

### Who must carry out a DPIA?

The obligation rests with the **controller** — the company or authority that determines the purposes and means of processing (Art. 4(7) GDPR). The **Data Protection Officer**, if appointed, must be consulted under Art. 35(2) GDPR. Processors are not themselves obligated to carry out a DPIA but must assist the controller under Art. 28(3)(f) GDPR.

### What happens if a required DPIA is not carried out?

Failing to carry out a legally required DPIA is a standalone GDPR violation. Supervisory authorities may impose fines of up to EUR 10 million or 2% of global annual turnover under Art. 83(4)(a) GDPR. The supervisory authority may also order a temporary or permanent ban on the processing under Art. 58(2)(f) GDPR.

### Does a DPIA need to be repeated after changes to the processing system?

Yes. A DPIA must be updated whenever the processing changes materially — for example, through new data categories, new recipients, a change of cloud provider, or the integration of an AI system. Minor changes that do not affect the risk level do not require a full repeat assessment, but should be documented.

### How long must a DPIA be retained?

A DPIA forms part of the record of processing activities under Art. 30 GDPR and must be kept current for the entire duration of the processing. After processing ends, supervisory authorities recommend retaining the DPIA for at least three years, as data subject claims and regulatory proceedings can be initiated retrospectively.

### What is the difference between a DPIA and a FRIA under the AI Act?

The **DPIA** (Art. 35 GDPR) assesses risks to data subjects' privacy rights and applies to any processing that poses a high risk. The **FRIA** (*Fundamental Rights Impact Assessment*, Art. 27 AI Act) assesses risks to all fundamental rights — including non-discrimination, human dignity, and the rule of law — posed by high-risk AI systems as classified under Annex III AI Act. The two assessments cover different legal frameworks and must be conducted independently. Joint documentation is permitted where both sets of requirements are fully satisfied in the same document. For more on the AI Act obligations that may run alongside a DPIA, see the [AI Act Compliance Check](/en-DE/skills/ai-act-compliance/) skill. For related GDPR data subject rights obligations, see the [GDPR Data Request](/en-DE/skills/gdpr-data-request/) skill.
