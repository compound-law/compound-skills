---
name: hinweisgebersystem
description: 'Hinweisgebersystem gesetzeskonform einrichten: Meldekanäle, Fristen und Dokumentation nach HinSchG und EU-Richtlinie 2019/1937 — für Unternehmen ab 50 Beschäftigten.'
---


## Überblick

Dieser Skill leitet die Implementierung und Prüfung interner Hinweisgebersysteme nach dem **Hinweisgeberschutzgesetz (HinSchG)** an, das die **EU-Richtlinie 2019/1937** umsetzt. Das HinSchG, in Kraft seit dem 2. Juli 2023, verpflichtet Unternehmen zur Einrichtung interner Meldekanäle, über die Beschäftigte und andere Personen Verstöße gegen bestimmte Rechtsvorschriften melden können. Zentrale Vorschriften sind **§ 12** (Pflicht zur Einrichtung interner Meldekanäle), **§ 16** (Anforderungen an den internen Meldekanal), **§ 15** (Bestellung zuständiger Personen), **§ 8** (Vertraulichkeit), **§ 36** (Verbot von Repressalien) und **§ 40** (Bußgeldvorschriften). Dieser Skill ist anzuwenden bei der Einrichtung eines neuen Hinweisgebersystems, bei der Compliance-Prüfung eines bestehenden Systems oder bei der Beratung zur Bearbeitung einer konkreten Meldung.

Das HinSchG erfasst einen breiten Anwendungsbereich melderelevanter Verstöße, darunter Verletzungen von EU-Recht, Straftaten, bestimmte Ordnungswidrigkeiten und sektorspezifische Vorschriften. Unternehmen, die keinen konformen Meldekanal einrichten, drohen Bußgelder bis zu 20.000 EUR (§ 40 Abs. 1 HinSchG), während Behinderung der Meldung oder Repressalien gegen Hinweisgeber mit Bußgeldern bis zu 50.000 EUR geahndet werden können (§ 40 Abs. 2, 6 HinSchG). Über Bußgelder hinaus birgt die Nichtbeachtung erhebliches Reputationsrisiko und kann dazu führen, dass Hinweisgeber sich direkt an externe Behörden oder die Medien wenden.

Das Hinweisgebersystem verarbeitet personenbezogene Daten von Hinweisgebern und Beschuldigten und löst damit [Auftragsverarbeitungsvertrag-Pflichten](/de-DE/skills/auftragsverarbeitung/) für externe Plattformanbieter aus. Ein Beschäftigter, gegen den nach einer Meldung Maßnahmen ergriffen werden, kann Kündigungsschutz beanspruchen — die Prüfcheckliste liefert der Skill [Kündigungsprüfung](/de-DE/skills/kuendigungspruefung/). DSGVO-Auskunftsanfragen in Bezug auf Hinweisgeberfallakten unterliegen besonderen Beschränkungen — die einschlägigen Ausnahmen beschreibt der Skill [DSGVO-Auskunftsanfrage](/de-DE/skills/dsgvo-auskunft/).


## Systematische Prüfung

### Schritt 1: Verpflichtungsumfang und Anwendbarkeit (§ 12 HinSchG)

Stellen Sie fest, ob das Unternehmen zur Einrichtung eines internen Meldekanals verpflichtet ist und welche Frist gilt.

