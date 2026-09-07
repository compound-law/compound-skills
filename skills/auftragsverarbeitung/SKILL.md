---
name: auftragsverarbeitung
description: 'AVV rechtssicher gestalten: Art. 28 DSGVO-Anforderungen, Unterauftragnehmer-Regelungen und Drittlandtransfers anwaltlich prüfen — Bußgelder bis 10 Mio. EUR vermeiden.'
---


## Überblick

Dieser Skill leitet die Prüfung von Auftragsverarbeitungsverträgen (AVV) nach **Art. 28 DSGVO** an. Wenn ein Verantwortlicher einen Auftragsverarbeiter mit der Verarbeitung personenbezogener Daten beauftragt, ist ein schriftlicher AVV zwingend erforderlich (Art. 28 Abs. 3 DSGVO). Das Fehlen eines konformen AVV stellt einen eigenständigen DSGVO-Verstoß dar, der mit Bußgeldern bis zu 10 Mio. EUR oder 2 % des weltweiten Jahresumsatzes geahndet werden kann (**Art. 83 Abs. 4 lit. a DSGVO**). Dieser Skill ist anzuwenden beim Onboarding neuer Dienstleister, bei der Prüfung bestehender Auftragsverarbeitungsverhältnisse oder bei der Bewertung von AVV-Entwürfen der Anbieterseite. Wesentliche Vorschriften sind **Art. 28** (Pflichten des Auftragsverarbeiters), **Art. 32** (Sicherheit der Verarbeitung), **Art. 44-49** (internationale Übermittlungen) und **§ 62 BDSG** (zusätzliche deutsche Anforderungen für öffentliche Stellen).

In der Praxis werden die meisten AVV vom Auftragsverarbeiter erstellt und als nicht verhandelbar präsentiert. Der prüfende Rechtsanwalt muss die zwingenden Pflichtinhalte identifizieren, Abweichungen von den DSGVO-Anforderungen kennzeichnen und bewerten, ob die Risiko- und Verantwortungsverteilung für den Verantwortlichen akzeptabel ist. Deutsche Aufsichtsbehörden -- insbesondere die Landesdatenschutzbeauftragten (LfDI) und der Bundesdatenschutzbeauftragte (BfDI) -- haben detaillierte Leitlinien veröffentlicht und Bußgelder gezielt wegen mangelhafter AVV verhängt.

Betroffene Personen, deren Daten im Rahmen des AVV verarbeitet werden, haben Auskunftsrechte nach Art. 15 DSGVO — der Bearbeitungsprozess ist im Skill [DSGVO-Auskunftsanfrage](/de-DE/skills/dsgvo-auskunft/) beschrieben. Für KI-Systeme, die als Auftragsverarbeiter personenbezogene Daten verarbeiten, begründet der [KI-Verordnung Compliance-Check](/de-DE/skills/ki-verordnung-compliance/) zusätzliche Dokumentationspflichten neben dem AVV. Hinweisgebersysteme, die externe Plattformanbieter einsetzen, erfordern ebenfalls einen konformen AVV — den vollständigen Compliance-Rahmen beschreibt der Skill [Hinweisgebersystem-Einrichtung](/de-DE/skills/hinweisgebersystem/).


## Systematische Prüfung

### Schritt 1: Vorfrage -- Auftragsverarbeitung oder gemeinsame Verantwortlichkeit?

Vor der Prüfung des AVV ist zu klären, ob tatsächlich eine Auftragsverarbeitung (Art. 28 DSGVO) vorliegt oder ob es sich um eine gemeinsame Verantwortlichkeit (Art. 26 DSGVO) oder eigenständige Verantwortlichkeit handelt.

