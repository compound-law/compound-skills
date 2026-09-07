---
name: saas-agreement
description: 'SaaS contracts shift risk onto you: liability caps, GDPR gaps, and data lock-in. Expert review under German law before you sign.'
---


## Overview

Under German law, SaaS agreements are classified as **Mietvertrag** (rental agreements, §§ 535 ff. BGB), giving customers statutory defect rights (§ 536 BGB) and extraordinary termination rights (§ 543 BGB). The four highest-risk review areas are: liability caps under §§ 305–310 BGB, data portability, GDPR-compliant processing terms, and exit provisions that prevent data lock-in.

This skill provides a structured review of Software-as-a-Service (SaaS) subscription agreements from the customer's perspective under German and EU law. The BGH has not issued a definitive classification ruling, and the prevailing view treats standard SaaS as a lease of software functionality. Key consumer and SME protections apply through AGB control (**§§ 305–310 BGB**), particularly **§ 307** (unreasonable disadvantage test), **§ 308** (prohibited clauses with evaluation possibility), and **§ 309** (strict prohibitions including § 309 Nr. 7 on liability exclusions for personal injury). Use this skill when evaluating vendor-drafted SaaS terms for procurement, renegotiating renewal terms, or assessing data protection and exit risks.

SaaS agreements present unique risks around data lock-in, unilateral service modifications, opaque subcontracting, and liability caps that may leave the customer without adequate recourse. A thorough review must address commercial terms alongside data protection, intellectual property, and regulatory compliance dimensions.

Common SaaS tools reviewed with this skill include [Airtable](/en-DE/tools/airtable-ai/) and [Notion](/en-DE/tools/notion-ai/). If the vendor uses AI-powered features, additional review of [AI customer service compliance](/en-DE/compliance/ai-customer-service/) under the EU AI Act may apply.


## Systematic Review

### Step 1: Service Description and SLA Commitments

The service description is the foundation of the entire agreement. Verify that it is precise enough to establish the contractual performance obligation (Leistungspflicht).

- **Functional scope:** The agreement must specify the features, modules, and capabilities included in the subscription. Vague descriptions like "access to the platform" are insufficient -- the customer needs to know exactly what it is paying for, and any reduction in functionality may constitute a defect (Mangel).
- **User limits and access model:** Confirm whether the subscription is based on named users, concurrent users, or enterprise-wide access. Check whether API access, integrations, and administrative accounts are included.
- **Storage and data quotas:** Verify included storage volumes, data retention periods, and the consequences of exceeding quotas (automatic upgrade, throttling, or data deletion).
- **Geographic availability:** For international deployments, confirm whether the service is available in all relevant jurisdictions and whether data residency requirements are met.
- **SLA uptime commitment:** The SLA should define a specific monthly availability percentage (market standard: 99.5% to 99.9%). Check the following details:
  - **Measurement methodology:** How is downtime calculated? Is it measured at the application layer or only the infrastructure layer? Infrastructure-level availability can mask application-level outages that render the service unusable for the customer.
  - **Exclusions:** Scheduled maintenance windows, force majeure, and third-party outages are typically excluded. Verify that maintenance windows are reasonable (e.g., weekends, low-traffic hours) and that the total excluded time per month is capped.
  - **Remedies for SLA breach:** Service credits are the standard remedy -- typically 5-10% of the monthly fee per defined increment of downtime (e.g., per 0.1% below the SLA target). Check whether credits are applied automatically or only on request, and whether there is a cap on credits.
  - **Escalation to termination:** At what level of persistent failure can the customer terminate? Best practice: if the SLA is breached for three consecutive months or four months in a 12-month period, the customer should have an extraordinary termination right.
- **Binding commitment vs. best effort:** Confirm whether the SLA is a **contractual commitment** (the provider is liable for breach) or merely a **target** or **best-effort undertaking** (no liability). An SLA labelled as "target" provides no contractual protection.

**Flag as risk:**
- Service description too vague to establish the contractual performance standard
- SLA defines "availability" at the infrastructure level only, masking application-level outages
- SLA remedies limited to service credits with no termination right for persistent failure
- SLA labelled as "target" or "best effort" rather than a binding commitment
- No scheduled maintenance window limits, allowing the provider to claim unlimited maintenance time

