---
name: gdpr-data-request
description: 'Guide for handling data access requests under Art. 15 GDPR. Deadlines, mandatory disclosures, and process steps for German companies.'
---


## Overview

This skill walks you through the complete handling of data access requests under Art. 15 GDPR (in Germany commonly referred to as "DSGVO-Auskunftsanfrage" or "Betroffenenanfrage"). It covers the entire process -- from receiving the request to delivering a timely, legally compliant response -- and takes into account the latest case law from the CJEU and German courts.

**Legal basis:** Art. 15 GDPR, Art. 12 GDPR, BDSG (Federal Data Protection Act) Sections 29, 34.

**Risk of non-compliance:** Fines of up to EUR 20 million or 4% of annual worldwide turnover (Art. 83(5) GDPR), plus damages claims by data subjects (Art. 82 GDPR).

## Step-by-Step Process

### Step 1: Receipt and Documentation

- Document the request immediately: date of receipt, channel (email, post, web form, verbal), sender, exact wording.
- Art. 15 requests have no formal requirements -- even verbal, casual, or unspecific requests such as "What data do you have about me?" trigger the obligation.
- The date of receipt starts the clock on the deadline. For email, the relevant time is when the message reaches the server, not when someone reads it.
- Notify the responsible internal team immediately (Data Protection Officer, legal department).
- Create a ticket or case file with deadline tracking.

### Step 2: Identity Verification

Identity verification must be **proportionate** (Art. 12(6) GDPR). The BfDI (Federal Commissioner for Data Protection) has clarified: there is no blanket right to demand a copy of an ID document (cf. PAuswG Section 20(2) -- no general right to copy identity documents).

**Differentiate by channel:**

| Request Channel | Appropriate Verification |
|---|---|
| Registered customer account | Login authentication is sufficient |
| Known business email address | Confirmation email to the known address |
| Unknown email address | Follow-up with identifying details (customer number, contract number, date of birth) |
| By post | Cross-reference with existing records; if needed, reply to the address on file |
| By telephone | Security questions based on existing data |
| Via a lawyer | Verify written power of attorney (Vollmacht) |

**Important:** The deadline continues to run during identity verification. Verification must therefore be carried out promptly. Only where there are reasonable doubts about the requester's identity may processing be suspended pending clarification (Art. 12(6) GDPR). In that case, the deadline runs from the date identity is confirmed.

### Step 3: Calculate Deadlines

- **Standard deadline:** 1 month from receipt of the request (Art. 12(3) GDPR).
- **Extension:** An additional 2 months is possible (3 months total) if the request is complex or multiple requests are received simultaneously.
- **If extending:** The data subject must be informed within the first month about the extension and the reasons for it.
- Deadline calculation follows Sections 187, 188 BGB (German Civil Code): receipt on 15 March means the deadline expires on 15 April (midnight). If the deadline falls on a Saturday, Sunday, or public holiday, it extends to the next business day (Section 193 BGB).

**When is a request considered "complex"?**
- Data processing across numerous systems
- Extensive third-country transfers
- Significant redaction requirements (third-party rights affected)
- Multiple simultaneous requests from the same individual

### Step 4: Data Collection

The record of processing activities (Verzeichnis von Verarbeitungstaetigkeiten, Art. 30 GDPR) serves as a checklist. Systematically search the following systems:

- **CRM system** (master customer data, communication history, notes)
- **Email systems** (all mailboxes where communication with the individual took place)
- **HR / personnel system** (for employee requests: personnel file, payroll, time tracking, sick notes, performance reviews)
- **ERP system** (orders, invoices, payment transactions)
- **Marketing tools** (newsletter subscriptions, tracking data, consent database)
- **Support / ticketing system** (inquiries, complaints, call notes)
- **Web analytics** (usage profiles, cookies -- to the extent attributable to the individual)
- **Access and log data** (building access, IT access logs)
- **Physical files** (contracts, correspondence, handwritten notes)
- **Processors** (Auftragsverarbeiter, Art. 28 GDPR -- obligation to include data processed by them)
- **Video surveillance / CCTV** (to the extent recordings still exist and the individual is identifiable)
- **Backup / archive systems** (see Step 5 on exceptions under BDSG Section 34)

