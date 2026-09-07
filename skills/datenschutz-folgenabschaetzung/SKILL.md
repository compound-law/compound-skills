---
name: datenschutz-folgenabschaetzung
description: 'DSFA/DPIA: Wann die Folgenabschätzung nach Art. 35 DSGVO Pflicht ist, wie sie durchgeführt und dokumentiert wird — mit Prüfrahmen für Deutschland.'
---


Eine **Datenschutz-Folgenabschätzung** (DSFA, englisch: *Data Protection Impact Assessment*, DPIA) ist eine Pflichtprüfung nach **Art. 35 DSGVO**, wenn eine Verarbeitung personenbezogener Daten voraussichtlich ein hohes Risiko für die Rechte und Freiheiten natürlicher Personen birgt. Die DSFA muss **vor Beginn der Verarbeitung** abgeschlossen sein — nicht erst im Nachhinein. Das Fehlen einer erforderlichen DSFA stellt einen eigenständigen DSGVO-Verstoß dar, der mit Bußgeldern bis zu **10 Mio. EUR oder 2 % des weltweiten Jahresumsatzes** geahndet werden kann (Art. 83 Abs. 4 lit. a DSGVO).

Dieser Skill leitet die systematische Durchführung und Dokumentation einer DSFA an. Er gilt sowohl für neue Verarbeitungsvorgänge als auch für wesentliche Änderungen bestehender Systeme — insbesondere bei KI-gestützten Prozessen, biometrischen Daten, Videoüberwachung, Profiling und Beschäftigtendaten. Für KI-Systeme, die als Hochrisiko-Systeme nach dem **AI Act** eingestuft werden, ist die DSFA nach Art. 35 DSGVO neben der Grundrechtsfolgenbewertung (FRIA) nach **Art. 27 AI Act** gesondert durchzuführen (→ [KI-Verordnung Compliance-Check](/de-DE/skills/ki-verordnung-compliance/)).


## Überblick

Dieser Skill bietet einen strukturierten Prüfrahmen für die Datenschutz-Folgenabschätzung nach Art. 35 DSGVO. Wesentliche Vorschriften sind **Art. 35** (Pflicht zur DSFA), **Art. 36** (Vorabkonsultation bei hohem Restrisiko), **Art. 5** (Datenschutzgrundsätze: Zweckbindung, Datenminimierung, Speicherbegrenzung), **Art. 25** (Datenschutz durch Technikgestaltung und datenschutzfreundliche Voreinstellungen) sowie **§ 67 BDSG** für besondere Verarbeitungssituationen im deutschen öffentlichen Sektor. Der betriebliche oder behördliche Datenschutzbeauftragte muss nach Art. 35 Abs. 2 DSGVO in jedem Fall konsultiert werden, sofern ein solcher bestellt ist.

Die DSFA ist kein einmaliges Dokument, sondern ein **lebender Prozess**: Wesentliche Änderungen an der Verarbeitung oder ihrem Kontext erfordern eine Aktualisierung. Aufsichtsbehörden wie der Bundesbeauftragte für den Datenschutz und die Informationsfreiheit (BfDI) oder die Landesdatenschutzbeauftragten (LfDI) können die DSFA-Dokumentation jederzeit anfordern.


## Systematische Prüfung

### Schritt 1: Ist eine DSFA erforderlich?

Der erste Schritt ist die Pflichtprüfung: Löst die geplante Verarbeitung die DSFA-Pflicht nach Art. 35 DSGVO aus?

