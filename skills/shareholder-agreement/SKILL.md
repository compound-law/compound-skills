---
name: shareholder-agreement
description: 'Structured review of shareholder agreements under German corporate law. Covers voting rights, transfer restrictions, and exit provisions.'
---


## Overview

This skill guides the structured review of shareholder agreements (Gesellschaftervereinbarungen) for German limited liability companies (GmbH). The GmbH is governed by the GmbHG, but shareholder agreements layer additional rights and obligations on top of the articles of association (Gesellschaftsvertrag). Key statutory references include **§ 47 GmbHG** (voting rights), **§ 15 GmbHG** (transfer of shares), **§ 53 GmbHG** (amendments to the articles), and **§ 29 GmbHG** (profit distribution). Use this skill whenever a client enters, renegotiates, or exits a GmbH shareholding structure, or when conducting due diligence on a target company's governance framework.

A well-drafted shareholder agreement must address the gap between the relatively sparse GmbHG defaults and the practical needs of multi-party ventures. German courts apply strict standards to contractual penalties, non-compete clauses, and transfer restrictions in shareholder agreements, making careful drafting and review essential. Unlike the articles of association, a shareholder agreement binds only its parties as a matter of contract law (schuldrechtliche Vereinbarung) and is not filed with the commercial register -- this creates both flexibility and enforcement risks that must be understood from the outset.


## Systematic Review

### Step 1: Shareholder Structure and Voting Thresholds

Identify each shareholder's percentage, nominal value (Nennbetrag), and any deviations from the statutory one-vote-per-EUR rule (§ 47 Abs. 2 GmbHG). Check whether the agreement introduces qualified majority requirements beyond the statutory thresholds.

- **Shareholding percentages and nominal values:** Verify that the percentages listed in the agreement match the commercial register entries. Even small rounding differences can matter when thresholds are at play.
- **Statutory majorities:** 75% for amendments to the articles (§ 53 Abs. 2 GmbHG), simple majority for ordinary resolutions (§ 47 Abs. 1 GmbHG). Any deviation from these thresholds must be clearly documented.
- **Veto rights and reserved matters (Zustimmungsvorbehalte):** Review the catalogue of reserved matters that require unanimous consent or a supermajority. Typical reserved matters include changes to the business purpose, capital increases or decreases, appointments of managing directors, annual budgets exceeding a threshold, related-party transactions, and entry into material contracts.
- **Voting agreements (Stimmbindungsvereinbarungen):** Confirm whether voting agreements exist and whether they are enforceable. A voting agreement creates a contractual obligation to vote in a particular way; breach entitles the other party to damages but does not automatically invalidate the resolution. Consider whether pooling arrangements are used to aggregate voting power among certain shareholders.
- **Quorum rules:** Check whether minimum attendance or representation requirements exist for shareholder meetings (Gesellschafterversammlungen). The GmbHG does not prescribe a quorum, so decisions can theoretically be taken with minimal attendance unless the agreement provides otherwise.

**Flag as risk:**
- Minority shareholder holds a de facto veto through supermajority requirements without corresponding obligations or fiduciary duties
- Voting agreements that are not mirrored in the articles of association, creating a gap between the corporate and contractual level
- No quorum rules, allowing decisions to be taken with minimal attendance
- Reserved matters catalogue either too broad (leading to deadlock) or too narrow (exposing minorities to unchecked majority decisions)

### Step 2: Transfer Restrictions and Pre-Emption Rights

Under § 15 Abs. 5 GmbHG, the articles may restrict or prohibit the transfer of shares (Vinkulierung). Verify whether the agreement imposes additional restrictions beyond the articles.

- **Consent requirements (Vinkulierung):** Determine who must approve a transfer -- all shareholders, a qualified majority, or the managing directors. Check the approval timeline: if no response period is specified, the consent requirement can become a de facto transfer prohibition.
- **Rights of first refusal (Vorkaufsrechte):** Verify the trigger conditions (any proposed transfer, or only transfers to third parties outside the existing shareholders), the exercise period (30-60 days is standard), and whether the right is structured as a right of first refusal (matching a third-party offer) or a right of first offer (requiring the selling shareholder to offer shares to co-shareholders before seeking external buyers).
- **Valuation methodology:** Common approaches include discounted cash flow (Ertragswertverfahren), multiples-based valuation, asset-based valuation (Substanzwertverfahren), or determination by a neutral auditor (Schiedsgutachten, § 317 BGB). Where the agreement specifies a formula (e.g., "book value"), check whether this may produce results significantly below fair market value, which could be challenged as unconscionable (§ 138 BGB).
- **Indirect transfers and change of control:** Check whether the restrictions capture changes of control at the shareholder level (e.g., a shareholder that is itself a holding company being acquired). If not, the restrictions can be easily circumvented by selling the holding entity rather than the GmbH shares directly. Transfers within family groups or affiliated entities (§ 15 AktG by analogy) should be addressed separately.
- **Lock-up periods:** Some agreements prohibit any transfer during an initial period (typically 2-5 years). Check whether these are proportionate and whether exceptions exist for hardship cases (e.g., death, insolvency).