- **Beschäftigtenschwelle (§ 12 Abs. 1 HinSchG):** Unternehmen mit **50 oder mehr Beschäftigten** müssen einen internen Meldekanal einrichten. Die Zählung umfasst alle Beschäftigten unabhängig von der Vertragsart -- Vollzeit, Teilzeit, geringfügig Beschäftigte, Leiharbeitnehmer und entsandte Beschäftigte. Auch Auszubildende werden gezählt. Maßgeblich ist die regelmäßige Belegschaft, nicht eine Stichtagsbetrachtung.
- **Compliance-Fristen:** Unternehmen mit **250+ Beschäftigten** seit dem 2. Juli 2023; Unternehmen mit **50-249 Beschäftigten** seit dem 17. Dezember 2023. Beide Fristen sind abgelaufen. Unternehmen ohne konformen Kanal befinden sich im Verstoß und sind bußgeldbewehrt.
- **Regulierte Sektoren (§ 12 Abs. 3 HinSchG):** Finanzdienstleistungsunternehmen (Kreditinstitute, Versicherungsunternehmen, Wertpapierfirmen, Zahlungsdienstleister) müssen **unabhängig von der Beschäftigtenzahl** einen Meldekanal einrichten. Dies erfasst auch kleine Fintech-Unternehmen und Versicherungsmakler unter 50 Beschäftigten.
- **Öffentlicher Sektor:** Kommunen, Behörden und andere öffentliche Einrichtungen mit 50+ Beschäftigten sind gleichermaßen verpflichtet.
- **Ressourcenteilung (§ 14 Abs. 2 HinSchG):** Unternehmen mit 50-249 Beschäftigten können Meldekanal-Ressourcen -- einschließlich der zuständigen Person und der technischen Infrastruktur -- mit anderen Unternehmen teilen. Unternehmen ab 250 Beschäftigten dürfen den Kanal nicht teilen.
- **Konzernstrukturen:** Jede rechtlich selbständige Einheit mit 50+ Beschäftigten muss einen eigenen Meldekanal unterhalten. Der Kanal der Muttergesellschaft erfüllt nicht automatisch die Pflicht der Tochtergesellschaften, obwohl die Infrastruktur (z. B. gemeinsame digitale Plattform) genutzt werden darf, sofern jede Einheit eine eigene zuständige Person hat und die Bearbeitung getrennt erfolgt.

**Risikokennzeichnung:**
- Unternehmen überschreitet die 50-Beschäftigten-Schwelle, hat aber keinen Meldekanal eingerichtet
- Beschäftigtenzahl berücksichtigt Leiharbeitnehmer, geringfügig Beschäftigte oder entsandte Arbeitnehmer nicht
- Compliance-Frist bereits abgelaufen ohne Umsetzung
- Finanzdienstleistungsunternehmen unter 50 Beschäftigten geht von Befreiung aus
- Konzern nutzt einen einzigen Kanal für alle Tochtergesellschaften ohne einheitenbezogene Bearbeitung

### Schritt 2: Einrichtung des internen Meldekanals (§ 16 HinSchG)

Der Kanal muss Meldungen in mehreren Formaten ermöglichen und die Vertraulichkeit der Identität der hinweisgebenden Person schützen.

- **Meldeformate (§ 16 Abs. 3 HinSchG):** Der Kanal muss Meldungen in drei Formaten annehmen: **(a) in Textform** -- dedizierte E-Mail-Adresse, webbasierte Meldeplattform oder physischer Briefkasten; **(b) mündlich** -- Telefonhotline, Sprachnachrichtensystem oder Anrufbeantworter; und **(c) persönlich** -- eine persönliche Zusammenkunft auf Verlangen der hinweisgebenden Person. Alle drei Formate müssen verfügbar sein; ein System, das nur Textmeldungen annimmt, ist nicht konform.
- **Vertraulichkeit durch Design (§ 16 Abs. 2 HinSchG):** Das System muss so gestaltet sein, dass die Identität der hinweisgebenden Person, der in der Meldung genannten Personen und aller Dritter geschützt wird. Dies erfordert: Ende-zu-Ende-Verschlüsselung für digitale Plattformen, Zugangsbeschränkungen (nur die zuständigen Personen dürfen auf Meldungen zugreifen), sichere Aufbewahrung und Trennung von allgemeinen HR- oder Compliance-Fallmanagementsystemen.
- **Zugänglichkeit (§ 16 Abs. 1 HinSchG):** Der Kanal muss allen Beschäftigten zugänglich sein. Zusätzlich sollte der Zugang, wo angemessen, auf Leiharbeitnehmer, Gesellschafter, Organmitglieder, Freiwillige, Lieferanten, Auftragnehmer und ehemalige Beschäftigte erstreckt werden. Best Practice: Kanal über die Unternehmenswebsite zugänglich machen (nicht hinter einem Login).
- **Sprache:** Der Kanal sollte in den Sprachen der Belegschaft verfügbar sein. Für internationale Unternehmen mit deutschem Betrieb ist Deutsch plus Englisch in der Regel das Minimum.
- **Auslagerung (§ 14 Abs. 1 HinSchG):** Der Betrieb des Kanals kann an Dritte ausgelagert werden -- typischerweise an eine externe Ombudsperson (häufig ein Rechtsanwalt) oder einen spezialisierten Plattformanbieter. Die Auslagerung entbindet das Unternehmen nicht von seinen Compliance-Pflichten.
- **Anonyme Meldungen (§ 16 Abs. 1 S. 5 HinSchG):** Das HinSchG verpflichtet nicht zur Annahme anonymer Meldungen, bestimmt aber, dass interne Meldekanäle anonyme Meldungen ermöglichen **sollen**. In der Praxis erhöht die Ermöglichung anonymer Meldungen das Meldeaufkommen erheblich. Der externe Meldekanal des Bundesamts für Justiz (BfJ) nimmt anonyme Meldungen an.

