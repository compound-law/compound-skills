---
name: ki-verordnung-compliance
description: 'EU AI Act Compliance umsetzen: KI-Systeme nach EU-KI-Verordnung (VO 2024/1689) klassifizieren, Dokumentationspflichten erfüllen und Konformitätsbewertung durchführen.'
---


## Überblick

Dieser Skill bietet eine strukturierte Compliance-Bewertung für KI-Systeme nach der **Verordnung (EU) 2024/1689** -- dem EU AI Act. Die Verordnung etabliert einen risikobasierten Regulierungsrahmen mit vier Stufen: unannehmbares Risiko (verboten), hohes Risiko (streng reguliert), begrenztes Risiko (Transparenzpflichten) und minimales Risiko (weitgehend unreguliert). Zentrale Vorschriften sind **Art. 5** (verbotene KI-Praktiken), **Art. 6** (Einstufung von Hochrisiko-Systemen), **Art. 8-15** (Anforderungen an Hochrisiko-Systeme), **Art. 26** (Betreiberpflichten) und **Art. 50** (Transparenzpflichten). Dieser Skill ist anzuwenden bei der Beratung zur Einführung, Beschaffung oder Entwicklung von KI-Systemen innerhalb der EU oder bei einer Compliance-Gap-Analyse bestehender Systeme.

Der AI Act gilt für Anbieter, Betreiber, Importeure und Händler von KI-Systemen, die auf dem EU-Markt bereitgestellt werden oder deren Output in der EU genutzt wird, unabhängig vom Sitz des Anbieters (Art. 2 Abs. 1). Deutsche Unternehmen müssen zudem das Zusammenspiel mit der DSGVO, sektorspezifischer Regulierung (z. B. MDR für medizinische KI, MiFID II für Finanz-KI, Produkthaftungsrichtlinie) und den zu erwartenden nationalen Durchführungsbestimmungen berücksichtigen. Die extraterritoriale Reichweite bedeutet, dass auch Nicht-EU-Anbieter mit EU-Kunden erfasst werden.

KI-Systeme, die personenbezogene Daten verarbeiten, erfordern parallel einen konformen [Auftragsverarbeitungsvertrag (AVV)](/de-DE/skills/auftragsverarbeitung/) nach Art. 28 DSGVO. Betroffene Personen, die automatisierten Entscheidungen nach Art. 22 DSGVO unterliegen, haben weitergehende Auskunftsrechte — der Bearbeitungsprozess ist im Skill [DSGVO-Auskunftsanfrage](/de-DE/skills/dsgvo-auskunft/) beschrieben. Unternehmen, die KI-gestützte Mitarbeiterüberwachung einsetzen, müssen zudem prüfen, ob ein [Hinweisgebersystem](/de-DE/skills/hinweisgebersystem/) nach HinSchG einschlägig ist — § 87 Abs. 1 Nr. 6 BetrVG greift bei technischen Überwachungseinrichtungen.


## Systematische Prüfung

### Schritt 1: Akteursklassifizierung und Anwendungsbereich

Bestimmen Sie die Rolle des Unternehmens nach dem AI Act und bestätigen Sie, dass das System in den Anwendungsbereich fällt. Die Pflichten unterscheiden sich erheblich je nach Akteursklassifizierung.

- **KI-System-Definition (Art. 3 Nr. 1):** Ein maschinengestütztes System, das mit unterschiedlichem Grad an Autonomie betrieben wird, das nach der Inbetriebnahme Anpassungsfähigkeit aufweisen kann und das Outputs wie Vorhersagen, Inhalte, Empfehlungen oder Entscheidungen erzeugt, die physische oder virtuelle Umgebungen beeinflussen. Diese Definition ist bewusst weit gefasst und erfasst maschinelles Lernen, regelbasierte Systeme und hybride Ansätze.
- **Anbieter (Art. 3 Nr. 3):** Entwickelt oder beauftragt ein KI-System und bringt es unter eigenem Namen oder eigener Marke in Verkehr oder nimmt es in Betrieb. Der Anbieter trägt die umfassendsten Compliance-Pflichten, einschließlich Konformitätsbewertung, technische Dokumentation und Marktüberwachung nach dem Inverkehrbringen.
- **Betreiber (Art. 3 Nr. 4):** Nutzt ein KI-System unter eigener Verantwortung, ausgenommen persönliche nicht-professionelle Nutzung. Unternehmen, die Standard-KI-Tools nutzen, gelten als Betreiber und tragen eigenständige Pflichten nach Art. 26.
- **Doppelrollen:** Ein Unternehmen kann gleichzeitig Anbieter und Betreiber sein -- beispielsweise bei Entwicklung eines KI-Systems für den eigenen Gebrauch. Beide Pflichtenkataloge gelten kumulativ.
- **Ausnahmen (Art. 2):** Militär und nationale Sicherheit (Art. 2 Abs. 3), ausschließlich für wissenschaftliche Forschung genutzte Systeme (Art. 2 Abs. 6) und Open-Source-Systeme mit Ausnahmen für Hochrisiko- und verbotene Kategorien (Art. 2 Abs. 12).

