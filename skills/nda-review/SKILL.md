---
name: nda-review
description: 'AI-powered guide for analyzing non-disclosure agreements under German law. Identifies risks, missing clauses, and non-standard terms.'
---


## Overview

This skill guides the systematic review of non-disclosure agreements (NDAs) under German law. It covers unilateral and mutual NDAs, pre-contractual confidentiality arrangements, M&A NDAs, and employee confidentiality agreements. The goal is to identify risks, missing clauses, and non-standard terms before they become a problem.

NDAs qualify as **reasonable protective measures** within the meaning of **§ 2 No. 1 lit. b GeschGehG** (German Trade Secrets Act) and are therefore a prerequisite for statutory trade secret protection. A defective NDA can cause trade secrets to lose their protected status entirely.


## Systematic Review

### Step 1: Basic Structure

Start by checking the formal foundations:

- **Parties:** Full company name including legal form (GmbH, AG, UG, etc.), registered office, commercial register number, and authority to represent. For corporate groups: Is only the parent company a party, or are subsidiaries included?
- **Unilateral or mutual:** Who discloses, who receives? For mutual NDAs, check whether the obligations are truly symmetrical or whether one side bears a heavier burden.
- **Purpose limitation:** Is the purpose of disclosure clearly defined? An NDA without a specific purpose (e.g., "evaluation of a potential cooperation in the area of X") is too broad and difficult to enforce.
- **Subject matter:** Does the NDA relate to a specific project, a due diligence exercise, or a general business relationship?

**Flag as risk:**
- Missing or unclear authority to represent
- Purpose clause missing entirely
- Unilateral NDA labelled as "mutual" even though only one party discloses

### Step 2: Definition of Confidential Information

The definition is the heart of every NDA. Check:

- **Specificity:** Is it clearly identifiable which information is protected? A blanket clause ("all information exchanged in the course of the collaboration") is problematic.
- **Marking requirement (Kennzeichnungspflicht):** Must the disclosing party mark information as "confidential"? If so: Does this also apply to oral disclosures (standard practice: written confirmation within 14-30 days after the fact)?
- **Scope:** Are the following categories adequately covered?
  - Technical information (source code, prototypes, algorithms)
  - Business information (customer lists, pricing, strategies)
  - Orally disclosed information
  - Visually observed information (e.g., during site visits)

**Flag as risk:**
- Definition is so broad that practically any information is captured -- this is vulnerable to challenge under standard terms law (§ 307 BGB)
- No marking requirement and no restriction to the defined purpose
- "Residual knowledge" clause allowing the recipient to use anything an employee can recall from memory -- this effectively hollows out the protection

### Step 3: Exceptions

An NDA must contain **five standard exceptions**. If any are missing, that is a warning sign:

1. **Already publicly known** -- the information was already in the public domain at the time of disclosure
2. **Subsequently became public** -- without fault on the part of the recipient
3. **Already in possession** -- the recipient already had the information before disclosure (proof required)
4. **Independently developed** -- the recipient developed the information on its own
5. **Lawfully received from a third party** -- without breach of any confidentiality obligation

**Additional checks:**
- **Mandatory disclosure to authorities or courts:** Is there an exception for legally compelled disclosure? The recipient should be permitted to notify the disclosing party before disclosure (to the extent legally permissible).
- **Whistleblower protection:** An NDA cannot effectively exclude protection under **§ 5 GeschGehG** and the **Whistleblower Protection Act (Hinweisgeberschutzgesetz, HinSchG)**. Clauses purporting to prohibit whistleblowing are void. Check whether the NDA overreaches here.

**Flag as risk:**
- "Already in possession" exception missing -- this is a significant risk for the recipient
- Burden of proof for exceptions shifted entirely to the recipient
- No exception for mandatory legal disclosure obligations

### Step 4: Duration and Survival Period

Check the total duration (contract term + survival period) against these benchmarks:

| Context | Market-standard survival period | Upper limit |
|---|---|---|
| **B2B cooperation** | 2-5 years after contract end | 3 years most common |
| **Employment agreement** | Contract duration + 1-2 years | 2 years after departure |
| **M&A / Due diligence** | 2-3 years after closing/abandonment | 3 years |
| **Technology licence** | 3-5 years after contract end | 5 years |

**Checkpoints:**
- Is the survival period clearly defined, or does the NDA apply "indefinitely"? Indefinite NDAs are generally permissible under German law but uncommon in practice and carry enforcement risks.
- Is there an ordinary termination right? For ongoing contractual relationships (Dauerschuldverhaltnisse), the absence of one can be problematic (§ 314 BGB: the right to extraordinary termination for good cause remains unaffected in any event).
- For employee NDAs: If the survival period exceeds 2 years, particular caution is warranted.

**Flag as risk:**
- Indefinite duration without any termination right
- Survival period exceeding 5 years without objective justification
- Employee NDA with a survival period exceeding 2 years

### Step 5: Contractual Penalty (Vertragsstrafe)

The contractual penalty (Vertragsstrafe, §§ 339-345 BGB) is the central enforcement mechanism in German NDAs. Review systematically:

