---
name: terms-check
description: 'Reviews general terms and conditions for validity under German law. Detects invalid clauses and violations of §§ 305-310 BGB.'
---


## 1. Overview

This skill systematically reviews **standard business terms (Allgemeine Geschäftsbedingungen, AGB)** for validity under §§ 305--310 BGB. German law on standard terms follows a **three-layer review**:

1. **Incorporation review** (§ 305) -- Did the terms actually become part of the contract?
2. **Interpretation review** (§ 305c) -- Does the text contain surprising or ambiguous clauses?
3. **Content review** (§§ 307--309) -- Are individual clauses substantively invalid?

Review each layer in sequence. If a clause already fails at the incorporation stage, the content review is unnecessary.

**Important:** Individually negotiated terms always take precedence over standard terms (§ 305b BGB) -- even an oral agreement overrides a written standard clause. Therefore, always check first whether an individual agreement exists.

SaaS and cloud service terms require additional review under the [SaaS Agreement Review](/en-DE/skills/saas-agreement/) skill for SLA commitments, exit provisions, and EU Data Act portability rights. Terms that involve data processing activities must be supplemented by a compliant [Data Processing Agreement](/en-DE/skills/data-processing-agreement/) under Art. 28 GDPR. Where terms include confidentiality provisions, these must also satisfy the requirements of a valid [NDA under German law](/en-DE/skills/nda-review/).


## 2. Review Framework

### Step 1: Are These Standard Terms? (§ 305 para. 1 BGB)

Standard business terms are all **contract terms pre-formulated for a multitude of contracts** that one party imposes on the other at the time of contracting.

Check for the following elements:

- **Pre-formulated:** The text was drafted before the contract was concluded. Even first-time use qualifies if the drafter intends to use the clauses in at least 3 further contracts (BGH NJW 2014, 1725).
- **Multitude of contracts:** The intent to use the terms repeatedly is sufficient; actual repeated use is not required.
- **Imposition (Stellen):** One party unilaterally dictates the terms. Genuinely negotiating individual clauses converts them into individually negotiated terms. Merely "walking through" the terms without real negotiation does not suffice (BGH NJW 2016, 1230).

**Distinguishing individually negotiated terms:** An individual agreement exists only if the drafter genuinely offered the clause for negotiation and the other party had the opportunity to influence its substance. The burden of proof lies with the drafter (§ 305 para. 1 sentence 3 BGB).


### Step 2: Incorporation Review (§ 305 para. 2 BGB)

Standard terms only become part of the contract if **all three requirements** are met:

1. **Express reference** to the terms at the time of contracting (or a clearly visible notice, if an express reference would be disproportionately difficult)
2. **Reasonable opportunity to review** -- the customer must be able to access the full text
3. **Consent** from the customer

**Online specifics:**

| Method | Valid? | Reasoning |
|---|---|---|
| **Click-wrap** (checkbox + link to full text) | Yes | Express consent + opportunity to review |
| **Browse-wrap** (terms linked in footer, no active consent) | **No** | No express reference, no provable consent (BGH NJW 2006, 2976) |
| **Sign-in-wrap** (notice at registration: "By registering, you accept...") | Borderline | Only valid if sufficiently prominent and linked |

**Offline specifics:** For oral or telephone contracts, the drafter must provide the terms before the contract is concluded. Sending them afterwards (e.g., on the invoice) is insufficient.

**Note for B2B:** § 305 para. 2 does not apply to businesses (§ 310 para. 1 sentence 1 BGB). Here, a reasonable opportunity to review is sufficient. Tacit incorporation through industry custom is possible.


### Step 3: Surprising Clauses (§ 305c BGB)

**§ 305c para. 1 -- Surprising clauses:** Provisions that are so unusual under the circumstances that the other party need not expect them do not become part of the contract.

Check for the **element of surprise**:

- The clause appears in an unexpected location (e.g., a non-compete clause in a price list)
- The clause does not match the outward appearance of the contract (e.g., a liability waiver in delivery terms)
- The clause deviates significantly from default law or ordinary expectations

Typical examples of surprising clauses:
- Liability waiver hidden in payment terms
- Non-compete obligation in the standard terms of a freelancer agreement
- Automatic renewal with a long lock-in period in a trial-month offer
- Assignment prohibition in standard purchasing terms

**§ 305c para. 2 -- Ambiguity rule (contra proferentem):** Doubts in interpretation are resolved against the drafter. If a clause allows two readings, the more customer-friendly interpretation applies.


### Step 4: Prohibited Clauses Without Discretion (§ 309 BGB)

These clauses are **per se invalid** -- there is no room for judicial discretion. Review the following key provisions:

| No. | Prohibition | What to check | Most common error |
|---|---|---|---|
| **No. 5** | Liquidated damages | The clause must expressly allow the customer to **prove that the actual loss was lower** | Missing right to prove lower damages |
| **No. 6** | Contractual penalties | The clause must be proportionate; no contractual penalty for mere payment obligations | Contractual penalty for late payment |
| **No. 7a** | Liability exclusion for **personal injury** | Liability for personal injury can **never be excluded** | "Liability for damages of any kind is excluded" |
| **No. 7b** | Liability exclusion for **intentional or grossly negligent** conduct | Liability for intent and gross negligence can **never be excluded** | Blanket liability exclusion without differentiation |
| **No. 8** | Warranty rights | No unreasonable shortening or restriction; for new goods, the limitation period must not be less than 1 year | Warranty exclusion for new goods |
| **No. 9** | Contract duration and notice periods | Maximum initial term of **2 years**; since 01.03.2022 for B2C: after the initial term, the consumer can cancel at any time with **1 month's** notice (no automatic renewal exceeding 1 month) | Automatic 12-month renewal under pre-reform practice |
| **No. 12** | Reversal of the burden of proof | No shifting the burden of proof to the customer's disadvantage | "The customer must prove that the defect existed at the time of delivery" |
| **No. 13** | Form requirements | Since 01.10.2021: cancellation in **text form** (§ 126b BGB) must be sufficient; requiring written form (Schriftform, § 126 BGB) for cancellations is invalid | "Cancellation requires written form" instead of text form |


### Step 5: Prohibited Clauses With Discretion (§ 308 BGB)

These clauses are invalid **insofar as they are unreasonable** -- here, the court has discretion.

| No. | Prohibition | Permissibility threshold |
|---|---|---|
| **No. 1** | Unreasonably long deadlines for acceptance or performance | The deadline must be objectively justified and industry-standard; in e-commerce: a delivery period exceeding 30 days without a specific reason is problematic |
| **No. 4** | Modification reservation | The right to modify must be **specifically described** (which service features, to what extent, for what reason); the **core performance** (what the customer pays for) must be preserved; the BGH requires disclosure of the reasons for modification (BGH NJW 2021, 1752) |
| **No. 5** | Deemed declarations (silence as consent) | Only valid if the customer is given a **reasonable deadline** and is **expressly informed of the consequences of silence** at the start of that period |
| **No. 7** | Unwinding after withdrawal | The drafter may not demand unreasonable compensation for use or depreciation |
| **No. 8** | Set-off prohibition | Only valid if limited to undisputed or legally established counterclaims |


### Step 6: General Clause (§ 307 BGB)

The **catch-all provision** for all clauses not already covered by §§ 308, 309. A clause is invalid if it **unreasonably disadvantages** the other party.

Three pillars of review:

**a) Transparency requirement (§ 307 para. 1 sentence 2):**
- The clause must be **clear and comprehensible**
- Opaque price adjustment clauses, hidden ancillary fees, and chains of cross-references to other documents regularly violate this requirement
- BGH: Any clause whose economic impact the average customer cannot assess is intransparent (BGH NJW 2014, 2269)

**b) Guiding principle of default law (§ 307 para. 2 no. 1):**
- A clause is unreasonable if it deviates from **essential principles of the statutory regime**
- Example: A complete exclusion of the right to withdraw for breach of duty contradicts the guiding principles of §§ 323 et seq. BGB

**c) Cardinal obligations (Kardinalspflichten) (§ 307 para. 2 no. 2):**
- Clauses that restrict **essential rights and obligations** to such an extent that the purpose of the contract is jeopardized are invalid
- **Cardinal obligations** are those whose fulfillment is essential for the proper performance of the contract and on which the other party may regularly rely
- Typical issue: Liability exclusion for slight negligence in breach of cardinal obligations without limiting liability to the foreseeable, contract-typical loss

**Valid liability clause structure:**
1. Liability for intent and gross negligence: unlimited
2. Liability for breach of cardinal obligations through slight negligence: limited to the foreseeable, contract-typical loss
3. Liability for personal injury: unlimited
4. Liability under the Product Liability Act (Produkthaftungsgesetz): unlimited


### Step 7: B2B Specifics (§ 310 para. 1 BGB)

In **business-to-business transactions**, the following deviations apply:

- §§ 308 and 309 BGB are **not directly applicable**
- **However:** Their underlying principles inform the general clause of § 307 BGB (so-called **indicative effect**, Indizwirkung)
- The BGH asks: If a clause would be per se invalid under § 309 BGB in a B2C context, this constitutes a **strong indication** of unreasonable disadvantage under § 307 BGB in a B2B context as well
- B2B is **not a free pass** -- the BGH regularly strikes down clauses between businesses too

**What is additionally permissible in B2B (compared to B2C):**
- Shorter warranty periods (e.g., 1 year, BGH NJW 2013, 291)
- Liability caps tied to the contract value (if proportionate)
- Stricter inspection and notice-of-defect obligations (commercial traders: § 377 HGB)
- Choice-of-forum clauses