**Risikokennzeichnung:**
- Kanal nimmt nur Textmeldungen an, nicht mündlich oder persönlich
- Keine Vertraulichkeitsschutzmaßnahmen im Systemdesign -- Meldungen für Personen außerhalb des zuständigen Teams zugänglich
- Kanal nicht für externe Melder (Lieferanten, Auftragnehmer, ehemalige Beschäftigte) zugänglich, wo erforderlich
- Keine anonyme Meldemöglichkeit trotz der gesetzlichen "Soll"-Empfehlung
- Ausgelagerter Kanalbetreiber verfügt nicht über die nach § 15 HinSchG erforderliche Fachkunde oder Unabhängigkeit

### Schritt 3: Bestellung zuständiger Personen (§ 15 HinSchG)

Das Unternehmen muss qualifizierte, unabhängige Personen benennen, die Meldungen entgegennehmen, prüfen und Folgemaßnahmen ergreifen.

- **Bestellung (§ 15 Abs. 1 HinSchG):** Eine oder mehrere natürliche Personen oder eine Organisationseinheit (z. B. Compliance-Abteilung) müssen als zuständig für den Kanalbetrieb und die Folgemaßnahmen benannt werden.
- **Unabhängigkeit und Freiheit von Interessenkonflikten:** Zuständige Personen müssen weisungsfrei in Bezug auf die unparteiische Bearbeitung von Meldungen sein. Die zuständige Person sollte nicht der Person unterstellt sein, die am ehesten Gegenstand von Meldungen ist. Strukturelle Absicherungen umfassen: Berichtsweg direkt an den Aufsichtsrat oder einen unabhängigen Compliance-Beauftragten, Trennung von der Personalabteilung und dokumentierte Befangenheitsregelungen.
- **Fachkunde (§ 15 Abs. 2 HinSchG):** Das HinSchG verlangt fachliche Sachkunde im Umgang mit Meldungen und im einschlägigen Rechtsrahmen. Dies umfasst: Kenntnis des sachlichen Anwendungsbereichs des HinSchG, Verfahrensanforderungen (Fristen, Dokumentation), Vertraulichkeitspflichten und Repressalienverbot. Regelmäßige Fortbildung ist unerlässlich -- mindestens jährlich.
- **Externe Ombudsperson:** Die Beauftragung eines Rechtsanwalts als externe Ombudsperson ist eine gängige und wirksame Lösung, insbesondere für KMU. Das anwaltliche Berufsgeheimnis (**§ 203 StGB**) bietet eine zusätzliche Vertraulichkeitsebene. Das Unternehmen bleibt jedoch für die Compliance verantwortlich.
- **Sonderkündigungsschutz (§ 15 Abs. 3 HinSchG):** Interne zuständige Personen genießen während ihrer Bestellung und für einen angemessenen Zeitraum danach besonderen Kündigungsschutz, vergleichbar dem von Betriebsratsmitgliedern.

**Risikokennzeichnung:**
- Zuständige Person ist der Person unterstellt, die am ehesten Gegenstand von Meldungen ist (z. B. Geschäftsführer ohne Aufsichtsratsüberwachung)
- Keine dokumentierte Schulung oder Qualifikation der zuständigen Personen
- Interessenkonflikt nicht adressiert (z. B. Personalleiterin zuständig für den Kanal und gleichzeitig für Arbeitsrechtsstreitigkeiten mit potenziellen Hinweisgebern)
- Externe Ombudsperson ohne Spezialisierung auf Compliance- oder Hinweisgeberschutzrecht
- Keine Stellvertretung für Abwesenheiten (Urlaub, Krankheit), sodass Meldungen unbearbeitet bleiben