**Existence and structure:**
- Is a contractual penalty agreed at all? Without one, the disclosing party is limited to damages claims, which require proof of actual loss -- often extremely difficult in confidentiality breaches.
- Is the penalty structured as a lump sum or under the **Hamburg Custom (Hamburger Brauch)** model (the amount is determined by the creditor in the event of a breach and subject to judicial review for reasonableness)?

**Appropriateness of the amount:**

| Context | Market-standard range | Upper limit (guideline) |
|---|---|---|
| **Employment agreement** | 1-3 gross monthly salaries | Per breach |
| **B2B SME** | EUR 10,000 - 50,000 | Per breach |
| **B2B large enterprise** | EUR 50,000 - 500,000 | Per breach |
| **M&A** | Individually negotiated, often higher | Tied to transaction value |

**Hamburg Custom (Hamburger Brauch):**
- The creditor sets the amount upon breach; the debtor may request judicial review.
- Advantage: More flexible than a fixed lump sum. Disadvantage: Uncertainty about the actual amount.
- In practice, this is the most common approach in B2B NDAs.

**Note for merchants (Kaufleute):** Between merchants (§ 348 HGB), the court **cannot** reduce the contractual penalty (§ 343 BGB does not apply). This makes agreeing on a reasonable amount particularly important.

**Flag as risk -- disclosing party:**
- No contractual penalty agreed
- Contractual penalty triggered only by intentional breach (not negligence)

**Flag as risk -- receiving party:**
- Contractual penalty without any cap ("unlimited" or cumulating per breach without a ceiling)
- No option for judicial review (void under § 307 BGB in standard terms)
- Contractual penalty triggered even by slight negligence without any graduated fault requirement

### Step 6: Return and Destruction Obligations

Check what happens to confidential information upon contract termination or on request:

- **Return or destruction:** Is it specified whether materials must be returned, destroyed, or both?
- **Confirmation obligation:** Must destruction be confirmed in writing?
- **Exceptions for statutory retention requirements:** The recipient must be allowed to retain materials where statutory retention obligations apply (e.g., commercial and tax law: 6-10 years). If this exception is missing, an irreconcilable conflict arises.
- **Electronic copies:** Does the agreement address how backups, email archives, and cloud storage are to be handled? Complete deletion of electronic copies is often technically impossible (backup systems). A workable clause acknowledges this reality.
- **Deadline:** Is a reasonable deadline for return/destruction provided (standard: 14-30 days)?

**Flag as risk:**
- No return/destruction provision at all
- No exception for statutory retention obligations
- Unrealistic deletion requirements for electronic copies

### Step 7: Standard Terms Control (AGB-Kontrolle)

An NDA is subject to **standard terms control (§§ 305 ff. BGB)** if it was pre-formulated by one party and presented to the other on a take-it-or-leave-it basis. This applies to the vast majority of NDAs.

**Check for typical standard terms pitfalls:**

- **Surprising clauses (§ 305c BGB):** Clauses that are unexpected in an NDA, such as a hidden non-compete or an exclusivity arrangement.
- **Unreasonable disadvantage (§ 307 BGB):**
  - Excessively broad definition of confidential information (everything is confidential)
  - Disproportionately high contractual penalty without judicial review
  - Reversal of the burden of proof to the recipient's detriment for all exceptions
  - One-sided indemnification obligation without any cap
- **Transparency requirement (§ 307(1) sentence 2 BGB):** Unclear or contradictory language works against the party that drafted the terms.

**Legal consequence of invalidity:** Invalid clauses are struck without replacement (§ 306 BGB). The remainder of the contract survives. Under German standard terms law, there is no "blue-pencil reduction" (geltungserhaltende Reduktion) -- the clause does not apply in a reduced form; it is void entirely.

**Flag as risk:**
- NDA contains a hidden non-compete
- Liquidated damages clause with no option to prove lower actual damages
- Complete reversal of burden of proof for all exception grounds

### Step 8: Trade Secrets Act Compliance (GeschGehG)

Since the **German Trade Secrets Act (Geschäftsgeheimnisgesetz, GeschGehG)** came into force in 2019, an NDA alone is no longer sufficient to protect trade secrets. Check:

- **Reasonable protective measures (§ 2 No. 1 lit. b GeschGehG):** The NDA is one such measure, but not the only one required. Does the NDA reference supplementary technical and organisational measures?
- **Reverse engineering (§ 3(1) No. 2 GeschGehG):** Reverse engineering of a lawfully obtained product is generally permitted. An effective exclusion must be explicitly agreed in the NDA. Check: Is a reverse-engineering prohibition included, and is it proportionate?
- **Permitted actions (§ 5 GeschGehG):** Disclosure in the legitimate interest of the public (whistleblowing, uncovering unlawful conduct) cannot be excluded by NDA.
- **Legitimate interest in secrecy (§ 2 No. 1 lit. a GeschGehG):** The information must derive economic value specifically from its secrecy. Trivial information cannot be elevated to trade secret status simply by including it in an NDA.

**Flag as risk:**
- NDA contains no reference to supplementary protective measures
- Reverse-engineering exclusion missing despite products/software being disclosed
- NDA attempts to exclude § 5 GeschGehG (void)