**Risikokennzeichnung:**
- Unternehmen handelt als Anbieter und Betreiber zugleich, ohne die doppelten Pflichten zu erkennen
- Open-Source-Ausnahme beansprucht, ohne zu prüfen, ob ein Anhang-III-Anwendungsfall vorliegt
- KI-System wird in der EU genutzt, aber Anbieter geht davon aus, dass der AI Act wegen Sitz außerhalb der EU nicht gilt
- Enge Auslegung des KI-System-Begriffs, um regelbasierte Entscheidungssysteme auszuschließen, die unter die Definition fallen können
- Nicht alle Akteure in der Wertschöpfungskette identifiziert (z. B. Wiederverkäufer als Händler)

### Schritt 2: Prüfung verbotener Praktiken (Art. 5)

Prüfen Sie, ob das KI-System eine der acht verbotenen Praktiken ausübt. Diese Verbote gelten seit dem **2. Februar 2025** und sind mit den höchsten Sanktionen belegt (bis zu 35 Mio. EUR oder 7 % des weltweiten Jahresumsatzes).

- **Unterschwellige Manipulation (Art. 5 Abs. 1 lit. a):** Techniken, die unterschwellige Elemente einsetzen, die einer Person nicht bewusst wahrnehmbar sind und ihr Verhalten wesentlich verzerren und erheblichen Schaden verursachen.
- **Ausnutzung von Schwachstellen (Art. 5 Abs. 1 lit. b):** Gezieltes Ansprechen bestimmter Gruppen aufgrund von Alter, Behinderung oder sozialer/wirtschaftlicher Lage zur wesentlichen Verhaltensverzerrung mit Schadensfolge.
- **Social Scoring (Art. 5 Abs. 1 lit. c):** Klassifizierung von Personen auf Grundlage sozialen Verhaltens oder persönlicher Merkmale, wenn der resultierende Score zu einer ungerechtfertigten oder unverhältnismäßigen nachteiligen Behandlung führt.
- **Vorhersage von Straftaten (Art. 5 Abs. 1 lit. d):** Individuelle Risikobewertung zur Vorhersage von Straftaten allein auf Grundlage von Profiling oder Persönlichkeitsmerkmalen.
- **Biometrische Echtzeit-Fernidentifizierung (Art. 5 Abs. 1 lit. h):** In öffentlich zugänglichen Räumen zu Strafverfolgungszwecken, mit engen Ausnahmen, die eine vorherige richterliche Genehmigung erfordern.
- **Emotionserkennung (Art. 5 Abs. 1 lit. f):** Am Arbeitsplatz und in Bildungseinrichtungen, außer aus medizinischen oder Sicherheitsgründen.
- **Anlassloses Gesichtsbilder-Scraping (Art. 5 Abs. 1 lit. e):** Erstellung oder Erweiterung von Gesichtserkennungsdatenbanken durch anlassloses Scraping von Gesichtsbildern aus dem Internet oder aus Videoüberwachung.
- **Biometrische Kategorisierung (Art. 5 Abs. 1 lit. g):** Nutzung biometrischer Daten zur Ableitung sensibler Merkmale wie Rasse, politische Meinungen, Gewerkschaftszugehörigkeit, religiöse Überzeugungen oder sexuelle Orientierung.