### Schritt 4: Bearbeitungsfristen und Folgemaßnahmen (§ 17 HinSchG)

Strikte Fristen bestimmen die Bearbeitung von Meldungen. Die Nichteinhaltung ist selbst ein Verstoß, der Bußgelder auslösen und den Hinweisgeber zur Eskalation an externe Kanäle veranlassen kann.

- **Eingangsbestätigung (§ 17 Abs. 1 S. 2 HinSchG):** Die zuständige Person muss dem Hinweisgeber den Eingang der Meldung **innerhalb von sieben Tagen** bestätigen. Die Bestätigung sollte den Erhalt bestätigen und darauf hinweisen, dass die Meldung geprüft wird, ohne Einzelheiten einer Untersuchung preiszugeben.
- **Prüfung des sachlichen Anwendungsbereichs (§§ 2, 3 HinSchG):** Stellen Sie fest, ob die gemeldeten Informationen in den sachlichen Anwendungsbereich des HinSchG fallen. Das Gesetz erfasst: **(a)** Verstöße gegen EU-Rechtsakte in bestimmten Bereichen (öffentliches Auftragswesen, Finanzdienstleistungen, Produktsicherheit, Transportsicherheit, Umweltschutz, Lebensmittelsicherheit, Gesundheitsschutz, Verbraucherschutz, Datenschutz, Wettbewerb), **(b)** Straftaten nach deutschem Recht, **(c)** bestimmte Ordnungswidrigkeiten, deren verletzte Norm den Schutz von Leben, Leib oder Gesundheit oder die Rechte der Beschäftigten oder ihrer Vertretungsorgane bezweckt, und **(d)** sektorspezifische Vorschriften für Finanzdienstleistungen.
- **Folgemaßnahmen (§ 18 HinSchG):** Angemessene Folgemaßnahmen können umfassen: interne Untersuchung, Weiterleitung an eine zuständige externe Behörde oder Einstellung des Verfahrens mangels hinreichender Anhaltspunkte. Die Wahl der Maßnahme muss verhältnismäßig und dokumentiert sein.
- **Rückmeldung an den Hinweisgeber (§ 17 Abs. 2 HinSchG):** Innerhalb von **drei Monaten** nach Eingangsbestätigung muss der Hinweisgeber eine Rückmeldung über die ergriffenen oder geplanten Folgemaßnahmen erhalten. Die Rückmeldung muss nicht das vollständige Untersuchungsergebnis offenlegen, aber aussagekräftige Informationen über die ergriffenen Maßnahmen enthalten.
- **Dokumentation:** Jeder Schritt muss zum Nachweis der Verfahrens-Compliance dokumentiert werden. Die Dokumentation umfasst: Datum der Meldung, inhaltliche Zusammenfassung, Prüfung des Anwendungsbereichs, ergriffene Folgemaßnahmen, eingehaltene Fristen und erteilte Rückmeldung. Meldungen und Dokumentation sind drei Jahre nach Abschluss des Verfahrens aufzubewahren (§ 11 Abs. 5 HinSchG).

**Risikokennzeichnung:**
- Keine Eingangsbestätigung innerhalb von sieben Tagen
- Keine dokumentierte Prüfung, ob die Meldung in den Anwendungsbereich des HinSchG fällt
- Dreimonatsfrist für Rückmeldung ohne dokumentierte Begründung versäumt
- Folgemaßnahmen nicht dokumentiert, sodass Verfahrenskonformität nicht nachweisbar
- Dokumentation länger als drei Jahre ohne Begründung aufbewahrt, was Datenminimierungsbedenken aufwirft

### Schritt 5: Vertraulichkeitsschutz (§ 8 HinSchG)

Die Vertraulichkeit der Identität der hinweisgebenden Person ist ein Eckpfeiler des HinSchG. Ein Verstoß gegen die Vertraulichkeit ist eine bußgeldbewehrte Ordnungswidrigkeit.