- **Regelbeispiele des Art. 35 Abs. 3 DSGVO:** Eine DSFA ist in jedem Fall erforderlich bei: (a) systematischer und umfassender Bewertung persönlicher Aspekte einschließlich Profiling mit rechtlicher oder ähnlich erheblicher Wirkung, (b) umfangreicher Verarbeitung besonderer Datenkategorien nach Art. 9 DSGVO (Gesundheit, Biometrie, Ethnie, Religion, politische Meinungen) oder von Daten über strafrechtliche Verurteilungen (Art. 10 DSGVO) und (c) systematischer Beobachtung öffentlich zugänglicher Bereiche in großem Umfang.
- **DSK-Muss-Liste:** Die Datenschutzkonferenz (DSK) hat eine Positivliste veröffentlicht, die Verarbeitungsarten benennt, die in Deutschland stets eine DSFA erfordern. Dazu gehören: Videoüberwachung mit biometrischer Identifizierung, Scoring-Verfahren für Kreditwürdigkeit oder Versicherungsrisiken, Tracking von Mitarbeiterverhalten (insbesondere per App oder Wearable), genetische oder biometrische Datenverarbeitung in großem Umfang sowie zentrale Verarbeitung von Gesundheitsdaten.
- **Drei-Kriterien-Test (WP 248, Art.-29-Datenschutzgruppe):** Liegen **zwei oder mehr** der folgenden Kriterien vor, ist eine DSFA stark indiziert: Scoring oder Profiling, automatisierte Entscheidungsfindung mit erheblicher Wirkung, systematische Überwachung, sensible Datenkategorien, umfangreiche Verarbeitung, Zusammenführung oder Abgleich von Datensätzen, vulnerable Personengruppen (Minderjährige, Beschäftigte, Patienten), innovative Technologie, Datenübermittlung in Drittländer mit erschwertem Rechtsschutz.
- **Wesentliche Änderungen:** Änderungen an bestehenden Verarbeitungsvorgängen, die deren Risikoniveau wesentlich erhöhen, lösen eine erneute DSFA-Pflicht aus — z. B. Wechsel zu einem neuen Cloud-Anbieter, Einführung eines KI-gestützten Analysesystems oder Erweiterung auf neue Datenkategorien.

**Risikokennzeichnung:**
- Drei-Kriterien-Test ergibt zwei oder mehr Treffer, aber DSFA abgelehnt
- Verarbeitung sensibler Datenkategorien in großem Umfang ohne DSFA-Prüfung
- Wesentliche Systemänderung ohne erneute DSFA-Bewertung
- Überwachungssystem am Arbeitsplatz ohne DSFA und ohne Betriebsratseinbindung nach § 87 Abs. 1 Nr. 6 BetrVG

### Schritt 2: Beschreibung des Verarbeitungsvorgangs (Art. 35 Abs. 7 lit. a DSGVO)

Die DSFA beginnt mit einer systematischen Beschreibung des Verarbeitungsvorgangs. Ohne präzise Beschreibung kann das Risiko nicht bewertet werden.

- **Zwecke und Rechtsgrundlagen:** Definieren Sie alle Verarbeitungszwecke und ordnen Sie jedem Zweck eine Rechtsgrundlage nach Art. 6 DSGVO zu. Bei besonderen Datenkategorien sind die Ausnahmetatbestände des Art. 9 Abs. 2 DSGVO sowie ggf. §§ 22, 26 BDSG zu benennen.
- **Datenflussdiagramm:** Dokumentieren Sie alle Datenflüsse: Erhebungsquellen, interne Weiterleitung, externe Empfänger (einschließlich Auftragsverarbeiter und gemeinsam Verantwortliche), Drittlandtransfers und Löschpfade.
- **Datenkategorien und Betroffenengruppen:** Listen Sie alle verarbeiteten Datenkategorien — mit besonderer Kennzeichnung sensibler Kategorien — und alle Betroffenengruppen auf. Besondere Aufmerksamkeit gilt vulnerablen Gruppen: Minderjährige, Beschäftigte (strukturelles Machtgefälle), Patienten, Straftatverdächtige.
- **Empfänger und Auftragsverarbeiter:** Jeder externe Empfänger ist zu benennen. Für Auftragsverarbeiter muss ein konformer **[Auftragsverarbeitungsvertrag (AVV) nach Art. 28 DSGVO](/de-DE/skills/auftragsverarbeitung/)** bestehen; bei Drittlandtransfers sind die Übermittlungsmechanismen (SCCs, Angemessenheitsbeschluss) zu dokumentieren.
- **Aufbewahrungsfristen:** Definieren Sie konkrete Lösch- oder Sperrfristen für jede Datenkategorie und die jeweils maßgebliche Grundlage (gesetzliche Aufbewahrungspflicht, legitimes Geschäftsinteresse, Einwilligung).

**Risikokennzeichnung:**
- Verarbeitungszwecke vage oder nicht vollständig dokumentiert
- Kein Datenflussdiagramm, Drittzugriffe nicht identifiziert
- Auftragsverarbeiter ohne konformen AVV eingebunden
- Löschfristen nicht definiert oder unrealistisch lang

### Schritt 3: Notwendigkeit und Verhältnismäßigkeit (Art. 35 Abs. 7 lit. b DSGVO)