- **Abgrenzungstest:** Der Auftragsverarbeiter handelt ausschließlich auf Weisung des Verantwortlichen und hat keine eigenständige Entscheidungsbefugnis über die Zwecke und Mittel der Verarbeitung. Bestimmt der Auftragsverarbeiter eigene Zwecke (z. B. Nutzung der Daten für Produktverbesserung, Analyse oder eigenes Marketing), kann eine eigenständige oder gemeinsame Verantwortlichkeit vorliegen.
- **Indikatoren gemeinsamer Verantwortlichkeit (Art. 26 DSGVO):** Beide Parteien bestimmen gemeinsam die Zwecke und Mittel der Verarbeitung. Der EuGH hat eine weite Auslegung angenommen (C-210/16, Wirtschaftsakademie Schleswig-Holstein; C-40/17, Fashion ID). In der Praxis qualifizieren sich Plattformanbieter, Analysedienste und Werbenetzwerke häufig als gemeinsam Verantwortliche statt als Auftragsverarbeiter.
- **Folge der Fehleinordnung:** Wird das Verhältnis als Auftragsverarbeitung eingestuft, obwohl tatsächlich eine gemeinsame Verantwortlichkeit vorliegt, erfüllt der AVV nicht die Anforderungen des Art. 26 an eine Vereinbarung über die gemeinsame Verantwortlichkeit, und beide Parteien sind in Verstoß.

**Risikokennzeichnung:**
- Auftragsverarbeiter nutzt Daten des Verantwortlichen für eigene Analysen, Benchmarking oder KI-Training -- mögliche gemeinsame Verantwortlichkeit
- Kein klarer Weisungsrahmen -- Auftragsverarbeiter bestimmt Verarbeitungsparameter eigenständig
- Mehrseitige Datenflüsse, bei denen die Rollen nicht klar abgegrenzt sind

### Schritt 2: Pflichtinhalte (Art. 28 Abs. 3 DSGVO)

Der AVV muss die Kernparameter des Verarbeitungsverhältnisses festlegen und alle zwingenden Pflichten des Auftragsverarbeiters enthalten. Jede Auslassung macht den AVV nicht konform.

- **Verarbeitungsparameter (Art. 28 Abs. 3 S. 1):** Der AVV muss festlegen: (a) Gegenstand und Dauer der Verarbeitung, (b) Art und Zweck der Verarbeitung, (c) Art der verarbeiteten personenbezogenen Daten (z. B. Name, E-Mail, Gesundheitsdaten, Finanzdaten) und (d) Kategorien betroffener Personen (z. B. Beschäftigte, Kunden, Websitebesucher). Vage Beschreibungen wie "personenbezogene Daten, die im Zusammenhang mit den Dienstleistungen verarbeitet werden" sind unzureichend.
- **Pflichten des Auftragsverarbeiters (Art. 28 Abs. 3 lit. a-h):**
  - **(a) Dokumentierte Weisungen:** Verarbeitung nur auf dokumentierte Weisung des Verantwortlichen. Der Auftragsverarbeiter muss den Verantwortlichen informieren, falls eine Weisung gegen die DSGVO verstößt (Art. 28 Abs. 3 S. 3).
  - **(b) Vertraulichkeit:** Alle zur Verarbeitung befugten Personen müssen vertraglichen oder gesetzlichen Vertraulichkeitspflichten unterliegen.
  - **(c) Sicherheitsmaßnahmen:** Umsetzung geeigneter technischer und organisatorischer Maßnahmen nach Art. 32 DSGVO.
  - **(d) Unterauftragsverarbeitung:** Einhaltung der Voraussetzungen des Art. 28 Abs. 2 und 4.
  - **(e) Unterstützung bei Betroffenenrechten:** Unterstützung bei der Beantwortung von Anfragen betroffener Personen (Auskunft, Berichtigung, Löschung, Datenübertragbarkeit, Einschränkung, Widerspruch).
  - **(f) Unterstützung bei Sicherheits- und DSFA-Pflichten:** Unterstützung bei Pflichten nach Art. 32-36 (Sicherheit, Meldung von Datenschutzverletzungen, Datenschutz-Folgenabschätzung).
  - **(g) Löschung oder Rückgabe:** Nach Wahl des Verantwortlichen bei Beendigung alle personenbezogenen Daten löschen oder zurückgeben und vorhandene Kopien löschen, es sei denn, EU- oder mitgliedstaatliches Recht erfordert die Aufbewahrung.
  - **(h) Audit und Überprüfung:** Dem Verantwortlichen alle Informationen zur Verfügung stellen, die zum Nachweis der Compliance erforderlich sind, und Überprüfungen -- einschließlich Inspektionen -- ermöglichen und dazu beitragen.