- **Zugangsbeschränkung (§ 8 Abs. 1 HinSchG):** Die Identität der hinweisgebenden Person darf nur den zuständigen Personen und denjenigen offengelegt werden, die diese für den Empfang und die Bearbeitung der Meldungen benötigen. Allgemeine Offenlegung an Geschäftsführung, Personalabteilung oder Rechtsabteilung ist unzulässig, sofern diese nicht Teil des zuständigen Teams sind.
- **Offenlegung gegenüber der beschuldigten Person:** Die Identität des Hinweisgebers darf der beschuldigten Person **nicht** offengelegt werden, es sei denn: (a) die Offenlegung ist für Straf- oder Disziplinarverfahren erforderlich, (b) der Hinweisgeber hat ausdrücklich eingewilligt oder (c) die Offenlegung ist gesetzlich vorgeschrieben (z. B. Gerichtsbeschluss).
- **Offenlegung an Dritte (§ 9 HinSchG):** Über die beschuldigte Person hinaus ist eine Offenlegung an Dritte nur zulässig, wenn sie für Folgemaßnahmen unerlässlich und verhältnismäßig ist.
- **Technische Absicherungen:** Zugangskontrollen (rollenbasierter Zugang, Zwei-Faktor-Authentifizierung), Need-to-know-Grundsatz, verschlüsselte Aufbewahrung von Meldeunterlagen, Protokollierung der Zugriffe und physische Sicherheit für Papiermeldungen. Die Meldeplattform sollte von allgemeinen IT-Systemen getrennt sein.
- **Bußgeld bei Verstoß (§ 40 Abs. 4 HinSchG):** Verletzung der Vertraulichkeitspflichten ist eine bußgeldbewehrte Ordnungswidrigkeit. Das Bußgeld kann gegen die verstoßende natürliche Person und über § 30 OWiG auch gegen das Unternehmen verhängt werden.

**Risikokennzeichnung:**
- Meldeunterlagen für Personen außerhalb des zuständigen Teams zugänglich
- Identität des Hinweisgebers ohne Rechtsgrundlage der beschuldigten Person offengelegt
- Keine technischen Zugangskontrollen auf der Meldeplattform -- Meldungen in gemeinsamen Ordnern oder allgemeinen Compliance-Datenbanken gespeichert
- Papiermeldungen in unverschlossenen oder gemeinsamen Ablageorten aufbewahrt
- Kein Zugriffsprotokoll, wer auf welche Meldungen zugegriffen hat

### Schritt 6: Repressalienverbot (§ 36 HinSchG)

Das Verbot von Repressalien ist der bedeutendste Schutz des HinSchG. Es umfasst eine **Beweislastumkehr**, die das Prozessrisiko auf den Arbeitgeber verlagert.

- **Verbotene Repressalien (§ 36 Abs. 1 HinSchG):** Das HinSchG enthält eine nicht abschließende Liste: Kündigung, Suspendierung, Herabstufung, Verweigerung einer Beförderung, Versetzung, Gehaltskürzung, Änderung der Arbeitszeit, Vorenthaltung von Fortbildung, negative Leistungsbewertungen, Verhängung von Disziplinarmaßnahmen, Nötigung, Einschüchterung, Belästigung, Ausgrenzung, Diskriminierung und Aufnahme auf eine schwarze Liste.
- **Beweislastumkehr (§ 36 Abs. 2 HinSchG):** Erleidet ein Hinweisgeber nach einer Meldung einen Nachteil, wird **vermutet**, dass es sich um eine Repressalie handelt. Der Arbeitgeber muss dann beweisen, dass die Maßnahme auf hinreichend gerechtfertigten, von der Meldung unabhängigen Gründen beruht. Dies ist ein hoher Standard -- allein die zeitliche Nähe zwischen Meldung und nachteiliger Maßnahme begründet eine starke Vermutung. Der Arbeitgeber muss urkundliche Nachweise der unabhängigen Begründung vorlegen.
- **Schadensersatz und Entschädigung (§ 37 HinSchG):** Hinweisgeber, die Repressalien erleiden, haben Anspruch auf vollständigen Ersatz aller materiellen und immateriellen Schäden, einschließlich entgangenem Lohn, verlorenen Karrieremöglichkeiten und Entschädigung für psychische Belastung.
- **Erstreckung des Schutzes:** Der Repressalienschutz erstreckt sich nicht nur auf den Hinweisgeber, sondern auch auf Personen, die den Hinweisgeber unterstützen, und auf mit dem Hinweisgeber verbundene Personen (§ 34 HinSchG) -- einschließlich Kollegen, Familienangehörige und Rechtsberater.
- **Schulung der Führungskräfte:** Alle Führungskräfte, Vorgesetzten, Personalverantwortlichen und Compliance-Beauftragten müssen zum Repressalienverbot geschult werden. Die Schulung sollte umfassen: Was eine Repressalie darstellt, die Beweislastumkehr, Dokumentationspflichten für Personalmaßnahmen, die bekannte Hinweisgeber betreffen, und das persönliche Haftungsrisiko.