Prüfen Sie, ob die Verarbeitung auf das notwendige Maß beschränkt ist (Datenminimierung nach Art. 5 Abs. 1 lit. c DSGVO) und ob die gewählten Mittel verhältnismäßig zu den angestrebten Zwecken sind.

- **Datensparsamkeit:** Werden nur die Daten verarbeitet, die für den jeweiligen Zweck tatsächlich erforderlich sind? Häufige Fehler: überbordende Nutzungsprofile, Echtzeitlokalisierung ohne operativen Bedarf, Langzeitspeicherung für hypothetische künftige Anfragen.
- **Zweckbindung (Art. 5 Abs. 1 lit. b DSGVO):** Prüfen Sie, ob eine beabsichtigte Weiterverarbeitung mit dem ursprünglichen Erhebungszweck vereinbar ist (Art. 6 Abs. 4 DSGVO: Kriterien Zusammenhang, Art der Daten, Folgen, Garantien). Unvereinbare Weiterverarbeitung erfordert eine neue eigenständige Rechtsgrundlage.
- **Alternative Mittel:** Wurden weniger einschneidende Alternativen erwogen? Pseudonymisierung statt Klardaten, aggregierte Analysen statt Einzeldaten, Opt-in statt Opt-out. Dokumentieren Sie, warum die gewählte Methode Alternativen vorzuziehen ist.
- **Verhältnismäßigkeit im Beschäftigungskontext:** Bei Beschäftigtendaten ist die Verhältnismäßigkeit besonders streng zu prüfen (§ 26 BDSG). Überwachungsmaßnahmen müssen erforderlich, angemessen und für die Beschäftigten zumutbar sein.

**Risikokennzeichnung:**
- Mehr Daten erhoben als für den Zweck erforderlich, ohne dokumentierte Begründung
- Weiterverarbeitung zu neuen Zwecken ohne Vereinbarkeitstest nach Art. 6 Abs. 4 DSGVO
- Keine Prüfung weniger einschneidender Alternativen dokumentiert
- Beschäftigtendaten ohne Abwägung der Verhältnismäßigkeit nach § 26 BDSG

### Schritt 4: Risikoidentifikation und -bewertung (Art. 35 Abs. 7 lit. c DSGVO)

Der Kern der DSFA ist die strukturierte Risikoanalyse. Risiken sind aus der **Perspektive der betroffenen Personen** zu bewerten, nicht aus Unternehmensperspektive.

- **Risikoszenarien:** Identifizieren Sie konkrete Szenarien, in denen die Verarbeitung zu erheblichen Risiken für die Betroffenen führen kann:
  - **Unrechtmäßiger Zugriff:** Datenpanne, Hacking, Insidermissbrauch
  - **Unbeabsichtigte Veränderung:** Datenverlust, Datenverfälschung
  - **Unzulässige Verarbeitung:** Zweckentfremdung, Diskriminierung durch Algorithmen, Profiling-Missbrauch
  - **Identitätsdiebstahl / Rufschädigung:** Exponierung sensibler Merkmale oder biometrischer Daten
  - **Entscheidungsfolgen:** Benachteiligung bei Kredit, Einstellung oder Versicherung durch fehlerhafte automatisierte Entscheidungen
- **Risikoeinschätzung:** Bewerten Sie jedes Szenario nach **Eintrittswahrscheinlichkeit** (hoch/mittel/niedrig) und **Schwere der Folgen** (hoch/mittel/niedrig). Szenarien mit hoher Wahrscheinlichkeit und/oder hoher Schwere sind vorrangig zu behandeln.
- **Bestehende Maßnahmen berücksichtigen:** Beziehen Sie bereits vorhandene technische und organisatorische Maßnahmen (TOMs) in die Bewertung ein — das **Restrisiko** nach Anwendung der TOMs ist maßgeblich.
- **Spezifika von KI-Systemen:** Für KI-gestützte Verarbeitung sind zusätzliche Risikofaktoren zu berücksichtigen: algorithmische Verzerrungen (Bias), fehlende Nachvollziehbarkeit von Entscheidungen (Explainability), schleichende Zweckausdehnung durch Modell-Updates sowie Risiken bei der Modellentstehung (Privacy by Design nach Art. 25 DSGVO).

**Risikokennzeichnung:**
- Risikobewertung aus Unternehmensperspektive statt Betroffenenperspektive
- Nur abstrakte Risiken ohne konkrete Szenarien mit Wahrscheinlichkeit und Schwere
- Keine Berücksichtigung von Verzerrungsrisiken bei KI-gestützten Entscheidungen
- Risikoanalyse ignoriert bekannte Schwachstellen oder vergangene Sicherheitsvorfälle