**Flag as risk:**
- No pre-emption right, allowing shares to pass to third parties without existing shareholder approval
- Valuation mechanism missing, ambiguous, or unilaterally determined by one party
- Indirect transfers not covered, enabling circumvention of transfer restrictions
- Lock-up period without any exception for death or insolvency of a shareholder
- Consent process without a defined response period, creating a de facto transfer prohibition

### Step 3: Drag-Along and Tag-Along Provisions

Drag-along clauses compel minority shareholders to sell alongside the majority; tag-along clauses protect minorities by allowing them to join a sale on the same terms.

- **Drag-along trigger thresholds:** Typically 75-80% for drag-along -- verify the exact percentage. Consider whether the threshold relates to shares held by a single shareholder or by a group acting in concert.
- **Price determination mechanism:** Confirm the methodology ensures fair market value. Drag-along at a price below fair market value is vulnerable to challenge under **§ 138 BGB** (unconscionability). Best practice: an independent valuation (by an auditor or investment bank) or matching the third-party offer price.
- **Tag-along terms:** Check whether tag-along rights include identical economic and legal terms (same price per share, same representations and warranties, same escrow arrangements). Partial tag-along rights (where the minority can only tag a proportional part of its shares) are less protective.
- **Notice and exercise periods:** The selling majority must provide adequate notice (typically 30-60 days) before exercising drag-along rights. The minority must have sufficient time to evaluate the terms and, if necessary, obtain independent advice.
- **BGH case law compliance:** The BGH has held that drag-along provisions must not unfairly disadvantage minority shareholders (BGH, II ZR 329/04). Clauses that allow forced sale at below fair market value or without adequate notice may be void under § 138 BGB or reviewed under the principles of shareholder fiduciary duties (gesellschafterliche Treuepflicht).

**Flag as risk:**
- Drag-along allows sale at a price below fair market value without independent valuation
- No tag-along right for minority shareholders
- Drag-along exercisable without adequate notice period (less than 30 days)
- No obligation to provide the minority with the same economic terms as the majority
- Drag-along triggered by a single majority shareholder acting alone without safeguards

### Step 4: Non-Compete and Non-Solicitation Clauses

German courts require non-compete clauses to be limited in scope, geography, and duration. Excessive restrictions are void or may be judicially reduced.

- **Scope distinction:** Verify whether the clause distinguishes between active shareholders/managing directors and passive investors. Passive financial investors should generally not be subject to non-compete obligations, as they have no access to trade secrets or operational knowledge.
- **Fiduciary non-compete duties:** Under **§ 112 HGB** (applied by analogy to GmbH managing directors), managing directors owe an implicit non-compete obligation during their tenure. This ends when they leave office unless the shareholder agreement provides otherwise.
- **Post-exit non-compete:** Duration should not exceed two years after departure (or, at most, three years in exceptional cases with significant consideration). Geographic scope must be proportionate to the company's actual market -- a worldwide prohibition requires justification by worldwide operations.
- **Non-compete compensation (Karenzentschadigung):** Where a shareholder is also employed (common in founder structures), a post-contractual non-compete requires compensation of at least 50% of the most recent remuneration (§ 74 Abs. 2 HGB by analogy). Even for non-employed shareholders, a non-compete without any consideration may be challenged as disproportionate.
- **Non-solicitation:** Separate from non-compete, these clauses prohibit poaching employees or customers. They are generally enforceable if limited to active solicitation (not passive acceptance) and reasonable in duration (12-24 months).

**Flag as risk:**
- Non-compete exceeding two years post-exit without objective justification
- No distinction between active and passive shareholders
- Missing Karenzentschadigung where the shareholder is also employed
- Geographic scope broader than the company's actual market
- Non-compete so broad that it effectively prevents the departing shareholder from earning a livelihood in their professional field

