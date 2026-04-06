---
name: ai-act-compliance
description: 'Assessment framework for EU AI Act compliance. Risk classification, documentation requirements, and conformity assessment paths.'
---


## Overview

This skill provides a structured compliance assessment for AI systems under **Regulation (EU) 2024/1689** -- the EU AI Act. The regulation establishes a risk-based framework that categorizes AI systems into four tiers: unacceptable risk (prohibited), high risk (heavily regulated), limited risk (transparency obligations), and minimal risk (largely unregulated). Key provisions include **Art. 5** (prohibited AI practices), **Art. 6** (classification of high-risk systems), **Art. 8-15** (requirements for high-risk systems), **Art. 26** (deployer obligations), and **Art. 50** (transparency obligations). Use this skill when advising on the deployment, procurement, or development of AI systems within the EU, or when an existing system requires a compliance gap analysis.

The AI Act applies to providers, deployers, importers, and distributors of AI systems placed on the EU market or whose output is used in the EU, regardless of where the provider is established (Art. 2 Abs. 1). German companies must also consider the interplay with GDPR, sector-specific regulation (e.g., MDR for medical AI, MiFID II for financial AI, the Product Liability Directive), and the anticipated national implementation provisions. The regulation's extraterritorial reach means that non-EU providers serving EU customers are equally captured.


## Systematic Review

### Step 1: Actor Classification and Scope

Determine the entity's role under the AI Act and confirm the system falls within its scope. The obligations differ significantly depending on the actor classification.

- **AI system definition (Art. 3 Nr. 1):** A machine-based system designed to operate with varying levels of autonomy, that may exhibit adaptiveness after deployment, and that generates outputs such as predictions, content, recommendations, or decisions influencing physical or virtual environments. This definition is deliberately broad and captures machine learning models, rule-based systems, and hybrid approaches.
- **Provider (Art. 3 Nr. 3):** Develops or commissions an AI system and places it on the market or puts it into service under its own name or trademark. The provider bears the heaviest compliance burden, including conformity assessment, technical documentation, and post-market monitoring.
- **Deployer (Art. 3 Nr. 4):** Uses an AI system under its authority, except for personal non-professional activity. Companies using off-the-shelf AI tools qualify as deployers and bear independent obligations under Art. 26.
- **Importer and distributor:** Each carries distinct verification and record-keeping obligations (Art. 23-27).
- **Dual roles:** An entity may simultaneously be a provider and deployer -- for example, a company that develops an AI system for internal use. Both sets of obligations apply cumulatively.
- **Exclusions (Art. 2):** Military and national security systems (Art. 2 Abs. 3), systems used exclusively for scientific research (Art. 2 Abs. 6), and open-source systems with exceptions for high-risk and prohibited categories (Art. 2 Abs. 12).

**Flag as risk:**
- Entity acts as both provider and deployer without recognizing dual obligations
- Open-source exception claimed without verifying that no Annex III use case applies
- AI system used in the EU but provider assumes the Act does not apply due to non-EU establishment
- Narrow interpretation of "AI system" to exclude rule-based decision systems that may fall within the definition
- Failure to identify all entities in the value chain (e.g., a reseller qualifying as distributor)

### Step 2: Prohibited Practices Screening (Art. 5)

Check whether the AI system engages in any of the eight prohibited practices. These prohibitions have been enforceable since **2 February 2025** and carry the highest penalties (up to EUR 35 million or 7% of global annual turnover).