### Schritt 5: Maßnahmen zur Risikobehandlung (Art. 35 Abs. 7 lit. d DSGVO)

Für jedes identifizierte Risiko sind geeignete Maßnahmen zur Risikominderung zu dokumentieren.

- **Technische Maßnahmen:** Verschlüsselung im Ruhezustand (AES-256) und bei der Übertragung (TLS 1.2+), Pseudonymisierung, rollenbasierte Zugangskontrollen (RBAC), Protokollierung und Auditierung, Penetrationstests, Datenmaskierung in Test- und Entwicklungsumgebungen, sichere Löschverfahren.
- **Organisatorische Maßnahmen:** Schulungen, Datenschutz-Richtlinien, Need-to-know-Prinzip, Incident-Response-Verfahren, Einbindung des Datenschutzbeauftragten, aktuelles Verzeichnis der Verarbeitungstätigkeiten nach Art. 30 DSGVO.
- **Vertragliche Maßnahmen:** Konformer AVV mit Auftragsverarbeitern, geeignete Drittlandtransfer-Mechanismen (SCCs, Angemessenheitsbeschluss), vertraglich vereinbarte Auditrechte gegenüber Dienstleistern.
- **Restrisiko:** Nach Anwendung aller Maßnahmen ist das verbleibende Restrisiko einzuschätzen. Verbleibt ein **hohes Restrisiko**, ist eine **Vorabkonsultation** der Aufsichtsbehörde nach Art. 36 DSGVO zwingend erforderlich. Die zuständige Behörde gibt binnen acht Wochen (verlängerbar auf sechs Monate) eine schriftliche Empfehlung ab.
- **Mitbestimmung des Betriebsrats:** Bei Beschäftigtendaten-Verarbeitungen, die Mitbestimmungsrechte nach § 87 Abs. 1 Nr. 6 BetrVG berühren, ist der Betriebsrat einzubeziehen. Eine Betriebsvereinbarung kann zugleich als Dokumentation der Verhältnismäßigkeit dienen.

**Risikokennzeichnung:**
- Maßnahmen beschreiben nur generelle TOMs ohne Bezug zu identifizierten konkreten Risiken
- Restrisikobewertung fehlt oder kommt ohne Begründung zum Ergebnis "niedriges Risiko"
- Vorabkonsultation nach Art. 36 DSGVO bei hohem Restrisiko unterblieben
- Betriebsrat bei mitbestimmungspflichtigen Überwachungsmaßnahmen nicht eingebunden


## Besondere Szenarien

### KI-Systeme und automatisierte Entscheidungen

KI-gestützte Verarbeitungsvorgänge erfüllen in aller Regel mindestens zwei Kriterien des Drei-Kriterien-Tests und lösen damit regelmäßig die DSFA-Pflicht aus. Besonders relevant:

- **Hochrisiko-KI-Systeme nach AI Act (Anhang III):** Die DSFA nach Art. 35 DSGVO und die FRIA nach Art. 27 AI Act sind **getrennte Instrumente** und müssen eigenständig durchgeführt werden. Eine gemeinsame Dokumentation ist zulässig, sofern alle jeweiligen Anforderungen vollständig erfüllt sind (→ [KI-Verordnung Compliance-Check](/de-DE/skills/ki-verordnung-compliance/)).
- **Automatisierte Einzelentscheidungen (Art. 22 DSGVO):** Entscheidungen, die ausschließlich auf automatisierter Verarbeitung beruhen und rechtliche oder ähnlich erhebliche Wirkung haben (z. B. Kreditablehnung, Versicherungstarif, Bewerbungsauswahl), sind nur unter engen Voraussetzungen zulässig und erfordern stets eine DSFA.
- **Profiling im Beschäftigtenverhältnis:** Leistungsbewertung, Verhaltensanalyse oder prädiktive Einstellungsentscheidungen auf KI-Basis lösen in Deutschland regelmäßig sowohl die DSFA-Pflicht als auch die Betriebsratsbeteiligung nach § 87 BetrVG aus. Beide Verfahren sind parallel zu führen.

### Videoüberwachung und biometrische Daten