**Risikokennzeichnung:**
- Zwingender Inhalt aus Art. 28 Abs. 3 lit. a-h fehlt vollständig
- Verarbeitungszweck in vagen Begriffen beschrieben, die Zweckausdehnung ermöglichen
- Keine Pflicht zur Verarbeitung nur auf dokumentierte Weisung
- Vertraulichkeitspflicht auf "angemessene Bemühungen" beschränkt statt einer bindenden Verpflichtung
- Keine Pflicht, den Verantwortlichen bei weisungswidrigem Handeln zu informieren

### Schritt 3: Unterauftragsverarbeitung (Art. 28 Abs. 2, 4 DSGVO)

Der Auftragsverarbeiter darf ohne vorherige Genehmigung des Verantwortlichen keinen weiteren Auftragsverarbeiter (Unterauftragsverarbeiter) einschalten.

- **Genehmigungsmodell:** Zwei Optionen: (a) gesonderte vorherige schriftliche Genehmigung für jeden namentlich benannten Unterauftragsverarbeiter oder (b) allgemeine schriftliche Genehmigung mit Benachrichtigungs- und Widerspruchsmechanismus.
- **Liste der Unterauftragsverarbeiter:** Der Auftragsverarbeiter sollte eine aktuelle Liste aller Unterauftragsverarbeiter bereitstellen, einschließlich Name, Standort und der von ihnen durchgeführten Verarbeitungstätigkeiten.
- **Änderungsbenachrichtigung bei allgemeiner Genehmigung:** Der Auftragsverarbeiter muss über beabsichtigte Hinzufügungen oder Ersetzungen informieren und dem Verantwortlichen Gelegenheit zum Widerspruch geben. Die Benachrichtigungsfrist muss angemessen sein -- 14-30 Tage sind marktüblich. Kürzere Fristen (z. B. 7 Tage) oder Zustimmungsfiktionen (Schweigen gilt als Zustimmung) sind problematisch.
- **Widerspruchsrecht und Folgen:** Bei Widerspruch sollte der Auftragsverarbeiter verpflichtet sein, den Unterauftragsverarbeiter nicht einzuschalten oder Alternativen vorzuschlagen. Wird keine Einigung erzielt, sollte der Verantwortliche ein Kündigungsrecht ohne Vertragsstrafe haben. Klauseln, die die Vertragskündigung als einziges Rechtsmittel ohne Übergangsfrist oder Datenmigrationshilfe vorsehen, sind einseitig.
- **Back-to-Back-Pflichten (Art. 28 Abs. 4 DSGVO):** Der Auftragsverarbeiter muss dem Unterauftragsverarbeiter dieselben Datenschutzpflichten auferlegen wie im AVV enthalten.
- **Haftung für Verstöße des Unterauftragsverarbeiters:** Nach Art. 28 Abs. 4 S. 2 DSGVO haftet der Auftragsverarbeiter dem Verantwortlichen gegenüber uneingeschränkt für die Einhaltung der Pflichten des Unterauftragsverarbeiters.

**Risikokennzeichnung:**
- Keine Liste der Unterauftragsverarbeiter bereitgestellt oder Liste veraltet
- Widerspruchsfrist kürzer als 14 Tage oder Widerspruchsrecht illusorisch (Zustimmungsfiktion)
- Kein Back-to-Back-Vertrag mit Unterauftragsverarbeitern
- Einziges Rechtsmittel des Verantwortlichen bei Widerspruch ist sofortige Vertragskündigung ohne Übergangsfrist
- Auftragsverarbeiter lehnt Haftung für Verstöße der Unterauftragsverarbeiter ab trotz Art. 28 Abs. 4 S. 2 DSGVO