### Step 5: Deadlock Resolution Mechanisms

When shareholders with equal or blocking stakes disagree on fundamental matters, the company can become paralysed. Effective deadlock resolution is critical.

- **Deadlock definition:** Confirm the definition is precise and covers the relevant decision-making levels (shareholder meetings and, where applicable, management board). A typical definition requires two consecutive meetings at which the same matter fails to achieve the required majority.
- **Escalation procedures:** Common first-step mechanisms include escalation from management to shareholder level, mediation by an agreed neutral third party, or binding expert determination (Schiedsgutachten) for valuation or technical disputes.
- **Forced sale mechanisms:** If escalation fails, the agreement may provide for a Russian roulette (shoot-out) clause, where one party names a price and the other must either buy at that price or sell at that price. A Texas shoot-out is a sealed-bid variant. Both mechanisms carry risk for the financially weaker party.
- **Fairness safeguards:** German courts may consider a shoot-out clause unconscionable (§ 138 BGB) if it lacks a minimum price floor or if one party is significantly weaker financially, effectively allowing the other to force a sale at an unfair price.
- **Resolution timeline:** Verify that the escalation steps include reasonable deadlines (e.g., 30 days for mediation attempt, 90 days for arbitration). Open-ended deadlock resolution without firm timelines defeats the purpose.
- **Dissolution as last resort:** Absent a contractual mechanism, the only recourse is dissolution for cause (Auflosung aus wichtigem Grund, § 61 GmbHG) or exclusion of a shareholder through judicial proceedings (Ausschliessungsklage). Both are slow, expensive, and unpredictable.

**Flag as risk:**
- No deadlock mechanism at all, leaving parties reliant on dissolution for cause or judicial exclusion
- Shoot-out clause without minimum price floor or fairness safeguard for the financially weaker party
- Deadlock definition so narrow that genuine deadlocks are not captured
- No deadlines in the escalation procedure, allowing indefinite paralysis
- Mediation or arbitration clause without a specified institution or set of rules

### Step 6: Profit Distribution and Information Rights

Verify whether the agreement departs from the statutory pro-rata distribution rule (§ 29 GmbHG) and whether minority shareholders retain adequate visibility into the company's affairs.

- **Preferential returns:** Check for preferential returns (e.g., investor receives a fixed return before profits are distributed pro rata), cumulative dividend rights (unpaid preferential returns carry forward), or participating preferential rights (investor receives preference plus a pro-rata share of the remainder).
- **Reinvestment obligations and reserves:** Some agreements require a minimum percentage of profits to be retained or invested. Verify that these obligations do not systematically starve minority shareholders of distributions over extended periods.
- **Distributions in kind:** Check whether the agreement addresses non-cash distributions and how they are valued.
- **Information rights (§ 51a GmbHG):** The statutory right to information is mandatory and cannot be waived. Verify that any contractual information provisions supplement (not replace) the statutory minimum. Best practice: quarterly financial reports, annual audited accounts, prompt notification of material events.
- **Expanded information rights for investors:** Investor shareholders typically negotiate board observer rights, access to monthly management reports, and the right to appoint an auditor at the company's expense. Verify these do not conflict with confidentiality obligations or data protection requirements.
- **Anti-dilution provisions:** For venture capital and growth equity structures, check for anti-dilution protections (weighted average or full ratchet) that adjust the investor's shareholding in the event of a down-round.

**Flag as risk:**
- Information rights restricted below the statutory minimum of § 51a GmbHG
- Profit distribution mechanism that systematically disadvantages minority shareholders without a business justification
- No provisions for resolving disputes about the amount or timing of distributions
- Anti-dilution provisions that are so aggressive (full ratchet) that founders are effectively wiped out in a down-round
- Reinvestment obligation without any time limit or review mechanism


## Risk Assessment

### Red Flags: Majority Shareholder's Perspective

| Red Flag | Risk | Recommended Action |
|---|---|---|
| No drag-along clause | Cannot compel minority to participate in exit | Include a drag-along with fair market value and minimum notice period |
| Reserved matters list too broad | Minority veto on routine business decisions | Narrow the catalogue and use tiered thresholds |
| No non-compete for departing shareholders | Former shareholder competes immediately | Include a proportionate non-compete with Karenzentschadigung |
| Weak deadlock mechanism | Paralysis without resolution | Implement a multi-step escalation ending in a shoot-out or arbitration |
| No good-leaver/bad-leaver distinction | Same exit terms regardless of circumstances | Differentiate exit pricing based on reason for departure |