- **Videoüberwachung mit biometrischer Identifizierung:** Stets DSFA-pflichtig nach DSK-Muss-Liste und Art. 35 Abs. 3 lit. b DSGVO.
- **Einfache Videoüberwachung** (ohne Biometrie): DSFA erforderlich, wenn sie systematisch öffentlich zugängliche Bereiche in großem Umfang überwacht (Art. 35 Abs. 3 lit. c DSGVO). Zusätzlich gilt § 4 BDSG mit Interessenabwägung und Hinweispflichten.
- **Gesundheitsdaten im Unternehmen:** Betriebliche Gesundheitsförderung, Krankmeldungsauswertungen oder biometrische Zugangssysteme erfordern stets eine DSFA in Verbindung mit einer Rechtsgrundlage nach Art. 9 Abs. 2 DSGVO und § 26 Abs. 3 BDSG.

### Datentransfers in Drittländer

Werden Daten aus einer Verarbeitung mit hohem Risiko in Drittländer ohne Angemessenheitsbeschluss übermittelt (insbesondere USA ohne DPF-Zertifizierung, China, Russland), sind in der DSFA das Transferrisiko und die angewandten Übermittlungsmechanismen (SCCs, Transfer Impact Assessment nach Schrems II) gesondert zu bewerten. Ein fehlerhaftes oder fehlendes TIA in Kombination mit einem Drittlandtransfer erhöht das Restrisiko erheblich.


## Wie läuft eine DSFA bei Compound ab?

Wenn Sie Compound mit der Durchführung oder Überprüfung einer Datenschutz-Folgenabschätzung beauftragen, folgt der Prozess einem strukturierten Ablauf:

1. **Erstgespräch:** Erfassung des Verarbeitungsvorgangs, vorläufige Einschätzung der DSFA-Pflicht und Abstimmung des Prüfungsumfangs.
2. **Datenfluss-Workshop:** Gemeinsame Erarbeitung des vollständigen Datenflussdiagramms mit Ihren Fach- und IT-Abteilungen.
3. **Risikoanalyse:** Systematische Identifikation und Bewertung der Risiken für Betroffene, einschließlich spezifischer Szenarien für Ihre konkrete Verarbeitungssituation.
4. **Maßnahmenplan:** Entwicklung eines priorisierten Maßnahmenplans zur Risikoreduzierung, abgestimmt auf Ihre technische und organisatorische Infrastruktur.
5. **DSFA-Dokument:** Erstellung des vollständigen DSFA-Dokuments mit Restrisiko-Einschätzung und Empfehlung zur Vorabkonsultation, falls erforderlich.
6. **Laufende Betreuung:** Jährliche Überprüfung und anlassbezogene Aktualisierung bei wesentlichen Änderungen der Verarbeitung oder des regulatorischen Rahmens.


## Grenzen dieses Skills

Dieser Skill bietet eine strukturierte Erstbewertung. In folgenden Fällen ist die Einschaltung eines Rechtsanwalts oder Datenschutzbeauftragten erforderlich:

- **Vorabkonsultation (Art. 36 DSGVO):** Wenn das Restrisiko nach Anwendung aller Maßnahmen hoch bleibt, ist die Konsultation der zuständigen Aufsichtsbehörde (LfDI des jeweiligen Bundeslandes oder BfDI) Pflicht. Compound begleitet diesen Prozess einschließlich der Aufbereitung der Konsultationsunterlagen.
- **KI-Hochrisiko-Systeme:** Das Zusammenspiel von DSFA (Art. 35 DSGVO), FRIA (Art. 27 AI Act) und technischer Dokumentationspflicht (Art. 11, Anhang IV AI Act) erfordert rechtliche Koordination beider Regelwerke.
- **Grenzüberschreitende Verarbeitungen:** Bei Datenflüssen in mehrere EU-Mitgliedstaaten kann der One-Stop-Shop-Mechanismus nach Art. 56 DSGVO einschlägig sein, mit der federführenden Aufsichtsbehörde des Hauptsitzes.
- **Strafverfolgungsdaten (§ 62 BDSG, Richtlinie (EU) 2016/680):** Für Polizei und Justiz gelten gesonderte Regelungen anstelle von Art. 35 DSGVO.
- **Streitige Betriebsratsbeteiligung:** Bei Konflikten über Mitbestimmungsrechte zu datenschutzrelevanten Überwachungs- oder Auswertungsmaßnahmen.

Compound unterstützt gerne bei der Durchführung, Dokumentation und Überprüfung von Datenschutz-Folgenabschätzungen — sowohl als Erstbewertung als auch als laufende Compliance-Begleitung.