**Risikokennzeichnung:**
- Jede Übereinstimmung mit einer verbotenen Praktik erfordert sofortige Einstellung oder grundlegende Umgestaltung
- System verwendet biometrische Daten ohne klare Rechtfertigung unter einer zulässigen Ausnahme
- Emotionserkennung im Arbeitsumfeld, auch wenn als "freiwillig" oder für "Wohlbefinden" deklariert
- Persuasive KI in Marketing, die die Grenze zur unterschwelligen Manipulation überschreiten kann
- Social-Scoring-Elemente in Bonitäts- oder Versicherungsbewertungen durch öffentliche Stellen

### Schritt 3: Risikoklassifizierung (Art. 6 und Anhänge I/III)

Ist das System nicht verboten, ist zu prüfen, ob es als Hochrisiko-System einzustufen ist. Diese Einstufung ist die Eintrittsschwelle zu den anspruchsvollsten Compliance-Anforderungen.

- **Anhang-I-Pfad (Sicherheitskomponente):** Das System ist eine Sicherheitskomponente eines Produkts oder selbst ein Produkt, das unter harmonisiertes EU-Recht gemäß Anhang I fällt. Dies umfasst Maschinen (Verordnung 2023/1230), Medizinprodukte (MDR 2017/745), In-vitro-Diagnostika (IVDR 2017/746), Kraftfahrzeuge (Verordnung 2019/2144), Luftfahrt, Schienenverkehr, Spielzeug, Aufzüge und Druckgeräte.
- **Anhang-III-Pfad (eigenständiges Hochrisiko-System):** Das System fällt unter eine der acht Kategorien: (1) biometrische Identifizierung und Kategorisierung, (2) Betrieb kritischer Infrastruktur, (3) Bildung und Berufsausbildung, (4) Beschäftigung und Arbeitnehmerführung, (5) Zugang zu wesentlichen Dienstleistungen, (6) Strafverfolgung, (7) Migration, Asyl und Grenzkontrolle, (8) Rechtspflege und demokratische Prozesse.
- **Art. 6 Abs. 3-Ausnahme:** Ein in Anhang III aufgeführtes System ist nicht hochriskant, wenn es kein signifikantes Schadensrisiko birgt, das Ergebnis der Entscheidungsfindung nicht wesentlich beeinflusst (d. h. rein vorbereitend ist) und keine natürlichen Personen profiliert. Der Anbieter muss die Bewertung dokumentieren und die zuständige nationale Behörde vor dem Inverkehrbringen benachrichtigen.
- **KI-Modelle mit allgemeinem Verwendungszweck (Art. 51-56):** Modelle, die mit großen Datenmengen durch Selbstüberwachung trainiert wurden und erhebliche Allgemeinheit aufweisen. Anbieter von GPAI-Modellen unterliegen Transparenzpflichten (Art. 53) und bei systemischem Risiko (kumulativer Rechenaufwand über 10^25 FLOPS oder Einstufung durch das AI Office) zusätzlichen Pflichten einschließlich Adversarial Testing, Vorfallmeldung und Cybersicherheitsmaßnahmen (Art. 55).

**Risikokennzeichnung:**
- Klassifizierungsbegründung nicht dokumentiert (Art. 6 Abs. 4)
- Art. 6 Abs. 3-Ausnahme beansprucht ohne schriftliche Begründung oder ohne Benachrichtigung der nationalen Behörde
- System fällt eindeutig unter Anhang III, wird aber als System mit begrenztem Risiko behandelt
- GPAI-Modell-Anbieter kennt die Schwelle für systemisches Risiko nicht
- KI-System in ein Produkt eingebettet, das unter harmonisiertes Recht nach Anhang I reguliert ist, ohne Koordination mit der Produkt-Konformitätsbewertung

### Schritt 4: Anforderungen an Hochrisiko-Systeme (Art. 8-15, Art. 26)

Für als hochriskant eingestufte Systeme ist die Einhaltung jeder zwingenden Anforderung zu bestätigen. Die Pflichten treffen Anbieter (Art. 8-15) und Betreiber (Art. 26) mit unterschiedlichem Umfang.