### Step 2: Performance Standards and Support Levels

Beyond availability, verify that the agreement includes performance and support commitments that ensure the service remains usable in practice.

- **Response times:** The agreement should define maximum response times for the platform (e.g., page load times, API response times under normal load).
- **Support tiers and response windows:** Support should be categorized by severity:

| Priority | Description | Response time | Resolution target |
|---|---|---|---|
| **P1 Critical** | Service completely unavailable or core functionality broken | 1-4 hours | 8-24 hours |
| **P2 High** | Significant feature degraded, workaround available | 4-8 hours | 1-3 business days |
| **P3 Medium** | Non-critical feature impaired | 1 business day | 5-10 business days |
| **P4 Low** | Minor issue or feature request | 2-5 business days | Best effort |

- **Support channels:** Check whether support is available by phone, email, chat, or ticket system, and during which hours (24/7 for P1 is standard for enterprise SaaS).
- **Reporting obligations:** The provider should deliver monthly uptime reports and incident post-mortem reports for significant outages. Without reporting, the customer cannot verify SLA compliance.
- **Defect under lease law:** Under German lease law principles (§§ 535 ff. BGB), persistent failure to meet contractual performance levels constitutes a defect (Mangel) entitling the customer to **rent reduction** (§ 536 BGB) or, if the defect is material, **extraordinary termination** (§ 543 BGB). The SLA credit mechanism does not automatically exclude these statutory remedies -- a clause purporting to do so must be reviewed under § 307 BGB.

**Flag as risk:**
- No support response time commitments
- P1 critical support unavailable outside business hours
- No monthly uptime reporting, preventing SLA verification
- SLA credits expressly exclude any further claims under statutory defect law
- No escalation procedure for unresolved issues

### Step 3: Data Ownership, Portability, and Deletion Rights

Data lock-in is the most strategically dangerous risk in SaaS agreements. Verify that the customer retains full control over its data at all times.

- **Customer data ownership:** The agreement must clearly state that the customer retains full ownership of all data uploaded to or generated within the platform ("customer data"). The provider should receive only a limited, revocable license to process customer data for the sole purpose of delivering the service.
- **Provider's data use rights:** Scrutinize any clause granting the provider rights to aggregate, anonymize, or use customer data for product improvement, benchmarking, analytics, machine learning training, or marketing. Under **GDPR Art. 6**, any processing beyond the primary service purpose requires an independent lawful basis. The customer's legitimate interest in data control should take precedence over the provider's commercial interest in data exploitation.
- **Data export (portability):** The customer should be able to export all customer data in standard, machine-readable formats (CSV, JSON, XML, or industry-specific formats such as XBRL for financial data) at any time during the contract and for a defined post-termination period (30-90 days is standard). Export functionality should be self-service and available without additional fees.
- **Data deletion after termination:** The provider must delete all customer data within a specified period after contract termination (30 days is common) and provide **written certification** of deletion. Check whether the deletion obligation extends to backups and disaster recovery copies -- complete deletion of backups may be technically impractical, in which case the agreement should specify a maximum retention period for backup copies (typically 90-180 days) with access restrictions.
- **Data in transit and at rest:** Verify that the agreement addresses data encryption in transit (TLS 1.2+) and at rest (AES-256 or equivalent). Bring-your-own-key (BYOK) or hold-your-own-key (HYOK) encryption gives the customer control over the encryption keys and prevents provider access to unencrypted data.

**Flag as risk:**
- Provider claims ownership of or a broad license to customer data
- Provider uses customer data for AI training, benchmarking, or product improvement without explicit consent
- No data export functionality or export only in proprietary formats
- No deletion obligation or no written certification of deletion
- Deletion obligation excludes backup copies without any retention limit
- No encryption at rest or in transit for customer data

### Step 4: Liability Caps and Exclusions (§§ 305-310 BGB)

German AGB law imposes mandatory limits on liability exclusions in standard terms. SaaS providers frequently push liability caps to the minimum -- the customer must verify that the caps provide meaningful protection.