### Schritt 4: Internationale Übermittlungsmechanismen (Art. 44-49 DSGVO)

Werden personenbezogene Daten außerhalb des EWR übermittelt (an den Auftragsverarbeiter, einen Unterauftragsverarbeiter oder eine Datenspeicherinfrastruktur), ist die Rechtsgrundlage für jede Übermittlung zu prüfen.

- **Angemessenheitsbeschluss (Art. 45 DSGVO):** Prüfen Sie, ob für das Empfängerland ein gültiger Angemessenheitsbeschluss vorliegt. Aktuelle Beschlüsse bestehen u.a. für: Japan, Südkorea, Vereinigtes Königreich, Kanada (kommerzielle Organisationen), Argentinien, Israel, Neuseeland, Schweiz, Uruguay und die USA (EU-US Data Privacy Framework, DPF, angenommen am 10. Juli 2023).
- **Standardvertragsklauseln (SCCs):** Die aktuellen SCCs wurden durch Durchführungsbeschluss 2021/914 angenommen. Bestätigen Sie das korrekte Modul: **Modul 2** (Verantwortlicher an Auftragsverarbeiter) oder **Modul 3** (Auftragsverarbeiter an Unterauftragsverarbeiter). Prüfen Sie, ob **Anhang I** (Parteien, Datenübermittlungen, zuständige Aufsichtsbehörde) und **Anhang II** (TOMs) vollständig mit konkreten Angaben ausgefüllt sind.
- **Transfer Impact Assessment (TIA):** Nach der Schrems-II-Entscheidung (EuGH, C-311/18) müssen Parteien, die sich auf SCCs stützen, bewerten, ob das Rechtssystem des Empfängerlandes im Wesentlichen gleichwertigen Schutz bietet. Die Bewertung muss Überwachungsgesetze, Zugang durch Behörden, wirksame Rechtsbehelfe und die konkreten Umstände der Übermittlung berücksichtigen.
- **Übermittlungen in die USA unter dem DPF:** Der DPF-Angemessenheitsbeschluss erfasst Übermittlungen an US-Organisationen, die unter dem DPF selbstzertifiziert sind. Prüfen Sie den aktiven Zertifizierungsstatus unter dataprivacyframework.gov.
- **Binding Corporate Rules (Art. 47 DSGVO):** Alternative für konzerninterne Übermittlungen mit Genehmigung der federführenden Aufsichtsbehörde.

**Risikokennzeichnung:**
- Datenübermittlung in ein Drittland ohne identifizierte Rechtsgrundlage
- SCCs verwendet, aber Anhang I und II nicht oder mit generischem Text ausgefüllt
- Kein TIA trotz Übermittlung in ein Land ohne Angemessenheitsbeschluss durchgeführt
- US-Empfänger nicht unter dem EU-US DPF zertifiziert trotz Berufung auf den Angemessenheitsbeschluss
- Unterauftragsverarbeiter in Drittstaat nicht in der Liste offengelegt

### Schritt 5: Technische und organisatorische Maßnahmen (Art. 32 DSGVO)

Der AVV muss konkrete TOMs enthalten oder referenzieren, die dem Risiko der Verarbeitungstätigkeiten angemessen sind. Deutsche Aufsichtsbehörden betonen, dass generische, formelhafte TOMs die DSGVO nicht erfüllen.