- **Risikomanagementsystem (Art. 9):** Ein kontinuierlicher, iterativer Prozess zur Identifizierung, Analyse, Bewertung und Evaluierung von Risiken. Das System muss über den gesamten Lebenszyklus des KI-Systems eingerichtet, dokumentiert, umgesetzt und aufrechterhalten werden.
- **Datengovernance (Art. 10):** Trainings-, Validierungs- und Testdatensätze müssen relevant, hinreichend repräsentativ und soweit möglich fehlerfrei sein. Maßnahmen zur Erkennung und Minderung von Verzerrungen (Bias) sind zwingend. Art. 10 Abs. 5 schafft eine begrenzte Ausnahme für die Verarbeitung besonderer Kategorien personenbezogener Daten (Art. 9 DSGVO) zur Bias-Überwachung unter strengen Auflagen.
- **Technische Dokumentation (Art. 11, Anhang IV):** Umfassende Dokumentation zu allgemeiner Systembeschreibung, detaillierter Entwicklungsmethodik, Überwachungs- und Kontrollmechanismen, Risikomanagementprozess und Änderungsprotokoll. Dokumentation muss vor dem Inverkehrbringen erstellt und aktuell gehalten werden.
- **Aufzeichnungspflichten und Protokollierung (Art. 12):** Automatische Aufzeichnung von Ereignissen (Logs) zur Rückverfolgbarkeit über den gesamten Lebenszyklus. Aufbewahrung mindestens sechs Monate, sofern nicht anders gesetzlich vorgeschrieben.
- **Transparenz und Information an Betreiber (Art. 13):** Klare, prägnante Gebrauchsanweisungen einschließlich Fähigkeiten, Einschränkungen, Zweckbestimmung, vorhersehbarer Fehlanwendungen und Leistungskennzahlen.
- **Menschliche Aufsicht (Art. 14):** Maßnahmen, die eine wirksame menschliche Überwachung während des Betriebs ermöglichen. Die Aufsichtsperson muss die Fähigkeiten und Grenzen des Systems verstehen, Outputs korrekt interpretieren, sich gegen das Output entscheiden und das System stoppen können. Bloßes Abnicken erfüllt die Anforderung nicht.
- **Genauigkeit, Robustheit, Cybersicherheit (Art. 15):** Angemessene Niveaus über den gesamten Lebenszyklus, einschließlich Resilienz gegen Manipulationsversuche (Data Poisoning, Adversarial Attacks).

**Betreiber-spezifische Pflichten (Art. 26):**
- Nutzung des Systems gemäß der Gebrauchsanweisung des Anbieters
- Einsatz kompetenter, geschulter und autorisierter Personen für die menschliche Aufsicht
- Überwachung des Systembetriebs und Meldung von Vorfällen
- Durchführung einer **Grundrechtsfolgenbewertung (FRIA)** nach Art. 27 vor dem Einsatz von Hochrisiko-Systemen in bestimmten Kategorien (Kreditbewertung, Versicherungstarife, Personalauswahl, öffentliche Dienstleistungen)
- Information natürlicher Personen, dass sie einem Hochrisiko-KI-System unterliegen

**Risikokennzeichnung:**
- Kein dokumentierter Risikomanagementprozess oder Prozess auf einmalige Bewertung bei Inbetriebnahme beschränkt
- Herkunft der Trainingsdaten unbekannt oder nicht dokumentiert, Bias-Bewertung unmöglich
- Menschliche Aufsicht rein nominell, ohne praktische Möglichkeit zur Intervention oder Außerkraftsetzung
- FRIA nicht durchgeführt, wo Art. 27 dies erfordert
- Protokollierung deaktiviert oder Aufbewahrungsfrist unzureichend
- Technische Dokumentation unvollständig oder nach wesentlichen Änderungen nicht aktualisiert

### Schritt 5: Transparenzpflichten für alle KI-Systeme (Art. 50)

Auch Systeme, die nicht als hochriskant eingestuft sind, müssen Transparenzanforderungen erfüllen, wenn sie mit natürlichen Personen interagieren oder synthetische Inhalte erzeugen.