## Häufig gestellte Fragen zur Datenschutz-Folgenabschätzung

### Wann ist eine Datenschutz-Folgenabschätzung nach DSGVO Pflicht?

Eine DSFA ist nach Art. 35 DSGVO Pflicht, wenn eine Verarbeitung voraussichtlich ein hohes Risiko für die Rechte und Freiheiten natürlicher Personen birgt. Dies gilt insbesondere bei umfangreicher Verarbeitung besonderer Datenkategorien (z. B. Gesundheits- oder Biometriedaten), bei systematischem Profiling mit erheblicher Wirkung sowie bei Videoüberwachung öffentlicher Bereiche in großem Umfang. Die DSK-Muss-Liste benennt für Deutschland spezifische Verarbeitungsarten, die stets eine DSFA auslösen.

### Was muss eine DSFA enthalten?

Eine DSFA muss nach Art. 35 Abs. 7 DSGVO mindestens enthalten: (1) eine systematische Beschreibung der geplanten Verarbeitung einschließlich Zweck und Rechtsgrundlagen, (2) eine Bewertung der Notwendigkeit und Verhältnismäßigkeit der Verarbeitung, (3) eine Bewertung der Risiken für die Rechte und Freiheiten der betroffenen Personen und (4) die geplanten Abhilfemaßnahmen einschließlich Garantien, Sicherheitsvorkehrungen und Verfahren zum Schutz personenbezogener Daten.

### Wer muss eine DSFA durchführen?

Die Pflicht trifft den **Verantwortlichen** nach Art. 4 Nr. 7 DSGVO, d. h. das Unternehmen oder die Behörde, die über Zwecke und Mittel der Verarbeitung bestimmt. Der **Datenschutzbeauftragte** (sofern vorhanden) muss nach Art. 35 Abs. 2 DSGVO konsultiert werden. Auftragsverarbeiter sind nicht zur DSFA verpflichtet, müssen aber nach Art. 28 Abs. 3 lit. f DSGVO bei der Durchführung unterstützen.

### Was passiert, wenn eine erforderliche DSFA nicht durchgeführt wird?

Das Unterlassen einer gesetzlich erforderlichen DSFA stellt einen eigenständigen DSGVO-Verstoß dar. Aufsichtsbehörden können gemäß Art. 83 Abs. 4 lit. a DSGVO Bußgelder von bis zu 10 Mio. EUR oder 2 % des weltweiten Jahresumsatzes verhängen. Zusätzlich kann die Aufsichtsbehörde die Verarbeitung vorübergehend oder dauerhaft untersagen (Art. 58 Abs. 2 lit. f DSGVO).

### Muss die DSFA bei Änderungen am Verarbeitungssystem wiederholt werden?

Ja. Eine DSFA ist zu aktualisieren, wenn sich die Verarbeitung wesentlich ändert — etwa durch neue Datenkategorien, neue Empfänger, den Wechsel des Cloud-Anbieters oder die Integration eines KI-Systems. Geringfügige Änderungen ohne Auswirkung auf das Risikoniveau erfordern keine vollständige Wiederholung, sollten aber dokumentiert werden.

### Wie lange muss eine DSFA aufbewahrt werden?

Eine DSFA ist Teil des Verzeichnisses der Verarbeitungstätigkeiten nach Art. 30 DSGVO und muss für die gesamte Dauer der Verarbeitung aktuell gehalten werden. Nach Einstellung der Verarbeitung empfehlen Aufsichtsbehörden eine Aufbewahrung von mindestens drei Jahren, da Betroffenenansprüche und Aufsichtsverfahren noch nachträglich eingeleitet werden können.

### Was ist der Unterschied zwischen DSFA und FRIA nach dem AI Act?

Die **DSFA** (Art. 35 DSGVO) bewertet Risiken für die Datenschutzrechte betroffener Personen und ist unabhängig vom AI Act. Die **FRIA** (*Fundamental Rights Impact Assessment*, Art. 27 AI Act) bewertet Risiken für alle Grundrechte durch Hochrisiko-KI-Systeme — also über den Datenschutz hinaus auch Diskriminierungsfreiheit, Würde, Rechtsstaatlichkeit. Beide Instrumente sind getrennt durchzuführen, können aber in einem gemeinsamen Dokument zusammengefasst werden, sofern alle Anforderungen beider Regelwerke vollständig erfüllt sind.