**Risikokennzeichnung:**
- Kein Repressalienverbot gegenüber Führungskräften und Personalabteilung kommuniziert
- Personalmaßnahme gegen einen Hinweisgeber ohne dokumentierte, von der Meldung unabhängige Begründung
- Keine Schulung der Führungskräfte zu HinSchG-Pflichten
- Identität des Hinweisgebers dem direkten Vorgesetzten bekannt, der anschließend nachteilige Maßnahmen einleitet
- Unternehmen verlässt sich auf informelle Zusicherungen statt dokumentierter Richtlinien und Verfahren


## Risikobewertung

### Häufige Compliance-Lücken

| Lücke | Bußgeldrisiko | Empfohlene Maßnahme |
|---|---|---|
| Kein interner Meldekanal | 20.000 EUR (§ 40 Abs. 1) | Kanal unverzüglich einrichten |
| Kanal nur für Textmeldungen | Nichtkonformität mit § 16 Abs. 3 | Mündliche und persönliche Meldemöglichkeit ergänzen |
| Keine zuständige Person bestellt | Nichtkonformität mit § 15 | Zuständige Person benennen und schulen |
| Keine anonyme Meldemöglichkeit | Best-Practice-Lücke (kein Bußgeld, aber erhöhtes Risiko externer Meldungen) | Anonyme Meldungen ermöglichen |
| Eingangsbestätigung nicht innerhalb von 7 Tagen | Verfahrensverstoß | Automatisierte Bestätigung in der Plattform einrichten |
| Rückmeldung nicht innerhalb von 3 Monaten | Verfahrensverstoß | Kalendererinnerungen und Workflow-Trigger setzen |
| Vertraulichkeitsverstoß | Bußgeld (§ 40 Abs. 4) + Schadensersatz (§ 37) | Technische Zugangskontrollen und Zugriffsprotokolle |
| Repressalie gegen Hinweisgeber | 50.000 EUR (§ 40 Abs. 6) + Schadensersatz (§ 37) | Führungskräfteschulung, Dokumentation aller Personalmaßnahmen |


## Besondere Szenarien

### Zusammenspiel mit Datenschutz (DSGVO / BDSG)

Hinweisgebersysteme verarbeiten personenbezogene Daten des Hinweisgebers, der beschuldigten Person und von Zeugen. Dies löst DSGVO-Pflichten aus:

- **Rechtsgrundlage:** Typischerweise Art. 6 Abs. 1 lit. c DSGVO (rechtliche Verpflichtung) für Unternehmen, die § 12 HinSchG unterliegen. Für Unternehmen unterhalb der Schwelle, die freiwillig einen Kanal einrichten, kann Art. 6 Abs. 1 lit. f (berechtigtes Interesse) greifen.
- **Datenschutz-Folgenabschätzung (Art. 35 DSGVO):** Eine DSFA ist angesichts der sensiblen Natur der Hinweisgeberdaten und der potenziell nachteiligen Auswirkungen auf die beschuldigte Person wahrscheinlich erforderlich.
- **Informationspflichten (Art. 13, 14 DSGVO):** Der Hinweisgeber muss über die Datenverarbeitung informiert werden. Für die beschuldigte Person kann die Information nach Art. 14 aufgeschoben werden, wenn sie die Untersuchung gefährden würde (Art. 14 Abs. 5 lit. b DSGVO), muss aber erteilt werden, sobald das Risiko entfällt.
- **Aufbewahrungsfristen (§ 11 Abs. 5 HinSchG):** Meldungsdokumentation ist drei Jahre nach Abschluss des Verfahrens zu löschen, sofern nicht eine längere Aufbewahrung für laufende Verfahren erforderlich ist.
- **Betriebsrat:** Die Einführung eines Hinweisgebersystems kann Mitbestimmungsrechte nach **§ 87 Abs. 1 Nr. 1 BetrVG** (Ordnung des Betriebs) und **§ 87 Abs. 1 Nr. 6 BetrVG** (technische Überwachungseinrichtungen) auslösen. Der Betriebsrat ist vor der Einführung zu beteiligen.