- **Offenlegung der KI-Interaktion (Art. 50 Abs. 1):** Anbieter von KI-Systemen, die für die direkte Interaktion mit natürlichen Personen bestimmt sind (Chatbots, virtuelle Assistenten, Kundenservice-Agenten), müssen sicherstellen, dass das System offenlegt, dass der Nutzer mit einer KI interagiert.
- **Kennzeichnung synthetischer Inhalte (Art. 50 Abs. 2):** Anbieter von KI-Systemen, die synthetische Audio-, Bild-, Video- oder Textinhalte erzeugen, müssen sicherstellen, dass die Outputs in maschinenlesbarem Format als künstlich erzeugt oder manipuliert gekennzeichnet werden.
- **Emotionserkennung und biometrische Kategorisierung (Art. 50 Abs. 3):** Betroffene Personen müssen informiert werden.
- **Transparenz bei Allgemein-KI-Modellen (Art. 53):** GPAI-Modell-Anbieter müssen technische Dokumentation erstellen, EU-Urheberrecht einhalten und eine hinreichend detaillierte Zusammenfassung der Trainingsdateninhalte veröffentlichen.

**Risikokennzeichnung:**
- Kein Offenlegungsmechanismus für KI-generierte Inhalte, insbesondere in kundengerichteten Anwendungen
- Deepfake-fähiges System ohne maschinenlesbare Output-Kennzeichnung
- Chatbot oder virtueller Assistent ohne KI-Offenlegung eingesetzt
- KI-generierter Text in rechtlichen, medizinischen oder finanziellen Mitteilungen ohne Offenlegung verwendet
- GPAI-Modell zur Inhaltserzeugung in großem Umfang ohne Urheberrechts-Compliance genutzt

### Schritt 6: Compliance-Zeitplan, Konformitätsbewertung und Durchsetzung

Der AI Act gilt in Phasen. Bestimmen Sie, welche Fristen und Verfahren für das konkrete System und den Akteur gelten.

- **Verbotene Praktiken:** Durchsetzbar seit **2. Februar 2025**
- **KI-Modelle mit allgemeinem Verwendungszweck:** Pflichten seit **2. August 2025**
- **Hochrisiko-Systeme nach Anhang III:** Anforderungen ab **2. August 2026**
- **Produkte unter harmonisiertem Recht nach Anhang I:** Anforderungen ab **2. August 2027**
- **Konformitätsbewertung (Art. 43):** Für die meisten Hochrisiko-Systeme genügt eine Selbstbewertung (internes Kontrollverfahren, Anhang VI). Eine Drittbewertung durch eine benannte Stelle ist erforderlich für biometrische Identifizierungssysteme (Anhang III Nr. 1) und für Hochrisiko-Systeme, die Sicherheitskomponenten von Produkten sind, die nach Anhang I eine Drittbewertung erfordern.
- **EU-Konformitätserklärung (Art. 47):** Vom Anbieter schriftlich zu erstellen, aktuell zu halten und nationalen Behörden 10 Jahre zugänglich zu machen.
- **CE-Kennzeichnung (Art. 48):** Erforderlich für Hochrisiko-Systeme, sichtbar und lesbar am System oder seiner Verpackung anzubringen.
- **EU-Datenbankregistrierung (Art. 49):** Hochrisiko-Systeme müssen vor dem Inverkehrbringen in der EU-Datenbank registriert werden.

**Durchsetzung und Sanktionen (Art. 99):**

| Verstoß | Höchststrafe |
|---|---|
| Verbotene Praktiken (Art. 5) | 35 Mio. EUR oder 7 % des weltweiten Jahresumsatzes |
| Anforderungen an Hochrisiko-Systeme | 15 Mio. EUR oder 3 % des weltweiten Jahresumsatzes |
| Falsche Angaben gegenüber Behörden | 7,5 Mio. EUR oder 1 % des weltweiten Jahresumsatzes |

KMU und Start-ups profitieren von verhältnismäßigen Obergrenzen (Art. 99 Abs. 6). Nationale Marktüberwachungsbehörden setzen die Verordnung durch, koordiniert durch das AI Office.

**Risikokennzeichnung:**
- Frist für anwendbare Pflichten bereits abgelaufen ohne Compliance-Maßnahmen
- Kein Konformitätsbewertungsverfahren identifiziert oder eingeleitet
- CE-Kennzeichnung erforderlich, aber nicht angebracht
- System nicht in der EU-Datenbank registriert
- Keine zuständige nationale Aufsichtsbehörde identifiziert


## Besondere Szenarien

### KI im Personalwesen und bei der Einstellung