- **Subliminal manipulation (Art. 5 Abs. 1 lit. a):** Techniques deploying subliminal components beyond a person's consciousness that materially distort behaviour and cause significant harm. The prohibition covers techniques the person cannot reasonably perceive, regardless of whether the distortion is intended.
- **Exploitation of vulnerabilities (Art. 5 Abs. 1 lit. b):** Targeting specific groups based on age, disability, or social or economic situation to materially distort their behaviour in a manner that causes significant harm.
- **Social scoring (Art. 5 Abs. 1 lit. c):** Classification of persons based on social behaviour or personal characteristics, where the resulting social score leads to detrimental treatment that is unjustified or disproportionate. This prohibition applies to public authorities and entities acting on their behalf.
- **Criminal offence prediction (Art. 5 Abs. 1 lit. d):** Individual risk assessment for predicting criminal offences based solely on profiling or personality traits, except where used to augment human assessment based on objective, verifiable facts.
- **Real-time remote biometric identification (Art. 5 Abs. 1 lit. h):** In publicly accessible spaces for law enforcement purposes, with narrow exceptions requiring prior judicial authorization.
- **Emotion recognition (Art. 5 Abs. 1 lit. f):** In workplaces and educational institutions, except for medical or safety reasons.
- **Untargeted facial image scraping (Art. 5 Abs. 1 lit. e):** Creating or expanding facial recognition databases through untargeted scraping of facial images from the internet or CCTV footage.
- **Biometric categorization (Art. 5 Abs. 1 lit. g):** Using biometric data to infer sensitive attributes such as race, political opinions, trade union membership, religious beliefs, or sexual orientation, except for law enforcement with prior judicial authorization.

**Flag as risk:**
- Any match with a prohibited practice requires immediate cessation or fundamental redesign
- System uses biometric data without clear justification under a permitted exception
- Emotion recognition deployed in a workplace setting, even if labelled as "voluntary" or for "wellbeing"
- Persuasive AI in marketing that may cross the line into subliminal manipulation
- Social scoring elements embedded in creditworthiness or insurance assessments by public entities

### Step 3: Risk Classification (Art. 6 and Annexes I/III)

If the system is not prohibited, determine whether it qualifies as high-risk. This classification is the gateway to the most demanding compliance requirements.

- **Annex I pathway (safety component):** The system is a safety component of a product, or is itself a product, covered by EU harmonised legislation listed in Annex I. This includes machinery (Regulation 2023/1230), medical devices (MDR 2017/745), in vitro diagnostics (IVDR 2017/746), automotive (Regulation 2019/2144), aviation, rail, marine, toys, lifts, and pressure equipment. If the product requires a third-party conformity assessment, the AI system must also undergo third-party assessment.
- **Annex III pathway (standalone high-risk):** The system falls within one of the eight listed categories: (1) biometric identification and categorization, (2) management and operation of critical infrastructure, (3) education and vocational training, (4) employment, workers management, and self-employment access, (5) access to essential private and public services, (6) law enforcement, (7) migration, asylum, and border control, (8) administration of justice and democratic processes.
- **Art. 6 Abs. 3 exception:** A system listed in Annex III is not high-risk if it does not pose a significant risk of harm to health, safety, or fundamental rights, does not materially influence the outcome of decision-making (i.e., it is purely preparatory), and does not profile natural persons. The provider must document the assessment and notify the relevant national authority before placing the system on the market.
- **General-purpose AI models (Art. 51-56):** Models trained with large amounts of data using self-supervision that display significant generality. Providers of GPAI models face transparency obligations (Art. 53) and, if classified as posing systemic risk (based on cumulative compute above 10^25 FLOPS or designation by the AI Office), additional obligations including adversarial testing, incident reporting, and cybersecurity measures (Art. 55).

**Flag as risk:**
- Classification rationale not documented as required by Art. 6 Abs. 4
- Art. 6 Abs. 3 exception claimed without written justification or without notification to the national authority
- System clearly falls within Annex III but is treated as limited risk to avoid compliance costs
- GPAI model provider unaware of systemic risk classification threshold
- AI system embedded in a product regulated under Annex I harmonised legislation without coordination with the product conformity assessment

### Step 4: High-Risk System Requirements (Art. 8-15, Art. 26)

For systems classified as high-risk, confirm compliance with each mandatory requirement. These obligations apply to providers (Art. 8-15) and deployers (Art. 26) with different scopes.