### Grenzüberschreitende Meldestrukturen

Multinationale Konzerne stehen vor der Herausforderung, das HinSchG mit Hinweisgeberschutzgesetzen anderer EU-Mitgliedstaaten und Nicht-EU-Rechtsordnungen in Einklang zu bringen:

- **Ein Kanal je Einheit:** Das HinSchG erfordert für jede verpflichtete deutsche Einheit einen eigenen Kanal. Eine globale Ethik-Hotline kann als Infrastruktur dienen, aber die Bearbeitung muss auf Einheitenebene erfolgen.
- **Sprache:** Der deutsche Kanal muss in Deutsch verfügbar sein. Für internationale Belegschaften sind weitere Sprachen Best Practice.
- **Datenübermittlungen:** Werden Meldungen von einem zentralen Compliance-Team außerhalb Deutschlands bearbeitet, müssen Datenübermittlungsmechanismen (Art. 44-49 DSGVO) vorhanden sein.

### Meldungen gegen die Geschäftsleitung

Meldungen gegen Geschäftsführer, Vorstände oder die zuständige Person selbst erfordern besondere Verfahren:

- **Befangenheit:** Die zuständige Person muss sich selbst ablösen, wenn die Meldung sie oder eine Person betrifft, der sie unmittelbar unterstellt ist. Eine Stellvertretung oder externe Ombudsperson sollte solche Meldungen bearbeiten.
- **Eskalation an den Aufsichtsrat:** In Unternehmen mit Aufsichtsrat sollten Meldungen gegen Geschäftsführer an den Aufsichtsratsvorsitzenden oder einen bestimmten Aufsichtsratsausschuss eskaliert werden.
- **Externe Meldung:** Der Hinweisgeber behält stets das Recht, sich direkt an die externe Behörde (BfJ) zu wenden (§ 7 Abs. 1 HinSchG), ohne zuvor den internen Kanal nutzen zu müssen.


## Grenzen dieses Skills

Dieser Skill bietet einen strukturierten Implementierungs- und Prüfungsrahmen. In folgenden Fällen ist die Einschaltung eines Rechtsanwalts erforderlich:

- **Bearbeitung konkreter Meldungen** mit potenziellem Straftatenbezug, aufsichtsrechtlichen Verstößen oder komplexen Sachverhalten
- **Interne Untersuchungen**, die durch Hinweisgebermeldungen ausgelöst werden, einschließlich Zeugenvernehmungen, Dokumentensicherung und Privilegienmanagement
- **Repressalienklagen** von Hinweisgebern, insbesondere bei erheblichem Arbeitgeberrisiko durch die Beweislastumkehr
- **Grenzüberschreitende Hinweisgeberprogramme** mit Koordinierungsbedarf zwischen HinSchG, EU-Richtlinie-2019/1937-Umsetzungen in anderen Mitgliedstaaten und Nicht-EU-Hinweisgeberregelungen (z. B. SOX, Dodd-Frank)
- **Betriebsratsverhandlungen** zur Einführung und Ausgestaltung des Hinweisgebersystems
- **Sektorspezifische Anforderungen** für Finanzdienstleistungsinstitute mit zusätzlichen BaFin-Vorgaben

Compound unterstützt gerne bei der Konzeption, Implementierung und Prüfung von Hinweisgebersystemen, die den Anforderungen des HinSchG entsprechen.