**What is regularly invalid even in B2B:**
- Complete liability exclusion for gross negligence
- Liability exclusion for cardinal obligations without a cap
- Unreasonably short limitation periods (under 1 year)
- Unilateral modification reservations without specificity


## 3. Industry-Specific Review Points

### SaaS and Cloud Services

- **Modification reservation (§ 308 no. 4):** Feature changes must be specified; the core functionality must be preserved; a generic "We may modify the service at any time" is invalid
- **Availability/Uptime:** Review SLA clauses; a clause stating "Availability on a best-efforts basis" without a concrete SLA commitment may undermine a cardinal obligation
- **Data portability:** Check whether the customer is provided with a **data export** in a common format upon contract termination; absence may violate § 307
- **Unilateral price adjustment:** Only valid with concrete adjustment criteria and a special right of termination; pure inflation clauses without a cap are problematic

### E-Commerce (B2C)

- **Right of withdrawal:** 14-day cooling-off period under § 355 BGB; the withdrawal notice must conform to the statutory model; a defective notice extends the period to 12 months + 14 days
- **Button solution (§ 312j para. 3 BGB):** The order button must be labeled "order with obligation to pay" (zahlungspflichtig bestellen) or an equally unambiguous wording; violations render the contract void
- **Delivery periods:** "Delivery approx. 2--4 weeks" is borderline as a standard clause; concrete delivery dates or maximum periods are required

### Marketplaces and Platforms

- **P2B Regulation (EU 2019/1150):** Platform terms must disclose **ranking parameters**, **grounds for differentiation**, and **notice periods** (at least 30 days)
- **Suspension rights:** Unilateral suspension of merchant accounts without a hearing and stated reasons is impermissible
- **Data access:** Check whether the platform adequately regulates access to business-relevant data of commercial users


## 4. Legal Consequences of Invalidity (§ 306 BGB)

**No partial enforcement to the permissible extent (keine geltungserhaltende Reduktion).** This is the central principle: An invalid clause is **not** reduced to the maximum permissible scope. Instead:

1. **§ 306 para. 1:** The contract remains valid in all other respects
2. **§ 306 para. 2:** The invalid clause is replaced by **default statutory law** -- in full, not "improved"
3. **§ 306 para. 3:** Only if upholding the contract would constitute an **undue hardship** for one party is the entire contract invalid

**Severability clauses** that attempt to replace invalid clauses with the "nearest valid alternative" (so-called replacement clauses) are **themselves invalid** because they circumvent the prohibition on partial enforcement (BGH NJW 2018, 2950). Pure preservation clauses ("The contract remains valid in all other respects") are unproblematic, as they merely restate § 306 para. 1.


## 5. Commonly Invalid Clauses

| Clause | Reason for invalidity | Provision |
|---|---|---|
| "Liability for damages of any kind is excluded" | Covers personal injury and gross negligence | § 309 No. 7 |
| "Cancellation requires written form" | Text form is the maximum requirement since 01.10.2021 | § 309 No. 13 |
| "The contract renews automatically for 12 months" (B2C) | Maximum one-month renewal after the initial term since 01.03.2022 | § 309 No. 9 |
| "Place of jurisdiction is [drafter's registered office]" (B2C) | Impermissible choice-of-forum clause with consumers | § 38 ZPO in conjunction with § 307 BGB |
| "We reserve the right to modify the service at any time" | Too vague, no specificity, core performance not preserved | § 308 No. 4 |
| "Upon receipt of the invoice, the service is deemed accepted" | Deemed declaration without notice and deadline | § 308 No. 5 |
| "Warranty claims expire after 6 months" (new goods, B2C) | At least 1 year for new goods | § 309 No. 8 |
| "Liquidated damages of 25% of the order value" (without right to prove lower damages) | Right to prove lower damages missing | § 309 No. 5 |
| "Withdrawal only in written form and within 3 days" | Double violation: form requirement + shortened deadline | § 309 No. 13, § 307 |
| Severability clause with replacement mechanism | Circumvents the prohibition on partial enforcement | § 306 BGB |


## 6. Limitations of This Skill

This skill provides a **structured preliminary assessment**. For the following scenarios, we recommend consulting a lawyer at [compound.law](https://compound.law):

- **Drafting new terms** (not just reviewing existing clauses)
- **International matters** involving choice-of-law and choice-of-forum clauses
- **Industry-specific regulation** (financial services, insurance, telecommunications, healthcare)
- **Cease-and-desist letters** due to invalid terms under the UWG or UKlaG
- **Collective action risk** by consumer protection associations (Verbraucherschutzverbände)
- **Conflicts with GDPR clauses** (data processing agreements, privacy notices)
- **Competition law considerations** in cases of market dominance

This analysis does not replace legal advice. The law of standard business terms is highly fact-specific -- clauses that are valid in one context may be invalid in another.