### Red Flags: Minority Shareholder's Perspective

| Red Flag | Risk | Recommended Action |
|---|---|---|
| No tag-along right | Majority sells to a third party; minority is left with a new, unchosen co-shareholder | Include a tag-along at identical economic terms |
| Valuation at book value | Significantly undervalues the shares, forcing a sale below fair value | Insist on fair market value with independent valuation |
| Information rights below statutory minimum | No visibility into the company's financial position | Supplement with quarterly reporting and auditor access |
| No pre-emption right | Shares can pass to competitors or hostile parties | Include a right of first refusal with a 30-60 day exercise period |
| Non-compete without compensation | Departing minority cannot work in their industry | Negotiate Karenzentschadigung or limit the scope |
| Shoot-out without price floor | Financially stronger party can force sale at low price | Include a minimum valuation floor or require independent appraisal |


## Special Scenarios

### Venture Capital and Startup Structures

Venture capital shareholder agreements (often called investor agreements or ISHA -- Investment and Shareholders' Agreement) have additional features:

- **Liquidation preferences:** Investor receives a multiple of its investment (1x-2x) before any distribution to founders. Check whether the preference is participating (investor also shares in remaining proceeds) or non-participating (investor chooses between preference and pro-rata share).
- **Anti-dilution protection:** Full ratchet (most protective for investors) or weighted average (more balanced). Full ratchet can devastate founders in a down-round.
- **Board composition and observer rights:** Investors typically negotiate for board seats proportional to their investment. Check voting mechanics at the board level.
- **Founder vesting and good-leaver/bad-leaver provisions:** Departing founders' shares may be subject to reverse vesting. A "bad leaver" (termination for cause, competition) typically receives book value or nominal value; a "good leaver" (death, disability, constructive dismissal) receives fair market value. The distinction must be precisely defined.
- **ESOP pool:** Employee stock option pool reserved for incentive compensation. Check whether the pool dilutes founders, investors, or both, and the size of the pool (typically 5-15%).
- **Conversion and IPO provisions:** Check for automatic conversion of preferred shares upon IPO and any registration rights or lock-up periods.

### 50/50 Joint Ventures

Equal joint ventures present unique deadlock risks:

- **Alternating chairmanship:** If board decisions require a majority, an alternating chairman with a casting vote can break ties -- but this creates asymmetry.
- **Specific deadlock triggers:** Define precisely which decisions constitute a deadlock. Operational decisions should be resolved at management level; strategic decisions escalate to the joint venture partners.
- **Put/call options:** A common exit mechanism where, upon unresolvable deadlock, one partner can put its shares to the other (at fair market value) or call the other's shares. The first mover may have a strategic advantage.
- **Non-compete scope:** In joint ventures between competitors, the non-compete clause must be carefully drawn to comply with competition law (Art. 101 TFEU, § 1 GWB).

### Family-Owned GmbH Structures

Family shareholder agreements address generational succession:

- **Transfer restrictions within the family:** Shares may only be transferred to direct descendants, with a right of first refusal for other family branches.
- **Compulsory offer on divorce:** To prevent shares from passing to a non-family spouse through matrimonial property division, the agreement should require a compulsory offer to the remaining family shareholders.
- **Governance during incapacity:** Powers of attorney and substitute voting arrangements for shareholders who become incapacitated.
- **Succession planning:** Integration with testamentary dispositions and lifetime gift arrangements. Ensure the shareholder agreement and the will do not conflict.


## Limitations of This Skill

This skill provides a structured initial analysis. In the following cases, engaging a lawyer is necessary:

- **Drafting and negotiation** of complex shareholder agreements, particularly for venture capital, private equity, or joint venture structures
- **Corporate restructuring** involving share transfers, capital measures, or conversions between legal forms
- **Tax implications** of profit distributions, transfer pricing, and exit proceeds (§§ 17, 20 EStG; § 8b KStG)
- **Competition law review** of non-compete clauses and joint venture arrangements (Art. 101 TFEU, § 1 GWB)
- **Disputes** between shareholders, including exclusion proceedings (Ausschliessungsklage) and dissolution for cause
- **Cross-border structures** involving shareholders or assets in multiple jurisdictions

Compound is happy to assist with the review, negotiation, and drafting of shareholder agreements that meet the requirements of German corporate law.