- **Pseudonymisierung und Verschlüsselung (Art. 32 Abs. 1 lit. a):** Prüfen Sie konkrete Zusagen: Verschlüsselung im Ruhezustand (AES-256 oder gleichwertig), Verschlüsselung bei der Übertragung (TLS 1.2+) und Pseudonymisierung personenbezogener Daten, soweit die Verarbeitung keine direkte Identifizierung erfordert.
- **Vertraulichkeit, Integrität, Verfügbarkeit, Belastbarkeit (Art. 32 Abs. 1 lit. b):** Maßnahmen müssen adressieren: Zugangskontrollen (rollenbasiert, Prinzip der geringsten Berechtigung), Netzwerksicherheit, physische Sicherheit der Rechenzentren, Business Continuity und Disaster Recovery sowie mandantenspezifische Datentrennung.
- **Regelmäßige Überprüfung (Art. 32 Abs. 1 lit. d):** Verfahren zur regelmäßigen Prüfung, Bewertung und Evaluierung der Wirksamkeit der TOMs, einschließlich Penetrationstests, Schwachstellenscans und Mitarbeiterschulungen.
- **Wiederherstellungsmaßnahmen (Art. 32 Abs. 1 lit. c):** Maßnahmen zur raschen Wiederherstellung des Zugangs zu personenbezogenen Daten nach einem physischen oder technischen Zwischenfall. Prüfen Sie zugesagte Recovery Time Objectives (RTO) und Recovery Point Objectives (RPO).
- **Konkretisierungsgrad:** Die TOMs müssen so konkret sein, dass sie überprüfbar sind. "Branchenübliche Sicherheitsmaßnahmen" oder "geeignete technische Maßnahmen" ohne weitere Spezifizierung erfüllen die Art.-32-Anforderung nicht. Best Practice: ein gesonderter Anhang mit strukturierter Aufschlüsselung nach Kategorien.

**Risikokennzeichnung:**
- TOMs völlig generisch oder formelhaft, ohne Bezug zu den tatsächlichen Verarbeitungstätigkeiten
- Keine Zusage zur Verschlüsselung im Ruhezustand oder bei der Übertragung für sensible Datenkategorien
- Kein Verfahren für regelmäßige Sicherheitsüberprüfung oder Penetrationstests
- RTO und RPO nicht definiert
- TOMs seit der ursprünglichen AVV-Unterzeichnung nicht aktualisiert trotz technologischer Änderungen

### Schritt 6: Auditrechte (Art. 28 Abs. 3 lit. h DSGVO)

Der Verantwortliche hat ein gesetzliches Recht zur Überprüfung des Auftragsverarbeiters. Dieses Recht ist nicht abdingbar, wird aber in AVV-Entwürfen der Auftragsverarbeiterseite häufig eingeschränkt.

- **Vorankündigungsfrist:** Eine angemessene Frist (14-30 Tage) ist akzeptabel. Fristen über 30 Tage sind übermäßig.
- **Häufigkeit:** Beschränkung auf ein routinemäßiges Audit pro Jahr ist üblich und grundsätzlich akzeptabel, sofern der Verantwortliche das Recht auf zusätzliche Audits aus besonderem Anlass behält (z. B. nach Datenschutzvorfall, behördlicher Anfrage oder begründeter Beschwerde).
- **Prüferauswahl:** Klauseln, die den Verantwortlichen zur Beauftragung eines vom Auftragsverarbeiter ausgewählten Prüfers verpflichten, untergraben die Unabhängigkeit. Der Verantwortliche sollte das Recht haben, seinen eigenen Prüfer zu bestellen.
- **Kostentragung:** Praxis variiert. Kostentragung durch den Verantwortlichen für routinemäßige Audits ist akzeptabel; bei Feststellung wesentlicher Mängel sollten die Kosten auf den Auftragsverarbeiter übergehen.
- **Akzeptable Alternativen:** Drittanbieter-Zertifizierungen (ISO 27001, SOC 2 Type II) und standardisierte Auditberichte können ergänzen -- aber nicht ersetzen --, solange der Verantwortliche das Recht auf eigene Audits bei begründetem Anlass behält.

**Risikokennzeichnung:**
- Auditrecht auf Prüfung von Selbstzertifizierungen oder Zusammenfassungen beschränkt
- Kein zusätzliches Auditrecht im Falle eines Datenschutzvorfalls oder einer behördlichen Anfrage
- Sämtliche Auditkosten vom Verantwortlichen zu tragen, unabhängig von den Ergebnissen
- Auftragsverarbeiter kann Audit aus "Geschäftsgeheimnissen" verweigern ohne angemessene Begrenzung
- Auditrecht durch kumulative Verfahrenseinschränkungen faktisch ausgehöhlt