**BGH VI ZR 576/19:** Internal memos, call notes, and file notes about the individual are personal data and are in principle subject to disclosure.

### Step 5: Review Exceptions

Not all data found must or may be disclosed:

**Art. 15(4) GDPR -- Rights of third parties:**
The right to obtain a copy must not adversely affect the rights and freedoms of others. Third-party data must be redacted (but not excessively -- only the third party's personal data, not the entire context).

**BDSG Section 34(1) -- Disproportionate effort:**
- Data in backup or archive systems stored only for technical reasons or retention purposes, where disclosure would require disproportionate effort.
- This exception must be interpreted narrowly and documented.

**BDSG Section 29(1) sentence 2 -- Employee data in legal disputes:**
- The right of access may be restricted to the extent that the data serve exclusively the assertion, exercise, or defence of legal claims and disclosure would jeopardise those claims.
- This exception must be applied restrictively (BAG 2 AZR 342/20: employees generally have a broad right of access).

**Trade secrets (Geschaeftsgeheimnisse):**
- Trade secrets do not justify a blanket refusal, but they may be taken into account in how the information is provided (e.g., a summary instead of raw data for scoring algorithms).

### Step 6: Prepare Data

**Redaction:**
- Consistently redact third-party personal data.
- Do not over-redact: the CJEU (C-487/21) requires a "faithful and intelligible reproduction" -- where there is doubt, complete documents (not just summaries) must be disclosed.
- Clearly mark redactions (e.g., "[third-party name redacted]").

**Format:**
- Art. 12(1) GDPR: The information must be provided "in a concise, transparent, intelligible and easily accessible form, using clear and plain language."
- For electronic requests: respond in a commonly used electronic format (Art. 15(3) sentence 3 GDPR), e.g. PDF.
- The first copy is free of charge (Art. 15(3) sentence 1 GDPR). For additional copies, a reasonable fee based on administrative costs may be charged.

**Structure of the response:** Cover letter + structured disclosure (mandatory information) + data copy.

### Step 7: Draft the Response

The response consists of three parts:

**Part 1 -- Cover letter:**
- Reference to the request (date, channel)
- Confirmation of whether personal data is being processed
- Reference to the enclosed disclosure and data copy
- Contact person for follow-up questions
- Notice of the right to lodge a complaint with the competent supervisory authority (Aufsichtsbehoerde)

**Part 2 -- Structured disclosure under Art. 15(1)(a)-(h):** (see mandatory disclosures checklist below)

**Part 3 -- Data copy (Art. 15(3)):**
- Complete copy of the personal data being processed.
- CJEU C-487/21: "faithful and intelligible reproduction" -- for documents, this may mean disclosing entire documents (not just extracts).

### Step 8: Dispatch and Documentation

- **Secure delivery method:** Encrypted email, secure portal, or registered post. Never send unencrypted email to unverified addresses.
- **Proof of dispatch:** Delivery receipt (registered mail receipt, email delivery confirmation, portal download log).
- **Internal documentation:** Create a complete file containing the request, internal processing history, the response as sent, proof of dispatch, and any justification for restrictions applied.
- **Retention:** Retain documentation for at least 3 years (limitation period for damages claims, Section 195 BGB).

## Mandatory Disclosures Checklist

The following information must be included in the response (Art. 15(1)(a)-(h) GDPR):

| No. | Mandatory Disclosure | Content / Notes |
|---|---|---|
| a | Purposes of processing | Specify all purposes per data category |
| b | Categories of data | Master data, contact data, contractual data, payment data, usage data, etc. |
| c | Recipients | Name specific recipients, not just categories (CJEU C-154/21). Recipients in third countries must be listed separately |
| d | Storage period | Specific duration or criteria for determining it |
| e | Data subject rights | Notice of right to rectification (Art. 16), erasure (Art. 17), restriction (Art. 18), objection (Art. 21) |
| f | Right to complain | Right to lodge a complaint with a supervisory authority |
| g | Data source | If data was not collected from the data subject: state the source |
| h | Automated decisions | Automated individual decision-making including profiling (Art. 22): explain the logic involved, significance, and envisaged consequences |
| -- | Third-country transfers | State appropriate safeguards under Art. 46 GDPR (Art. 15(2)) |

## Special Cases

**Request by a current employee:**
- BAG 2 AZR 342/20: Broad right of access. The personnel file (Personalakte) must in principle be disclosed in full.
- BDSG Section 29 applies only within narrow limits (only where a specific legal dispute exists and only for data relevant to that dispute).
- Performance reviews, internal memos, and formal warnings (Abmahnungen) are personal data.

**Request by a former employee:**
- The right of access continues to exist after the employment relationship has ended, as long as data is being processed.
- Check retention periods: payroll and salary records (6 or 10 years), personnel file (no statutory requirement, but typically 3 years after departure).

**Request through a lawyer:**
- Require written power of attorney (Vollmacht) (original or certified copy).
- Send the response to the lawyer, not directly to the data subject (unless the data subject requests otherwise).
- The deadline runs from receipt of the request, not from submission of the power of attorney.

**Mass requests (e.g. GDPR activism):**
- Art. 12(5) GDPR: For manifestly unfounded or excessive requests, a reasonable fee may be charged or compliance may be refused.
- The burden of proof for the "excessive" nature of the request lies with the controller.
- The threshold is high: a single request, even a comprehensive one, is generally not considered excessive.

## Common Mistakes

| Mistake | Risk | Recommendation |
|---|---|---|
| Incomplete system search | Incomplete disclosure, fine | Use the Art. 30 record of processing activities as a checklist |
| Data from processors missing | Incomplete disclosure | Include processors (Auftragsverarbeiter) and factor in their response time |
| Excessive redaction | Violation of access right | Redact only third-party personal data, not the entire context |
| Missed deadline | Fine, damages | Communicate any extension in good time |
| Blanket demand for ID copy | Data protection violation, delay | Use proportionate, channel-appropriate verification |
| Confusing Art. 15 with Art. 20 | Incorrect response | Art. 15 = all processed data; Art. 20 (data portability) = only automatically processed data provided by the data subject |
| Naming only data categories instead of specific recipients | Violation since CJEU C-154/21 | Name specific recipients where the data subject requests it |
| Providing only a summary instead of document copies | Violation since CJEU C-487/21 | Assess whether full documents must be disclosed |
| Response sent to wrong recipient | Data breach (Art. 33/34) | Always verify recipient identity |

## Fines and Damages Risk

**Fines (Art. 83(5) GDPR):**
Violations of data subject rights (Art. 12-22) fall into the highest fine category: up to EUR 20 million or 4% of annual worldwide turnover (whichever is higher).

**Damages (Art. 82 GDPR):**
- Any person who has suffered material or non-material damage as a result of a GDPR violation has a right to compensation.
- CJEU C-300/21: No de minimis threshold -- even minor non-material damages are compensable.
- German courts typically award between EUR 100 and EUR 5,000 in non-material damages for late or incomplete access responses.
- Trend is upward: claims aggregators and legal tech providers are increasingly bundling claims.

## Limitations of This Skill

This skill provides a structured working aid for standard cases. For the following scenarios, we recommend seeking advice from a lawyer:

- Manifestly unfounded or excessive requests where refusal is being considered
- Concurrent supervisory proceedings or complaints filed with a data protection authority (Datenschutzbehoerde)
- Complex third-country transfers or international group structures
- Conflicts between the right of access and third-party rights, trade secrets, or ongoing legal proceedings
- Damages claims or judicial enforcement of the right of access
- Mass requests by legal tech providers or activists
