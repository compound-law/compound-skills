---
name: employment-contract-review
description: 'Review framework for employment contracts under German law. Covers probation, notice periods, non-compete clauses, vacation entitlement, and overtime provisions under BGB, KSchG, and BUrlG.'
---


## Overview

Claude can review German employment contracts — checking probation periods, termination notice, restrictive covenants, and vacation entitlement under German law (BGB, KSchG, BUrlG). This skill provides a structured framework for employees reviewing a contract before signing, and for employers verifying that their standard templates comply with mandatory German statutory requirements.

German employment law sets a dense floor of mandatory protections that contractual clauses cannot undercut. Many standard-form contracts — particularly those drafted for other EU jurisdictions or for multinational groups — contain provisions that are invalid under German law even if signed by both parties. Identifying these clauses before signing prevents disputes and, for employers, exposure to claims that cannot be waived.

For issues identified during the review, consider using the [Employment Termination Review](/en-DE/skills/employment-termination/) skill if an existing contract is already being terminated, or the [Employment Reference Analysis](/en-DE/skills/employment-reference/) skill for questions about end-of-employment documentation.


## What Claude Checks in a German Employment Contract

### Probation Period (Probezeit, § 622 Abs. 3 BGB)

The statutory maximum probationary period is six months. During this time, either party may terminate with two weeks' notice to any calendar day. Contracts that extend the probation beyond six months or impose longer notice periods during probation are partially void — the probation is treated as ending at six months and the full statutory notice periods apply thereafter.

**Flag as risk:**
- Probation period stated as longer than six months
- Notice period during probation stated as longer than two weeks
- Contract silent on probation but written for a role where a collective bargaining agreement (Tarifvertrag) limits probation to a shorter period

### Notice Periods (Kündigungsfristen, § 622 BGB)

German law sets graduated minimum notice periods for employer-initiated terminations that increase with tenure. The base period is four weeks to the 15th or end of a calendar month. At two years' service: one month to month-end; at five years: two months; at eight years: three months; up to seven months at twenty years.

Contractual notice periods may be longer than the statutory minimum but not shorter — except during probation. If the contract sets equal notice periods for employee- and employer-initiated terminations, the employee's period may not exceed the employer's statutory minimum (§ 622 Abs. 6 BGB). A clause requiring the employee to give longer notice than the employer is void for that excess.

**Flag as risk:**
- Notice period shorter than the § 622 BGB statutory minimum for the employee's likely tenure at termination
- Employee's contractual notice period longer than the employer's notice period (void under § 622 Abs. 6 BGB)
- Notice to a fixed calendar date rather than to the 15th or end of the month (void unless the longer period is also met)
- Collective bargaining agreement (Tarifvertrag) referenced — CBA may set different periods, must verify

### Non-Compete and Post-Contractual Restrictions (Nachvertragliches Wettbewerbsverbot, §§ 74–75d HGB)

A post-contractual non-compete clause is only enforceable in Germany if: (1) it is in writing signed by the employer, (2) it does not exceed two years, (3) it covers activities competitive to the employer's actual business, and (4) the employer commits in writing to pay at least 50% of the employee's last contractual compensation for the full duration (Karenzentschädigung).

A non-compete clause that lacks the compensation commitment or exceeds two years is not automatically void — the employee may choose to comply and claim the compensation, or may choose to treat it as non-binding and compete freely. However, without the written compensation commitment, the employer cannot enforce compliance.

**Flag as risk:**
- Non-compete clause without written compensation commitment (Karenzentschädigung) of at least 50% of last remuneration
- Duration exceeds two years
- Geographic or subject-matter scope broader than the employer's actual business area
- Clause states compensation "may be offset against new employment income" in ways that reduce it below the 50% floor
- Garden leave clause purporting to serve as the compensation — this requires careful analysis

### Annual Leave (Urlaubsanspruch, BUrlG)

The Bundesurlaubsgesetz (BUrlG) mandates a minimum of 20 working days of paid annual leave for employees working a five-day week (24 days for a six-day week). This floor cannot be contracted away. Contracts may grant more leave; if collective bargaining agreements apply, they typically provide 25–30 days.

**Flag as risk:**
- Annual leave stated below the BUrlG statutory minimum for the employee's working days per week
- Clause purporting to allow forfeiture of unused leave without carry-over rights (BAG has restricted this; carry-over is required if the employee could not take leave for reasons they did not cause)
- Leave entitlement conditional on full-year employment without a pro-rata provision for partial years (§ 5 BUrlG provides for pro-rata entitlement after six months)

### Overtime and Working Hours (Überstunden, ArbZG)