KI-Systeme für Einstellung, Bewerberscreening, Beförderungsentscheidungen, Aufgabenzuweisung oder Leistungsüberwachung fallen unter **Anhang III Nr. 4** (Beschäftigung). Dies ist eine der häufigsten Hochrisiko-Kategorien für betreibende Unternehmen.

- **Betreiber-FRIA** erforderlich nach Art. 27 vor dem Einsatz
- **Mitbestimmung des Betriebsrats** nach **§ 87 Abs. 1 Nr. 6 BetrVG** (Überwachung des Arbeitnehmerverhaltens durch technische Einrichtungen) greift in Deutschland und schafft ein paralleles Zustimmungserfordernis
- **Antidiskriminierungsrecht:** Algorithmische Verzerrungen können Haftung nach dem **AGG** begründen, wenn geschützte Merkmale direkt oder indirekt in die Entscheidungsfindung einfließen
- **Arbeitnehmerinformation:** Arbeitnehmer müssen informiert werden, dass sie einem Hochrisiko-KI-System unterliegen (Art. 26 Abs. 7)

### KI in Finanzdienstleistungen

KI in der Kreditbewertung, Versicherungszeichnung und Betrugserkennung kann als Hochrisiko-System unter **Anhang III Nr. 5** (wesentliche Dienstleistungen) eingestuft werden und unterliegt zudem sektorspezifischer Regulierung.

- **MiFID-II-Geeignetheitsanforderungen** für KI-gestützte Anlageberatung
- **DORA** (Digital Operational Resilience Act) für IKT-Risikomanagement bei KI in Finanzinstituten
- **EZB/BaFin-Erwartungen** an Modell-Risikomanagement und Erklärbarkeit
- **DSGVO Art. 22:** Automatisierte Einzelentscheidungen einschließlich Profiling -- Betroffene haben das Recht, keiner ausschließlich auf automatisierter Verarbeitung beruhenden Entscheidung unterworfen zu werden

### Zusammenspiel DSGVO und AI Act

Beide Verordnungen gelten kumulativ. Wesentliche Überschneidungsbereiche:

- **Datenminimierung (Art. 5 Abs. 1 lit. c DSGVO)** vs. Datenqualitäts- und Repräsentativitätsanforderungen (Art. 10 AI Act) -- diese können in Spannung zueinander stehen
- **DSFA (Art. 35 DSGVO)** und **FRIA (Art. 27 AI Act)** sind getrennte Anforderungen, die ggf. parallel durchzuführen sind
- **Rechtsgrundlage für Trainingsdaten:** DSGVO Art. 6 gilt für alle personenbezogenen Daten in Trainingsdatensätzen; bei berechtigtem Interesse (Art. 6 Abs. 1 lit. f) ist eine Abwägung erforderlich
- **Art. 10 Abs. 5 AI Act** schafft eine enge Ausnahme für die Verarbeitung besonderer Kategorien personenbezogener Daten zur Bias-Erkennung unter strengen Auflagen


## Grenzen dieses Skills

Dieser Skill bietet eine strukturierte Erstbewertung. In folgenden Fällen ist die Einschaltung eines Rechtsanwalts erforderlich:

- **Konformitätsbewertungsverfahren** und Erstellung technischer Dokumentation für die Prüfung durch benannte Stellen
- **Sektorspezifisches Zusammenspiel** zwischen AI Act und Finanzregulierung (MiFID II, DORA), Medizinprodukterecht (MDR) oder Arbeitsrecht (BetrVG, AGG)
- **Grenzüberschreitender Einsatz** mit unterschiedlichen nationalen Umsetzungsmaßnahmen in verschiedenen EU-Mitgliedstaaten
- **GPAI-Modell-Anbieter** mit Einstufung als systemisches Risiko und den damit verbundenen Pflichten
- **Aufsichtsverfahren** oder Marktüberwachungsanfragen nationaler Behörden oder des AI Office
- **Vertragliche Zuordnung** der AI-Act-Pflichten zwischen Anbietern, Betreibern und Händlern in komplexen Lieferketten

Compound unterstützt gerne bei AI-Act-Compliance-Bewertungen, Risikoklassifizierungen und der Erstellung von Konformitätsdokumentation.
