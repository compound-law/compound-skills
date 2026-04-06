# Compound Skills

Turn any AI agent into a German law assistant. 12 skills covering contracts, compliance, GDPR, and corporate formation — in German and English.

## Install

All skills:

```bash
npx skills add compound-law/compound-skills
```

Single skill:

```bash
npx skills add compound-law/compound-skills --skill agb-check
```

## Skills

| German | English | Description |
|--------|---------|-------------|
| `agb-check` | `terms-check` | Reviews general terms and conditions for validity under German AGB law (§§ 305-310 BGB) |
| `ki-verordnung-compliance` | `ai-act-compliance` | EU AI Act compliance assessment — risk classification, documentation, and conformity |
| `arbeitszeugnis` | `employment-reference` | Analyzes German employment references and decodes the coded reference language |
| `gewerbemietvertrag` | `commercial-lease` | Review checklist for commercial lease agreements under German law |
| `hinweisgebersystem` | `compliance-whistleblower` | Whistleblower protection system implementation under HinSchG and EU Directive 2019/1937 |
| `auftragsverarbeitung` | `data-processing-agreement` | GDPR-compliant data processing agreement review — Art. 28, sub-processors, cross-border transfers |
| `dsgvo-auskunft` | `gdpr-data-request` | Handling data access requests under Art. 15 GDPR — deadlines, disclosures, and process steps |
| `kuendigungspruefung` | `employment-termination` | Employment termination review — notice periods, dismissal protection, and severance |
| `gmbh-gruendung` | `gmbh-formation` | Step-by-step GmbH formation — articles of association, notarization, and commercial register |
| `nda-pruefung` | `nda-review` | NDA analysis under German law — identifies risks, missing clauses, and non-standard terms |
| `saas-vertragspruefung` | `saas-agreement` | SaaS agreement review — SLA commitments, data ownership, liability caps, and exit provisions |
| `gesellschaftervereinbarung` | `shareholder-agreement` | Shareholder agreement review — voting rights, transfer restrictions, and exit provisions |