## Risk Assessment

### Red Flags: Disclosing Party's Perspective

| Red Flag | Risk | Recommended Action |
|---|---|---|
| No contractual penalty (Vertragsstrafe) | Enforcement limited to damages claims (evidentiary burden) | Include a contractual penalty, at minimum under the Hamburg Custom model |
| Residual knowledge clause | Recipient may use anything retained in memory | Delete the clause or restrict it to general professional knowledge |
| Broad "affiliates" sharing | Confidential information flows uncontrolled across group companies | Limit sharing to named entities or require prior consent |
| No reverse-engineering exclusion | Products may be analysed (§ 3(1) No. 2 GeschGehG) | Include an express prohibition |
| No return obligation | Information remains permanently with the recipient | Add a return/destruction clause with written confirmation requirement |
| No injunctive relief right | Only damages, no ability to halt a breach quickly | Include a contractual cease-and-desist obligation with interim relief clause |

### Red Flags: Receiving Party's Perspective

| Red Flag | Risk | Recommended Action |
|---|---|---|
| Excessively broad definition | Practically any information is confidential | Restrict to the defined purpose, require marking |
| No "prior knowledge" exception | Recipient is liable for information already in its possession | Include all five standard exceptions |
| Contractual penalty without cap | Potentially existential liability exposure | Agree on a reasonable cap or use the Hamburg Custom model |
| Indefinite duration | Perpetual obligation with no exit | Limit survival period to 2-3 years |
| Hidden non-compete | Restriction on business activities without consideration | Void as a surprising clause under standard terms law (§ 305c BGB); insist on removal |
| Comprehensive indemnification obligation | Recipient liable for all damages, including disproportionate ones | Limit to intent and gross negligence |


## Special Scenarios

### Employee Confidentiality Agreements

Employee NDAs are subject to particular restrictions:

- **General professional skills and industry knowledge** cannot be restricted post-employment. An NDA that prohibits an employee from using acquired skills and general industry knowledge in a new role is void.
- **Disguised non-compete:** If an NDA effectively prevents an employee from working in their professional field, it constitutes a post-contractual non-compete. This requires **compensation during the restriction period (Karenzentschadigung)** of at least 50% of the most recent remuneration (§ 74(2) HGB). Without such compensation, the clause is void under established Federal Labour Court (BAG) case law.
- **Contractual penalty (Vertragsstrafe):** For employees, a maximum of 1-3 gross monthly salaries per breach. Higher penalties are regularly deemed disproportionate by the courts.
- **Standard terms control:** Employment contracts and their annexes (including NDAs) are always subject to standard terms control (§ 310(4) BGB, with the particularities of employment law taken into account).

**Key question:** Can the employee realistically work in their professional field after leaving without breaching the NDA? If not: disguised non-compete.

### Cross-Border NDAs

US and common-law NDAs typically contain features that are problematic under German law:

- **Indefinite duration** ("in perpetuity") -- uncommon in Germany and concerning for employee NDAs.
- **Missing standard exceptions** -- US NDAs frequently omit the "already in possession" or "independently developed" exceptions.
- **Overly broad definitions** -- "Confidential Information means any and all information" is vulnerable to challenge under German standard terms law.
- **Injunctive relief clause** -- References to injunctive relief under US law have no effect in Germany.
- **Choice of law clause:** Check which law governs. For employees whose habitual place of work is in Germany, German employment law applies mandatorily (Art. 8 Rome I Regulation), regardless of the contractual choice of law.

**Recommendation:** Adapt US-standard NDAs for the German legal environment. At a minimum: add standard exceptions, limit duration, and ensure compliance with standard terms law.

### M&A / Due Diligence

M&A NDAs have particular requirements:

- **Non-solicitation:** Prohibitions on soliciting employees and customers are standard in M&A NDAs but should be limited in duration (12-24 months).
- **Standstill clause:** Prohibition on hostile takeover approaches for a defined period. Review separately for appropriateness.
- **Sharing with advisors:** Provisions governing the involvement of lawyers, auditors, and financial advisors, with their own confidentiality obligations.
- **Clean team arrangement:** Where competitors enter into due diligence, the NDA must specify which individuals have access to which categories of information.
- **Shorter survival period:** 2-3 years is market standard, as M&A information loses relevance more quickly.


## Limitations of This Skill

This skill provides a structured initial analysis. In the following cases, engaging a lawyer is necessary:

- **Negotiation and drafting** of complex NDA clauses, particularly contractual penalties (Vertragsstrafe) and liability provisions
- **M&A transactions** with significant transaction values or involving multiple jurisdictions
- **Cross-border NDAs** where multiple legal systems interact
- **Industry-specific requirements** (regulated industries such as pharmaceuticals, defence, financial services)
- **Disputes** arising from existing NDAs, particularly contractual penalty claims
- **Employee NDAs with non-compete characteristics** that require an individual assessment of the compensation obligation (Karenzentschadigung)

Compound is happy to assist with the review, negotiation, and drafting of NDAs that meet the requirements of German law.