- **Risk management system (Art. 9):** A continuous, iterative process for identifying, analysing, estimating, and evaluating risks. The system must be established, documented, implemented, and maintained throughout the AI system's lifecycle. Risk management must include testing to identify the most appropriate risk mitigation measures.
- **Data governance (Art. 10):** Training, validation, and testing datasets must be relevant, sufficiently representative, and free of errors to the extent possible. Bias detection and mitigation measures are mandatory. Art. 10 Abs. 5 creates a limited exception for processing special category data (Art. 9 GDPR) specifically for bias monitoring, subject to strict safeguards.
- **Technical documentation (Art. 11, Annex IV):** Comprehensive documentation covering the system's general description, detailed development methodology, monitoring and control mechanisms, risk management process, and record of changes. Documentation must be prepared before the system is placed on the market and kept up to date.
- **Record-keeping and logging (Art. 12):** Automatic recording of events (logs) for traceability throughout the system's lifecycle. Logs must be retained for a period appropriate to the intended purpose, and no less than six months unless otherwise required by law.
- **Transparency and information to deployers (Art. 13):** Clear, concise instructions for use, including the system's capabilities, limitations, intended purpose, foreseeable misuse scenarios, and performance metrics (accuracy, robustness, cybersecurity properties).
- **Human oversight (Art. 14):** Measures enabling effective human supervision during the system's operation. The human overseer must be able to understand the system's capabilities and limitations, correctly interpret outputs, decide not to use or override the output, and intervene or halt the system. Mere rubber-stamping does not satisfy the requirement.
- **Accuracy, robustness, cybersecurity (Art. 15):** Appropriate levels must be maintained throughout the lifecycle, including resilience against attempts to manipulate training data or outputs (data poisoning, adversarial attacks).

**Deployer-specific obligations (Art. 26):**
- Use the system in accordance with the provider's instructions for use
- Assign competent, trained, and authorised persons for human oversight
- Monitor the system's operation and report incidents to the provider or distributor
- Conduct a **fundamental rights impact assessment (FRIA)** under Art. 27 before deploying high-risk systems in certain categories (credit scoring, insurance pricing, recruitment, public services)
- Inform natural persons that they are subject to a high-risk AI system and provide meaningful information about the system's logic

**Flag as risk:**
- No documented risk management process or process limited to a one-time assessment at deployment
- Training data provenance unknown or undocumented, making bias assessment impossible
- Human oversight measures purely nominal with no practical ability to intervene or override
- FRIA not conducted where Art. 27 requires it (particularly for credit, insurance, employment, and public service use cases)
- Logging disabled or retention period inadequate
- Technical documentation incomplete or not updated after material changes

### Step 5: Transparency Obligations for All AI Systems (Art. 50)

Even systems that are not high-risk must meet transparency requirements when they interact with natural persons or generate synthetic content.

- **Disclosure of AI interaction (Art. 50 Abs. 1):** Providers of AI systems intended for direct interaction with natural persons (chatbots, virtual assistants, customer service agents) must ensure the system discloses that the user is interacting with an AI. Exception: where this is obvious from the circumstances, or where the system is authorised by law for detection of criminal offences.
- **Synthetic content labelling (Art. 50 Abs. 2):** Providers of AI systems that generate synthetic audio, image, video, or text must ensure the output is marked as artificially generated or manipulated in a machine-readable format. Deployers of deepfake systems must disclose that the content has been artificially generated or manipulated.
- **Emotion recognition and biometric categorization (Art. 50 Abs. 3):** Where such systems are deployed (outside the prohibited contexts), the deployer must inform the affected natural persons and process personal data in compliance with GDPR.
- **General-purpose AI transparency (Art. 53):** GPAI model providers must maintain technical documentation, comply with EU copyright law, and publish a sufficiently detailed summary of training data content.

**Flag as risk:**
- No disclosure mechanism for AI-generated content, particularly in customer-facing applications
- Deepfake-capable system without machine-readable output labelling
- Chatbot or virtual assistant deployed without AI disclosure, creating deception risk
- AI-generated text used in legal, medical, or financial communications without disclosure
- GPAI model used to generate content at scale without copyright compliance

### Step 6: Compliance Timeline, Conformity Assessment, and Enforcement

The AI Act applies in phases. Determine which deadlines and procedures apply to the specific system and actor.