### Schritt 7: Meldung von Datenschutzverletzungen, Löschung und Haftung

Bestätigen Sie die Pflichten nach einem Datenschutzvorfall und nach Vertragsende sowie die interne Haftungsverteilung.

- **Meldung von Datenschutzverletzungen (Art. 33 Abs. 2 DSGVO):** Der Auftragsverarbeiter muss den Verantwortlichen **unverzüglich** nach Kenntnis einer Verletzung des Schutzes personenbezogener Daten benachrichtigen. Prüfen Sie die konkrete Meldefrist im AVV -- "72 Stunden" spiegelt die Pflicht des Verantwortlichen gegenüber der Aufsichtsbehörde wider und ist eine angemessene Verpflichtung. Längere Fristen (z. B. "innerhalb von 5 Werktagen") können den Verantwortlichen daran hindern, seine eigene 72-Stunden-Frist einzuhalten.
- **Inhalt der Meldung:** Art der Verletzung, Kategorien und ungefähre Anzahl betroffener Personen, wahrscheinliche Folgen und ergriffene oder vorgeschlagene Maßnahmen.
- **Datenrückgabe oder Löschung (Art. 28 Abs. 3 lit. g DSGVO):** Nach Wahl des Verantwortlichen bei Beendigung alle personenbezogenen Daten löschen oder zurückgeben. Schriftliche Löschbestätigung innerhalb einer definierten Frist (30 Tage sind marktüblich).
- **Aufbewahrung nach Beendigung:** Der Auftragsverarbeiter darf Daten über die Beendigung hinaus nur aufbewahren, soweit EU- oder mitgliedstaatliches Recht dies erfordert. Verarbeitung zu eigenen Zwecken (Analyse, Produktverbesserung) ist unzulässig.
- **Haftungsverteilung (Art. 82 DSGVO):** Die DSGVO sieht eine gesamtschuldnerische Haftung gegenüber Betroffenen vor. Die interne Verteilung zwischen Verantwortlichem und Auftragsverarbeiter sollte im AVV geregelt werden. Haftungsobergrenzen auf Vertragswert oder Ausschluss von Folgeschäden können die Möglichkeit des Verantwortlichen untergraben, durchgereichte Bußgelder zu regressieren.
- **Freistellung für aufsichtsrechtliche Bußgelder:** Deutsche Gerichte lassen Freistellungsklauseln für Bußgelder grundsätzlich zu, die Durchsetzbarkeit bleibt aber umstritten, wenn das Bußgeld eigenes Verschulden der freistellungsberechtigten Partei ahndet.

**Risikokennzeichnung:**
- Keine Löschungspflicht oder keine Löschbestätigung
- Meldefrist für Datenschutzverletzungen übersteigt die für die Einhaltung der 72-Stunden-Frist des Verantwortlichen erforderliche Zeit
- Auftragsverarbeiter behält Daten nach Beendigung für "Analysen" oder "Produktverbesserung"
- Haftung des Auftragsverarbeiters auf eine Monatsvergütung begrenzt, während dem Verantwortlichen Bußgelder in Millionenhöhe drohen
- Keine Freistellungsregelung für Bußgelder, die durch Verstöße des Auftragsverarbeiters verursacht wurden


## Besondere Szenarien

### SaaS-Anbieter-AVV

SaaS-AVV sind typischerweise nicht verhandelbar. Fokussieren Sie auf:

- **Unterauftragsverarbeiter-Proliferation:** Große SaaS-Anbieter listen ggf. Dutzende Unterauftragsverarbeiter. Prüfen Sie Aktualität und ob der Änderungsbenachrichtigungsmechanismus echte Widerspruchsmöglichkeit bietet.
- **Datenstandort:** Bestätigen Sie, ob Daten ausschließlich im EWR oder auch in Drittländern gespeichert werden. "EU-Datenresidenz"-Optionen können gegen Aufpreis verfügbar sein.
- **Verschlüsselung und Zugang:** Prüfen Sie, ob der Anbieter auf unverschlüsselte Kundendaten zugreifen kann. BYOK- oder HYOK-Verschlüsselung kann den Zugangsrisiko mindern.
- **EU Data Act — Portabilität und Anbieterwechsel (ab 12. September 2025):** Seit dem **EU Data Act** (Verordnung (EU) 2023/2854, Art. 23–31) müssen Cloud- und SaaS-Anbieter aktiv den Wechsel zu alternativen Diensten ermöglichen. Ein DSGVO-konformer AVV allein genügt nicht mehr für einen vollständig marktkonformen Vertrag: Prüfen Sie, ob der AVV oder der zugehörige Hauptvertrag standardisierte Exportschnittstellen, maximale Wechselgebühren (ab Ende 2027 kostenfrei) und eine Mindest-Übergangsphase von 30 Tagen vorsieht. Ältere AVV-Templates erfüllen diese Anforderungen regelmäßig nicht und sind bei der nächsten Vertragsverlängerung anzupassen (→ [SaaS-Vertrag prüfen lassen](/de-DE/skills/saas-vertragspruefung/)).
- **DORA — IKT-Drittanbieterverträge für Finanzunternehmen (ab 17. Januar 2025):** Ist der Auftragsverarbeiter ein IKT-Drittanbieter eines Finanzunternehmens, gelten neben dem AVV nach Art. 28 DSGVO die Mindestanforderungen des **Digital Operational Resilience Act** (Verordnung (EU) 2022/2554, Art. 30). Der Vertrag muss dann zwingend Auditrechte für zuständige Aufsichtsbehörden (EBA, BaFin), Unterstützungspflichten bei IKT-Vorfällen und eine dokumentierte Exit-Strategie enthalten. Ein DSGVO-AVV ohne diese DORA-Klauseln ist für Finanzunternehmen unvollständig.

### Konzerninterne AVV

Konzerninterne Verarbeitung (z. B. Shared Service Center, zentrale HR-Systeme) erfordert ebenfalls einen AVV. Die DSGVO gewährt kein Konzernprivileg. Ein separater AVV ist erforderlich, auch wenn Binding Corporate Rules als Übermittlungsmechanismus dienen.

### Deutscher öffentlicher Sektor (§ 62 BDSG)

Öffentliche Stellen in Deutschland müssen zusätzliche Anforderungen des § 62 BDSG erfüllen, der Art. 28 DSGVO mit spezifischen Vorschriften für den öffentlichen Sektor ergänzt, insbesondere im Anwendungsbereich der Richtlinie (EU) 2016/680 (Datenschutz bei der Strafverfolgung).


## Grenzen dieses Skills

Dieser Skill bietet eine strukturierte Erstbewertung. In folgenden Fällen ist die Einschaltung eines Rechtsanwalts erforderlich:

- **Verhandlung von AVV-Bedingungen** mit großen Cloud-Anbietern oder SaaS-Anbietern, insbesondere bei wesentlichen Mängeln des Standard-AVV
- **Transfer Impact Assessments** mit Analyse der Überwachungsgesetze des Drittlandes und ergänzender Maßnahmen
- **Reaktion auf Datenschutzverletzungen**, bei denen der Verstoß des Auftragsverarbeiters Meldepflichten des Verantwortlichen nach Art. 33/34 DSGVO auslöst
- **Aufsichtsverfahren** oder Audits, die das Auftragsverarbeitungsverhältnis betreffen
- **Komplexe Mehrparteien-Verarbeitungsstrukturen** mit gemeinsam Verantwortlichen, mehreren Auftragsverarbeitern und Unterauftragsverarbeitern über Jurisdiktionen hinweg
- **Sektorspezifische Anforderungen** für Finanzdienstleistungen (DORA Art. 30, BaFin-Leitlinien zur Auslagerung, MaRisk AT 9), Gesundheitswesen (§ 203 StGB Berufsgeheimnis) oder Telekommunikation (§ 3 TTDSG)

Compound unterstützt gerne bei der Prüfung, Verhandlung und Gestaltung von AVV, die den Anforderungen der DSGVO und des BDSG entsprechen.