- **Mandatory unlimited liability:** Under German law, the following categories of liability **cannot be excluded or limited** in standard terms:
  - **Personal injury from negligence (§ 309 Nr. 7 lit. a BGB):** Any clause excluding or limiting liability for death or bodily injury caused by negligence is per se void.
  - **Gross negligence and intent (§ 309 Nr. 7 lit. b BGB):** Liability for other damages caused by gross negligence or intentional conduct cannot be excluded.
  - **Product Liability Act (Produkthaftungsgesetz):** Strict liability under the ProdHaftG cannot be excluded by contract.

- **Cardinal obligations (Kardinalpflichten/wesentliche Vertragspflichten):** Under § 307 BGB, liability for breach of cardinal obligations -- obligations whose fulfillment is essential for the proper performance of the contract and on which the customer may regularly rely -- may be limited, but only to the **typically foreseeable, contract-typical damage** (vertragstypisch vorhersehbarer Schaden). A cap below this level is void. For SaaS, cardinal obligations include: providing the service in accordance with the service description, maintaining data integrity, and complying with data protection obligations.

- **Valid liability clause structure:**
  1. Liability for intent and gross negligence: **unlimited**
  2. Liability for breach of cardinal obligations through slight negligence: limited to **typically foreseeable, contract-typical damage** (often quantified as 100% of annual subscription fees)
  3. Liability for personal injury: **unlimited**
  4. Liability under ProdHaftG: **unlimited**
  5. General cap for all other claims: commonly 100% of annual fees paid in the preceding 12 months

- **Data loss liability:** Clauses excluding liability for data loss regardless of fault are problematic. The provider should be liable for data loss at least to the extent of restoring data from the most recent backup, provided the customer has fulfilled any contractual backup obligations.
- **Indirect and consequential damages:** Many SaaS agreements exclude "indirect, consequential, special, or incidental damages." Under German law, this exclusion is unusual and ambiguous -- the German concept of Schadenersatz does not distinguish between direct and indirect damages in the common-law sense. A blanket exclusion may be invalid under § 307 BGB if it effectively eliminates liability for foreseeable contract-typical damages.

**Flag as risk:**
- Blanket liability exclusion without differentiating between fault categories ("Liability is excluded to the maximum extent permitted by law")
- Cap set at one month's fees or a similarly trivial amount
- Liability for data loss excluded regardless of fault
- Indirect/consequential damages excluded without distinguishing between breach categories
- Cardinal obligation liability capped below the typically foreseeable damage
- No carve-out for personal injury, gross negligence, or intent

### Step 5: Auto-Renewal, Term, and Price Changes

SaaS agreements are designed for recurring revenue. Verify that the renewal and pricing mechanisms are balanced.

- **Initial term:** Common ranges are 12 months (standard), 24 months, or 36 months (enterprise). Longer terms typically come with volume discounts but reduce flexibility.
- **Auto-renewal mechanism:** Most SaaS agreements renew automatically unless the customer provides timely notice of non-renewal. Under German AGB law (§ 307 BGB), auto-renewal clauses in B2B terms are permissible but must be proportionate. Renewal periods exceeding one year or notice periods shorter than three months may be challenged. For B2C (§ 309 Nr. 9 BGB), the initial term may not exceed two years, and after the initial term, the consumer may cancel at any time with one month's notice (since 01.03.2022).
- **Notice period for non-renewal:** Verify the exact deadline (e.g., 90 days, 60 days, or 30 days before the end of the current term). Missing the deadline locks the customer into another term.
- **Price increase upon renewal:** Check whether the provider may increase prices at renewal and under what conditions. Best practice: price increases capped at a specified percentage (e.g., CPI + 3%) or subject to the customer's right to terminate if the increase exceeds a threshold. Unlimited price increase discretion upon renewal is problematic under § 307 BGB.
- **Mid-term price changes:** Check whether the provider reserves the right to change prices during a running term. If so, the customer should have an extraordinary termination right within a defined period after the price change takes effect.
- **Downgrade and usage reduction:** Verify whether the customer can reduce the number of users, modules, or storage during the term, or only at renewal. "Ratchet" clauses that prevent downgrades lock the customer into the highest usage level reached.