- **Prohibited practices:** Enforceable since **2 February 2025**
- **General-purpose AI models:** Obligations since **2 August 2025**
- **Annex III high-risk systems:** Requirements from **2 August 2026**
- **Annex I harmonised legislation products:** Requirements from **2 August 2027**
- **Conformity assessment (Art. 43):** For most high-risk systems, self-assessment (internal control procedure, Annex VI) is sufficient. Third-party assessment through a notified body is required for biometric identification systems (Annex III Nr. 1) and for high-risk systems that are safety components of products requiring third-party assessment under Annex I harmonised legislation.
- **EU declaration of conformity (Art. 47):** The provider must draw up a written declaration, keep it updated, and make it available to national authorities for 10 years.
- **CE marking (Art. 48):** Required for high-risk systems, affixed visibly and legibly to the system or its packaging.
- **EU database registration (Art. 49):** High-risk systems must be registered in the EU database before being placed on the market.

**Enforcement and penalties (Art. 99):**

| Violation | Maximum penalty |
|---|---|
| Prohibited practices (Art. 5) | EUR 35 million or 7% of global annual turnover |
| High-risk system requirements | EUR 15 million or 3% of global annual turnover |
| Incorrect information to authorities | EUR 7.5 million or 1% of global annual turnover |

SMEs and startups benefit from proportionate caps (Art. 99 Abs. 6). National market surveillance authorities enforce the regulation, with coordination through the AI Office.

**Flag as risk:**
- Deadline for applicable obligations already passed without compliance measures in place
- No conformity assessment procedure identified or initiated
- CE marking required but not applied
- System not registered in the EU database
- No designated national supervisory authority identified


## Special Scenarios

### AI in HR and Recruitment

AI systems used for recruitment, candidate screening, promotion decisions, task allocation, or performance monitoring fall within **Annex III Nr. 4** (employment). This is one of the most common high-risk categories for corporate deployers.

- **Deployer FRIA required** under Art. 27 before deployment
- **Works council co-determination** under **§ 87 Abs. 1 Nr. 6 BetrVG** (monitoring of employee behaviour) applies in Germany, creating a parallel consent requirement
- **Anti-discrimination law:** Algorithmic bias can create liability under the **AGG** (General Equal Treatment Act) if protected characteristics are directly or indirectly used in decision-making
- **Employee notification:** Employees must be informed they are subject to a high-risk AI system (Art. 26 Abs. 7)

### AI in Financial Services

AI in credit scoring, insurance underwriting, and fraud detection may be high-risk under **Annex III Nr. 5** (essential services) and is also subject to sector-specific regulation.

- **MiFID II suitability requirements** for AI-driven investment advice
- **DORA (Digital Operational Resilience Act)** ICT risk management for AI in financial institutions
- **ECB/BaFin expectations** on model risk management and explainability
- **GDPR Art. 22:** Automated individual decision-making including profiling -- data subjects have the right not to be subject to decisions based solely on automated processing that produce legal or similarly significant effects

### GDPR and AI Act Interplay

The two regulations apply cumulatively. Key areas of overlap:

- **Data minimization (Art. 5 Abs. 1 lit. c GDPR)** vs. data quality and representativeness requirements (Art. 10 AI Act) -- these can create tension
- **DPIA (Art. 35 GDPR)** and **FRIA (Art. 27 AI Act)** are separate requirements that may need to be conducted in parallel
- **Lawful basis for training data:** GDPR Art. 6 applies to all personal data used in training, and legitimate interest (Art. 6 Abs. 1 lit. f) requires a balancing test
- **Art. 10 Abs. 5 AI Act** creates a narrow exception for processing special category data for bias detection, subject to anonymization after the bias assessment and with no re-use for other purposes


## Limitations of This Skill

This skill provides a structured preliminary assessment. In the following cases, engaging a lawyer is necessary:

- **Conformity assessment procedures** and preparation of technical documentation for notified body review
- **Sector-specific interplay** between the AI Act and financial regulation (MiFID II, DORA), medical device regulation (MDR), or employment law (BetrVG, AGG)
- **Cross-border deployment** involving multiple EU member states with differing national implementation measures
- **GPAI model providers** facing systemic risk classification and associated obligations
- **Regulatory proceedings** or market surveillance inquiries by national authorities or the AI Office
- **Contractual allocation** of AI Act obligations between providers, deployers, and distributors in complex supply chains

Compound is happy to assist with AI Act compliance assessments, risk classification, and the preparation of conformity documentation.