The Arbeitszeitgesetz (ArbZG) caps working time at 8 hours per working day, extendable to 10 hours if the average over six calendar months does not exceed 8 hours per day. Sunday and public holiday work is restricted. Overtime clauses that purport to allow unlimited overtime "covered by salary" or that set flat-rate compensation far below realistic overtime are routinely challenged.

**Flag as risk:**
- Clause stating all overtime is covered by the base salary without limit — this is void beyond a reasonable upper limit (German courts typically allow 10–20% of monthly working hours)
- No upper cap on required overtime (employer cannot contractually obligate unlimited extra hours)
- ArbZG Sunday/holiday restrictions not addressed where the role may require weekend work (sector-specific exemptions apply but must be verified)

### Governing Law and Jurisdiction (Gerichtsstand, Internationales Privatrecht)

If the contract is for a role performed in Germany, German mandatory employment law applies regardless of the governing law clause (Rome I Regulation, Art. 8). A contract stating "English law governs" does not avoid BGB, KSchG, or BUrlG protections for a German-based employee. For expat and internationally mobile employees, the applicable mandatory law requires careful analysis — German mandatory protections apply to work habitually performed in Germany.

**Flag as risk:**
- Foreign governing law clause without assessment of German mandatory law override
- Exclusive foreign jurisdiction clause for labor disputes (German labor courts have exclusive jurisdiction for many claims arising out of German employment — clause may not be enforceable)
- International mobility clause that could shift the habitual place of work and affect the applicable mandatory law


## What to Paste Into Claude

For an effective review, share the full employment contract text and tell Claude:

1. **The role and employment start date** — this determines probationary period timing and relevant collective bargaining agreements
2. **Whether a CBA applies** — if the offer letter or contract references a Tarifvertrag, name it; CBA terms override many statutory defaults and require separate analysis
3. **The proposed compensation structure** — needed to assess whether any non-compete clause meets the 50% Karenzentschädigung threshold
4. **Any specific clauses you want prioritized** — probation, notice, non-compete, bonus, or data protection clauses

A useful starting prompt: *"Review this German employment contract. I start on [date] as [role] at a company with [X] employees. No CBA applies. Flag any clauses that conflict with BGB, KSchG, BUrlG, or ArbZG, and identify any that favor the employer beyond what German law permits."*

For data privacy considerations when sharing contract text with Claude, see [Claude for Teams: GDPR](/en-DE/tools/claude-team-gdpr/).


## Limitations of This Skill

This skill identifies clause-level risks and statutory compliance issues. The following require a lawyer:

- **Negotiation strategy** — advising which clauses to push back on given the employer and sector is a legal judgment, not a checklist
- **Collective bargaining agreement analysis** — if a CBA applies, the full text of the applicable agreement must be analyzed against the contract
- **Discrimination and AGG compliance** — reviewing whether hiring criteria or compensation structures violate the Allgemeines Gleichbehandlungsgesetz requires a tailored assessment
- **Executive (leitender Angestellter) contracts** — managing directors (GmbH-Geschäftsführer) and senior executives have different rights; KSchG does not apply to GmbH-Geschäftsführer at all
- **Equity and phantom stock clauses** — vesting schedules, leaver provisions, and good/bad leaver definitions require detailed legal review
- **Cross-border and posted-worker arrangements** — where an employee will work across multiple EU jurisdictions, mandatory law analysis becomes complex

Compound is happy to assist with the legal review, negotiation preparation, and compliance assessment of employment contracts under German law.


## Frequently Asked Questions

### Can AI review my employment contract in Germany?

Yes. AI can identify clauses that conflict with German statutory minimums — checking probation length, notice periods, non-compete requirements, and annual leave against BGB, KSchG, BUrlG, and ArbZG. What AI cannot do is replace legal advice on whether to accept, negotiate, or reject specific clauses given your personal situation, leverage, and the employer's sector.

### Is Claude GDPR-compliant for employment contracts?

Claude for Teams and Claude for Enterprise process data under Anthropic's Data Processing Agreement and do not use business conversation data to train models. Employment contracts typically contain personal data (salary, address, tax details), so the appropriate product tier and configuration matters — see [Claude for Teams: GDPR](/en-DE/tools/claude-team-gdpr/) for the technical compliance details.

### What clauses should I check in a German employment contract?

The most consequential clauses to review before signing a German employment contract are: the probation period and notice periods during and after probation, the post-contractual non-compete clause and whether it includes the mandatory Karenzentschädigung, the annual leave entitlement against the BUrlG minimum, overtime provisions and whether "flat-rate coverage" is capped, and the governing law and jurisdiction clause if you are an expat or internationally mobile.