**Flag as risk:**
- Auto-renewal period exceeds one year in a B2B standard-form agreement
- Notice period for non-renewal shorter than three months (easy to miss)
- Unlimited price increase discretion at renewal without termination right
- Mid-term price changes permitted without customer's right to terminate
- Ratchet clause preventing any reduction in scope during or at the end of the term
- B2C terms with initial term exceeding two years or automatic renewal exceeding one month

### Step 6: Exit Provisions, Transition Assistance, and DPA Requirement

The end of the contract is often where the most significant risks materialize. Verify that the exit provisions protect the customer's continuity.

- **Post-termination transition period:** The agreement should provide a transition period (60-180 days is standard for enterprise SaaS) during which the customer retains access to the service and data export functionality, either at the existing subscription fee or at a defined transition rate.
- **Migration support:** For complex SaaS implementations, the provider should offer migration assistance -- data mapping, API access for migration tools, and technical support for the transition to a replacement service. Check the fees for migration support and whether they are capped.
- **Data portability at exit:** Confirm that the data export provisions (Step 3) apply during the transition period and that all data, including historical data, logs, and configurations, can be exported.
- **GDPR Art. 28 DPA requirement:** Whenever the SaaS provider processes personal data on behalf of the customer, a **Data Processing Agreement (Auftragsverarbeitungsvertrag, AVV)** compliant with Art. 28 GDPR is mandatory. The DPA should be reviewed separately using the Data Processing Agreement skill. Verify that the main SaaS agreement references or incorporates the DPA, and that the termination of the SaaS agreement triggers the DPA's data deletion obligations.
- **Provider insolvency or service discontinuation:** For business-critical SaaS, the customer should negotiate protective provisions:
  - **Source code escrow:** A third-party escrow agent holds the source code, which is released to the customer upon triggering events (provider insolvency filing, persistent material SLA breach, or service discontinuation). The escrow agreement should include the right to host and modify the code.
  - **Data escrow:** Separate from source code, the customer's data should be accessible even if the provider's infrastructure becomes unavailable.
  - **Step-in rights:** The right for the customer or a designated third party to take over operation of the service on the provider's infrastructure in case of provider failure.
- **Insolvency treatment (§ 103 InsO):** If the provider becomes insolvent, the insolvency administrator may reject executory contracts (contracts where performance is not yet complete on both sides). The customer's contractual claims for data return become unsecured insolvency claims (Insolvenzforderungen) unless the data is clearly the customer's property. This makes pre-insolvency protections (escrow, data export) essential.

**Flag as risk:**
- No transition period after termination -- access cut off immediately
- No data export capability or export only in proprietary formats during transition
- DPA missing or not Art. 28-compliant
- No source code escrow or continuity provisions for business-critical SaaS
- Migration support not addressed or subject to prohibitively expensive fees
- Insolvency of the provider not addressed, leaving the customer with unsecured claims for data return


## Risk Assessment

### Customer Risk Matrix

| Risk | Impact | Mitigation |
|---|---|---|
| SLA below 99.5% with no remedy | Service unreliability without recourse | Negotiate binding SLA with credits and termination right |
| Data lock-in (proprietary formats) | Cannot migrate to alternative provider | Require standard-format export at any time |
| Liability cap at 1 month's fees | Damages exceed cap in any serious incident | Negotiate 100% annual fees minimum, unlimited for data breach |
| No DPA or non-compliant DPA | GDPR violation and fine exposure | Require Art. 28-compliant DPA before go-live |
| Auto-renewal with short notice | Locked into unwanted renewal | Calendar the notice deadline; negotiate 90-day minimum |
| Unilateral feature changes | Core functionality removed mid-term | Require no material degradation + termination right for material changes |
| Provider insolvency | Loss of access to data and service | Source code escrow + data export + transition period |
| No deletion confirmation | Data retained after termination | Require written certification within 30 days |


## Special Scenarios

### Unilateral Service Modifications

One of the most contested clauses in SaaS agreements. Under German AGB law (§ 308 Nr. 4 BGB for B2C; § 307 BGB for B2B), unilateral modification clauses are subject to strict scrutiny:

- **Permissible modifications:** The change must serve a legitimate purpose (legal compliance, security update, technical improvement), must not alter the core service character (Kernleistung), and the customer must receive reasonable advance notice and a termination right if the modification is material.
- **Impermissible modifications:** A clause allowing the provider to "modify the service at any time for any reason" is void (BGH, III ZR 169/19). Similarly, removing features that were part of the agreed service description without replacing them with equivalent functionality crosses the line.
- **Customer's remedy:** The customer should have the right to terminate without penalty within a defined period (30-60 days) after a material modification takes effect.

### SaaS for Regulated Industries

Financial services, healthcare, and public sector customers face additional requirements:

- **BaFin outsourcing requirements (MaRisk AT 9):** Financial institutions must conduct a risk analysis before outsourcing to a SaaS provider, agree on audit and access rights for BaFin, and ensure the service can be transitioned without disruption.
- **Healthcare data (§ 203 StGB):** SaaS providers handling data subject to professional secrecy (medical, legal, tax) must be formally authorized. A DPA alone is insufficient -- a separate consent to data processing under § 203 StGB is required.
- **Public sector procurement:** Cloud services must comply with the BSI C5 cloud security standard (or equivalent) and the EVB-IT Cloud terms published by the German federal government.

### Open-Source Components

SaaS providers commonly use open-source software components. The agreement should:

- Warrant that all open-source use is compliant with applicable licenses
- Disclose any copyleft-licensed components (GPL, AGPL) that could create obligations for the customer
- Indemnify the customer against third-party claims arising from the provider's use of open-source components


## Frequently Asked Questions

### Is a SaaS agreement a rental contract under German law?

Yes. Under the prevailing view of German courts and legal commentary, standard SaaS agreements are classified as **Mietvertrag** (rental agreements, §§ 535 ff. BGB) because the customer receives temporary access to hosted software without ownership. This classification activates statutory defect rights: the customer may withhold rent proportionally if the service falls below the contractual standard (§ 536 BGB) and may terminate extraordinarily for persistent material failure (§ 543 BGB). The BGH has not issued a definitive ruling, but lower courts consistently apply rental law to cloud SaaS models.

### What GDPR clauses must be in a SaaS contract?

Every SaaS agreement where the vendor processes personal data on behalf of the customer must include a **Data Processing Agreement (Auftragsverarbeitungsvertrag, AVV)** compliant with Art. 28 GDPR. The AVV must specify the subject matter, nature, and purpose of processing, the type of personal data, and the vendor's obligations including data deletion, security measures, and sub-processor management. Without an Art. 28-compliant AVV, using the SaaS service constitutes an independent GDPR violation subject to fines up to EUR 10 million or 2% of global annual turnover.

### What are typical SaaS liability cap risks?

SaaS vendors typically cap liability at one or three months' subscription fees, which is far below actual damages in the event of data loss, a security breach, or prolonged outages. Under §§ 305–310 BGB, such caps are subject to AGB scrutiny: liability for intent and gross negligence cannot be limited (§ 309 Nr. 7 BGB), and caps for breach of cardinal obligations (Kardinalpflichten) must cover at least the typically foreseeable, contract-typical damage. A cap at one month's fees for a cardinal obligation breach may be void under § 307 BGB.


## Limitations of This Skill

This skill provides a structured preliminary assessment. In the following cases, engaging a lawyer is necessary:

- **Negotiation of enterprise SaaS agreements** with customized terms, particularly for critical infrastructure or regulated industries
- **GDPR compliance** including DPA review, transfer impact assessments, and cross-border data flow analysis
- **Intellectual property disputes** related to customer data, generated outputs, or AI training on customer data
- **Insolvency-related protections** including source code escrow agreements and step-in rights
- **Regulatory compliance** for financial services (MaRisk, DORA), healthcare (§ 203 StGB), and public sector procurement
- **Litigation** arising from SLA breaches, data loss, or unilateral service termination

Compound is happy to assist with the review, negotiation, and structuring of SaaS agreements that protect the customer's interests under German and EU law.
