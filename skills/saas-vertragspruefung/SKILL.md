---
name: saas-vertragspruefung
description: 'Prüfrahmen für SaaS-Abonnementverträge. SLA-Zusagen, Dateneigentum, Haftungsobergrenzen und Ausstiegsklauseln.'
---


## Überblick

Dieser Skill bietet eine strukturierte Prüfung von Software-as-a-Service (SaaS)-Abonnementverträgen aus der Perspektive des Kunden nach deutschem und EU-Recht. SaaS-Verträge werden nach deutschem Recht rechtlich entweder als Mietverträge (§§ 535 ff. BGB) für Standard-SaaS oder als Werk-/Dienstverträge eingeordnet, je nach Leistungsstruktur -- der BGH hat keine abschließende Einordnung vorgenommen, und die herrschende Meinung behandelt Standard-SaaS als Miete von Softwarefunktionalität. Wesentliche Verbraucherschutz- und KMU-Schutzvorschriften greifen über die AGB-Kontrolle (**§§ 305-310 BGB**), insbesondere **§ 307** (unangemessene Benachteiligung), **§ 308** (Klauseln mit Wertungsmöglichkeit) und **§ 309** (strikte Verbote, einschließlich § 309 Nr. 7 zu Haftungsausschlüssen bei Personenschäden). Dieser Skill ist anzuwenden bei der Prüfung anbieterseitiger SaaS-Bedingungen für die Beschaffung, bei Nachverhandlung von Verlängerungsbedingungen oder bei der Bewertung von Datenschutz- und Ausstiegsrisiken.

SaaS-Verträge bergen besondere Risiken hinsichtlich Daten-Lock-in, einseitiger Leistungsänderungen, intransparenter Unterbeauftragung und Haftungsbegrenzungen, die dem Kunden keinen angemessenen Rechtsschutz bieten. Eine gründliche Prüfung muss kommerzielle Bedingungen neben Datenschutz-, geistigen Eigentums- und regulatorischen Compliance-Aspekten adressieren.


## Systematische Prüfung

### Schritt 1: Leistungsbeschreibung und SLA-Zusagen

Die Leistungsbeschreibung ist die Grundlage des gesamten Vertrags. Prüfen Sie, ob sie präzise genug ist, um die vertragliche Leistungspflicht zu begründen.

- **Funktionaler Umfang:** Der Vertrag muss die enthaltenen Features, Module und Funktionalitäten spezifizieren. Vage Beschreibungen wie "Zugang zur Plattform" sind unzureichend -- der Kunde muss wissen, wofür er bezahlt, und jede Funktionsreduzierung kann einen Mangel (Mangel) darstellen.
- **Nutzerlimits und Zugriffsmodell:** Klären Sie, ob das Abonnement auf benannten Nutzern, gleichzeitigen Nutzern oder unternehmensweitem Zugang basiert. Prüfen Sie, ob API-Zugang, Integrationen und Administratorkonten eingeschlossen sind.
- **Speicher- und Datenkontingente:** Prüfen Sie die enthaltenen Speichervolumina, Datenaufbewahrungsfristen und die Folgen einer Kontingentüberschreitung (automatisches Upgrade, Drosselung oder Datenlöschung).
- **SLA-Verfügbarkeitszusage:** Das SLA sollte einen spezifischen monatlichen Verfügbarkeitsprozentsatz definieren (Marktstandard: 99,5 % bis 99,9 %). Prüfen Sie folgende Details:
  - **Messmethodik:** Wie wird Ausfallzeit berechnet? Wird auf Applikations- oder nur auf Infrastrukturebene gemessen? Infrastrukturseitige Verfügbarkeit kann applikationsseitige Ausfälle verdecken, die den Dienst für den Kunden unbrauchbar machen.
  - **Ausnahmen:** Geplante Wartungsfenster, höhere Gewalt und Ausfälle Dritter werden typischerweise ausgenommen. Prüfen Sie, ob Wartungsfenster angemessen sind und die gesamte ausgenommene Zeit pro Monat begrenzt ist.
  - **Rechtsfolgen bei SLA-Verletzung:** Service-Credits sind die Standardmaßnahme -- typischerweise 5-10 % der monatlichen Vergütung je definierter Stufe der Nichtverfügbarkeit. Prüfen Sie, ob Credits automatisch oder nur auf Anfrage gewährt werden und ob eine Obergrenze für Credits besteht.
  - **Eskalation zur Kündigung:** Ab welchem Ausmaß dauerhaften Versagens kann der Kunde kündigen? Best Practice: Bei SLA-Verletzung in drei aufeinanderfolgenden Monaten oder vier Monaten in einem 12-Monats-Zeitraum sollte der Kunde ein außerordentliches Kündigungsrecht haben.
- **Verbindliche Zusage vs. Best Effort:** Bestätigen Sie, ob das SLA eine **vertragliche Zusage** (Anbieter haftet bei Verletzung) oder lediglich eine **Zielvereinbarung** oder **Best-Effort-Verpflichtung** (keine Haftung) darstellt. Ein als "Ziel" bezeichnetes SLA bietet keinen vertraglichen Schutz.

**Risikokennzeichnung:**
- Leistungsbeschreibung zu vage, um den vertraglichen Leistungsstandard zu begründen
- SLA definiert "Verfügbarkeit" nur auf Infrastrukturebene, verdeckt applikationsseitige Ausfälle
- SLA-Rechtsfolgen auf Service-Credits beschränkt ohne Kündigungsrecht bei dauerhaftem Versagen
- SLA als "Ziel" oder "Best Effort" statt als verbindliche Zusage bezeichnet
- Keine Begrenzung der Wartungsfenster, die dem Anbieter unbegrenzte Wartungszeit erlauben

### Schritt 2: Leistungsstandards und Support-Level

Über die reine Verfügbarkeit hinaus prüfen Sie, ob der Vertrag Leistungs- und Support-Zusagen enthält, die die praktische Nutzbarkeit des Dienstes sicherstellen.

- **Antwortzeiten:** Der Vertrag sollte maximale Antwortzeiten für die Plattform definieren (z. B. Seitenladezeiten, API-Antwortzeiten unter Normallast).
- **Support-Stufen und Reaktionszeiten:** Support sollte nach Schweregrad kategorisiert sein:

| Priorität | Beschreibung | Reaktionszeit | Lösungsziel |
|---|---|---|---|
| **P1 Kritisch** | Dienst komplett nicht verfügbar oder Kernfunktionalität ausgefallen | 1-4 Stunden | 8-24 Stunden |
| **P2 Hoch** | Wesentliche Funktion beeinträchtigt, Workaround verfügbar | 4-8 Stunden | 1-3 Werktage |
| **P3 Mittel** | Nicht-kritische Funktion beeinträchtigt | 1 Werktag | 5-10 Werktage |
| **P4 Niedrig** | Geringfügiges Problem oder Feature-Anfrage | 2-5 Werktage | Best Effort |

- **Support-Kanäle:** Prüfen Sie, ob Support per Telefon, E-Mail, Chat oder Ticketsystem verfügbar ist und zu welchen Zeiten (24/7 für P1 ist Standard bei Enterprise-SaaS).
- **Berichtspflichten:** Der Anbieter sollte monatliche Verfügbarkeitsberichte und Incident-Post-Mortem-Berichte bei wesentlichen Ausfällen liefern. Ohne Berichterstattung kann der Kunde die SLA-Einhaltung nicht überprüfen.
- **Mangel nach Mietrecht:** Nach den Grundsätzen des deutschen Mietrechts (§§ 535 ff. BGB) kann ein dauerhaftes Unterschreiten der vertraglichen Leistungsstandards einen Mangel darstellen, der zur **Mietminderung** (§ 536 BGB) oder, bei Erheblichkeit, zur **außerordentlichen Kündigung** (§ 543 BGB) berechtigt. Der SLA-Credit-Mechanismus schließt diese gesetzlichen Rechtsbehelfe nicht automatisch aus -- eine entsprechende Klausel muss an § 307 BGB gemessen werden.

**Risikokennzeichnung:**
- Keine Support-Reaktionszeitenzusagen
- P1-kritischer Support außerhalb der Geschäftszeiten nicht verfügbar
- Keine monatliche Verfügbarkeitsberichterstattung, die SLA-Überprüfung verhindert
- SLA-Credits schließen ausdrücklich weitere Ansprüche aus dem gesetzlichen Mängelrecht aus
- Kein Eskalationsverfahren für ungelöste Probleme

### Schritt 3: Datenhoheit, Portabilität und Löschungsrechte

Daten-Lock-in ist das strategisch gefährlichste Risiko bei SaaS-Verträgen. Stellen Sie sicher, dass der Kunde jederzeit die volle Kontrolle über seine Daten behält.

- **Datenhoheit des Kunden:** Der Vertrag muss klar feststellen, dass der Kunde das volle Eigentum an allen auf die Plattform hochgeladenen oder dort generierten Daten ("Kundendaten") behält. Der Anbieter sollte lediglich eine begrenzte, widerrufliche Lizenz zur Verarbeitung der Kundendaten zum alleinigen Zweck der Leistungserbringung erhalten.
- **Datennutzungsrechte des Anbieters:** Prüfen Sie jede Klausel, die dem Anbieter Rechte einräumt, Kundendaten zu aggregieren, anonymisieren oder für Produktverbesserung, Benchmarking, Analytik, maschinelles Lernen oder Marketing zu nutzen. Nach **DSGVO Art. 6** erfordert jede Verarbeitung über den primären Dienstzweck hinaus eine eigenständige Rechtsgrundlage.
- **Datenexport (Portabilität):** Der Kunde sollte alle Kundendaten jederzeit während der Vertragslaufzeit und für einen definierten Zeitraum nach Vertragsende (30-90 Tage sind Standard) in standardisierten, maschinenlesbaren Formaten (CSV, JSON, XML oder branchenspezifische Formate) exportieren können. Die Exportfunktion sollte als Selbstbedienungsfunktion ohne Zusatzkosten verfügbar sein.
- **Datenlöschung nach Vertragsende:** Der Anbieter muss alle Kundendaten innerhalb einer festgelegten Frist nach Vertragsende löschen (30 Tage sind üblich) und die Löschung **schriftlich bestätigen**. Prüfen Sie, ob die Löschungspflicht auch Backups und Disaster-Recovery-Kopien erfasst -- vollständige Löschung von Backups kann technisch unpraktikabel sein, in diesem Fall sollte der Vertrag eine maximale Aufbewahrungsfrist für Backup-Kopien (typischerweise 90-180 Tage) mit Zugangsbeschränkungen vorsehen.
- **Verschlüsselung:** Prüfen Sie, ob der Vertrag Verschlüsselung bei der Übertragung (TLS 1.2+) und im Ruhezustand (AES-256 oder gleichwertig) vorsieht. Bring-your-own-key (BYOK) oder Hold-your-own-key (HYOK)-Verschlüsselung gibt dem Kunden Kontrolle über die Verschlüsselungsschlüssel.

**Risikokennzeichnung:**
- Anbieter beansprucht Eigentum an oder umfassende Lizenz an Kundendaten
- Anbieter nutzt Kundendaten für KI-Training, Benchmarking oder Produktverbesserung ohne ausdrückliche Einwilligung
- Keine Datenexportfunktion oder Export nur in proprietären Formaten
- Keine Löschungspflicht oder keine schriftliche Löschbestätigung
- Löschungspflicht schließt Backup-Kopien ohne Aufbewahrungsfrist aus
- Keine Verschlüsselung im Ruhezustand oder bei der Übertragung für Kundendaten

### Schritt 4: Haftungsbegrenzungen und -ausschlüsse (§§ 305-310 BGB)

Das deutsche AGB-Recht setzt zwingende Grenzen für Haftungsausschlüsse in Allgemeinen Geschäftsbedingungen. SaaS-Anbieter treiben Haftungsobergrenzen häufig auf das Minimum -- der Kunde muss prüfen, ob die Obergrenzen angemessenen Schutz bieten.

- **Zwingende unbeschränkte Haftung:** Nach deutschem Recht können folgende Haftungskategorien in AGB **nicht ausgeschlossen oder begrenzt** werden:
  - **Personenschäden durch Fahrlässigkeit (§ 309 Nr. 7 lit. a BGB):** Jede Klausel, die die Haftung für Tod oder Körperverletzung durch Fahrlässigkeit ausschließt oder begrenzt, ist per se unwirksam.
  - **Grobe Fahrlässigkeit und Vorsatz (§ 309 Nr. 7 lit. b BGB):** Haftung für sonstige Schäden durch grobe Fahrlässigkeit oder vorsätzliches Handeln kann nicht ausgeschlossen werden.
  - **Produkthaftungsgesetz:** Strikte Haftung nach dem ProdHaftG kann vertraglich nicht ausgeschlossen werden.

- **Wesentliche Vertragspflichten (Kardinalpflichten):** Nach § 307 BGB kann die Haftung für die Verletzung wesentlicher Vertragspflichten -- Pflichten, deren Erfüllung für die ordnungsgemäße Vertragsdurchführung wesentlich ist und auf deren Einhaltung der Kunde regelmäßig vertrauen darf -- begrenzt werden, aber nur auf den **vertragstypisch vorhersehbaren Schaden**. Eine Obergrenze unterhalb dieses Niveaus ist unwirksam. Bei SaaS umfassen Kardinalpflichten: Bereitstellung des Dienstes gemäß der Leistungsbeschreibung, Wahrung der Datenintegrität und Einhaltung der Datenschutzpflichten.

- **Zulässige Haftungsklauselstruktur:**
  1. Haftung für Vorsatz und grobe Fahrlässigkeit: **unbeschränkt**
  2. Haftung für Verletzung wesentlicher Vertragspflichten bei leichter Fahrlässigkeit: begrenzt auf den **vertragstypisch vorhersehbaren Schaden** (häufig quantifiziert als 100 % der jährlichen Vergütung)
  3. Haftung für Personenschäden: **unbeschränkt**
  4. Haftung nach ProdHaftG: **unbeschränkt**
  5. Allgemeine Obergrenze für sonstige Ansprüche: üblicherweise 100 % der in den letzten 12 Monaten gezahlten Vergütung

- **Haftung für Datenverlust:** Klauseln, die die Haftung für Datenverlust verschuldensunabhängig ausschließen, sind problematisch. Der Anbieter sollte mindestens für die Wiederherstellung der Daten aus dem letzten Backup haften.
- **Mittelbare und Folgeschäden:** Viele SaaS-Verträge schließen "mittelbare, Folge-, Sonder- oder Begleitschäden" aus. Im deutschen Recht ist diese Unterscheidung unüblich und mehrdeutig -- das deutsche Schadensersatzkonzept differenziert nicht zwischen direkten und indirekten Schäden im Common-Law-Sinne. Ein pauschaler Ausschluss kann nach § 307 BGB unwirksam sein, wenn er die Haftung für vorhersehbare vertragstypische Schäden faktisch beseitigt.

**Risikokennzeichnung:**
- Pauschaler Haftungsausschluss ohne Differenzierung nach Verschuldensgrad ("Die Haftung ist im gesetzlich zulässigen Umfang ausgeschlossen")
- Obergrenze auf eine Monatsvergütung oder einen ähnlich geringen Betrag festgelegt
- Haftung für Datenverlust verschuldensunabhängig ausgeschlossen
- Mittelbare/Folgeschäden ohne Differenzierung nach Verschuldensgrad ausgeschlossen
- Kardinalpflichthaftung unterhalb des vertragstypisch vorhersehbaren Schadens gedeckelt
- Kein Ausschluss des Ausschlusses für Personenschäden, grobe Fahrlässigkeit oder Vorsatz

### Schritt 5: Automatische Verlängerung, Laufzeit und Preisänderungen

SaaS-Verträge sind auf wiederkehrende Einnahmen ausgelegt. Prüfen Sie, ob die Verlängerungs- und Preismechanismen ausgewogen sind.

- **Erstlaufzeit:** Übliche Spannen sind 12 Monate (Standard), 24 Monate oder 36 Monate (Enterprise). Längere Laufzeiten bieten typischerweise Mengenrabatte, reduzieren aber die Flexibilität.
- **Automatische Verlängerung:** Die meisten SaaS-Verträge verlängern sich automatisch, sofern der Kunde nicht rechtzeitig die Nichtverlängerung erklärt. Nach deutschem AGB-Recht (§ 307 BGB) sind automatische Verlängerungsklauseln in B2B-AGB zulässig, müssen aber verhältnismäßig sein. Verlängerungszeiträume über ein Jahr oder Kündigungsfristen unter drei Monaten können angreifbar sein. Bei B2C (§ 309 Nr. 9 BGB) darf die Erstlaufzeit zwei Jahre nicht überschreiten, und nach der Erstlaufzeit kann der Verbraucher jederzeit mit einer Frist von einem Monat kündigen (seit 01.03.2022).
- **Kündigungsfrist für Nichtverlängerung:** Prüfen Sie den genauen Stichtag (z. B. 90, 60 oder 30 Tage vor Ende der laufenden Laufzeit). Verpasst der Kunde die Frist, ist er für eine weitere Laufzeit gebunden.
- **Preiserhöhung bei Verlängerung:** Prüfen Sie, ob der Anbieter bei Verlängerung Preise erhöhen darf und unter welchen Bedingungen. Best Practice: Preiserhöhungen auf einen bestimmten Prozentsatz gedeckelt (z. B. VPI + 3 %) oder dem Kunden ein Kündigungsrecht bei Überschreitung eines Schwellenwerts eingeräumt. Unbegrenztes Ermessen bei Preiserhöhungen ist nach § 307 BGB problematisch.
- **Unterjährige Preisänderungen:** Prüfen Sie, ob sich der Anbieter das Recht vorbehält, Preise während einer laufenden Laufzeit zu ändern. Falls ja, sollte dem Kunden ein außerordentliches Kündigungsrecht zustehen.
- **Downgrade und Nutzungsreduzierung:** Prüfen Sie, ob der Kunde Nutzerzahl, Module oder Speicher während der Laufzeit oder erst bei Verlängerung reduzieren kann. "Ratchet"-Klauseln, die eine Reduzierung verhindern, binden den Kunden an den jemals höchsten Nutzungsumfang.

**Risikokennzeichnung:**
- Automatischer Verlängerungszeitraum übersteigt ein Jahr in B2B-AGB
- Kündigungsfrist für Nichtverlängerung unter drei Monaten (leicht zu versäumen)
- Unbegrenztes Ermessen bei Preiserhöhungen bei Verlängerung ohne Kündigungsrecht
- Unterjährige Preisänderungen zulässig ohne Kündigungsrecht des Kunden
- Ratchet-Klausel verhindert jede Umfangsreduzierung während oder am Ende der Laufzeit
- B2C-Bedingungen mit Erstlaufzeit über zwei Jahre oder automatischer Verlängerung über einen Monat

### Schritt 6: Ausstiegsregelungen, Migrationsunterstützung und AVV-Erfordernis

Das Vertragsende ist häufig der Zeitpunkt, an dem sich die gravierendsten Risiken materialisieren. Prüfen Sie, ob die Ausstiegsregelungen die Geschäftskontinuität des Kunden schützen.

- **Übergangsphase nach Vertragsende:** Der Vertrag sollte eine Übergangsphase vorsehen (60-180 Tage sind bei Enterprise-SaaS Standard), während der der Kunde Zugriff auf den Dienst und die Datenexportfunktionalität behält, entweder zum bestehenden Abonnementpreis oder zu einem definierten Übergangstarif.
- **Migrationsunterstützung:** Bei komplexen SaaS-Implementierungen sollte der Anbieter Migrationshilfe anbieten -- Datenmapping, API-Zugang für Migrationstools und technischen Support für den Übergang zu einem Ersatzdienst. Prüfen Sie die Kosten und ob sie gedeckelt sind.
- **Datenportabilität beim Ausstieg:** Bestätigen Sie, dass die Datenexportregelungen (Schritt 3) während der Übergangsphase gelten und dass alle Daten, einschließlich historischer Daten, Protokolle und Konfigurationen, exportiert werden können.
- **DSGVO Art. 28 AVV-Erfordernis:** Verarbeitet der SaaS-Anbieter personenbezogene Daten im Auftrag des Kunden, ist ein **Auftragsverarbeitungsvertrag (AVV)** nach Art. 28 DSGVO zwingend erforderlich. Der AVV sollte separat unter Verwendung des Data Processing Agreement Skills geprüft werden. Stellen Sie sicher, dass der SaaS-Hauptvertrag den AVV referenziert oder einbezieht und dass die Beendigung des SaaS-Vertrags die Löschungspflichten des AVV auslöst.
- **Insolvenz oder Diensteinstellung des Anbieters:** Bei geschäftskritischem SaaS sollte der Kunde Schutzregelungen verhandeln:
  - **Quellcode-Escrow:** Ein Dritter verwahrt den Quellcode, der bei auslösenden Ereignissen (Insolvenzantrag des Anbieters, dauerhafte wesentliche SLA-Verletzung, Diensteinstellung) an den Kunden freigegeben wird. Die Escrow-Vereinbarung sollte das Recht umfassen, den Code zu hosten und zu modifizieren.
  - **Daten-Escrow:** Getrennt vom Quellcode sollten die Kundendaten auch bei Ausfall der Anbieterinfrastruktur zugänglich sein.
  - **Eintrittsrechte:** Das Recht des Kunden oder eines beauftragten Dritten, den Betrieb des Dienstes auf der Anbieterinfrastruktur bei Anbieterausfall zu übernehmen.
- **Insolvenzbehandlung (§ 103 InsO):** Wird der Anbieter insolvent, kann der Insolvenzverwalter gegenseitige Verträge ablehnen. Die vertraglichen Ansprüche des Kunden auf Datenrückgabe werden zu einfachen Insolvenzforderungen, sofern die Daten nicht eindeutig Eigentum des Kunden sind. Dies macht vorinsolvenzliche Schutzmaßnahmen (Escrow, Datenexport) unverzichtbar.

**Risikokennzeichnung:**
- Keine Übergangsphase nach Vertragsende -- Zugang sofort gesperrt
- Keine Datenexportmöglichkeit oder Export nur in proprietären Formaten
- AVV fehlt oder ist nicht Art.-28-konform
- Kein Quellcode-Escrow oder Kontinuitätsregelungen bei geschäftskritischem SaaS
- Migrationsunterstützung nicht geregelt oder prohibitiv teuer
- Insolvenz des Anbieters nicht adressiert, Kunde mit einfachen Insolvenzforderungen auf Datenrückgabe


## Risikobewertung

### Risikomatrix für den Kunden

| Risiko | Auswirkung | Abhilfe |
|---|---|---|
| SLA unter 99,5 % ohne Rechtsfolge | Dienstunzuverlässigkeit ohne Rechtsschutz | Verbindliches SLA mit Credits und Kündigungsrecht verhandeln |
| Daten-Lock-in (proprietäre Formate) | Migration zu Alternativanbieter unmöglich | Standardformat-Export jederzeit verlangen |
| Haftungsobergrenze bei einer Monatsvergütung | Schäden übersteigen Obergrenze bei jedem ernsthaften Vorfall | Mindestens 100 % Jahresvergütung, unbeschränkt bei Datenschutzverstoß |
| Kein AVV oder nicht-konformer AVV | DSGVO-Verstoß und Bußgeldrisiko | Art.-28-konformen AVV vor Go-live verlangen |
| Automatische Verlängerung mit kurzer Frist | Ungewollte Verlängerung | Kündigungsfrist im Kalender eintragen; mindestens 90 Tage verhandeln |
| Einseitige Leistungsänderungen | Kernfunktionalität während der Laufzeit entfernt | Keine wesentliche Verschlechterung + Kündigungsrecht bei wesentlicher Änderung |
| Anbieterinsolvenz | Verlust des Zugangs zu Daten und Dienst | Quellcode-Escrow + Datenexport + Übergangsphase |
| Keine Löschbestätigung | Daten nach Vertragsende aufbewahrt | Schriftliche Bestätigung innerhalb von 30 Tagen verlangen |


## Besondere Szenarien

### Einseitige Leistungsänderungen

Eine der umstrittensten Klauseln in SaaS-Verträgen. Nach deutschem AGB-Recht (§ 308 Nr. 4 BGB bei B2C; § 307 BGB bei B2B) unterliegen einseitige Leistungsänderungsklauseln strenger Prüfung:

- **Zulässige Änderungen:** Die Änderung muss einem berechtigten Zweck dienen (Rechtskonformität, Sicherheitsupdate, technische Verbesserung), darf den Kerncharakter des Dienstes (Kernleistung) nicht verändern, und der Kunde muss angemessene Vorankündigung und ein Kündigungsrecht bei wesentlichen Änderungen erhalten.
- **Unzulässige Änderungen:** Eine Klausel, die dem Anbieter erlaubt, "den Dienst jederzeit aus beliebigem Grund zu ändern", ist unwirksam (BGH, III ZR 169/19). Ebenso das Entfernen von Features, die Teil der vereinbarten Leistungsbeschreibung waren, ohne gleichwertigen Ersatz.
- **Rechtsfolge für den Kunden:** Der Kunde sollte das Recht haben, innerhalb einer definierten Frist (30-60 Tage) nach Wirksamwerden einer wesentlichen Änderung ohne Vertragsstrafe zu kündigen.

### SaaS für regulierte Branchen

Finanzdienstleistungen, Gesundheitswesen und öffentlicher Sektor unterliegen zusätzlichen Anforderungen:

- **BaFin-Auslagerungsanforderungen (MaRisk AT 9):** Finanzinstitute müssen vor Auslagerung an einen SaaS-Anbieter eine Risikoanalyse durchführen, Audit- und Zugangsrechte für die BaFin vereinbaren und sicherstellen, dass der Dienst ohne Unterbrechung übertragen werden kann.
- **Gesundheitsdaten (§ 203 StGB):** SaaS-Anbieter, die dem Berufsgeheimnis unterliegende Daten (medizinisch, anwaltlich, steuerlich) verarbeiten, müssen formell befugt werden. Ein AVV allein genügt nicht -- eine gesonderte Einwilligung nach § 203 StGB ist erforderlich.
- **Öffentliche Beschaffung:** Cloud-Dienste müssen den BSI C5 Cloud-Sicherheitsstandard (oder gleichwertig) und die EVB-IT Cloud-Bedingungen der Bundesregierung einhalten.

### Open-Source-Komponenten

SaaS-Anbieter verwenden häufig Open-Source-Softwarekomponenten. Der Vertrag sollte:

- Gewährleisten, dass alle Open-Source-Nutzungen lizenzkonform sind
- Copyleft-lizenzierte Komponenten (GPL, AGPL) offenlegen, die Pflichten für den Kunden begründen können
- Den Kunden gegen Ansprüche Dritter aus der Open-Source-Nutzung des Anbieters freistellen


## Grenzen dieses Skills

Dieser Skill bietet eine strukturierte Erstbewertung. In folgenden Fällen ist die Einschaltung eines Rechtsanwalts erforderlich:

- **Verhandlung von Enterprise-SaaS-Verträgen** mit individuellen Bedingungen, insbesondere für kritische Infrastruktur oder regulierte Branchen
- **DSGVO-Compliance** einschließlich AVV-Prüfung, Transfer Impact Assessments und grenzüberschreitende Datenflussanalyse
- **Streitigkeiten über geistiges Eigentum** an Kundendaten, generierten Outputs oder KI-Training mit Kundendaten
- **Insolvenzschutzmaßnahmen** einschließlich Quellcode-Escrow-Vereinbarungen und Eintrittsrechte
- **Regulatorische Compliance** für Finanzdienstleistungen (MaRisk, DORA), Gesundheitswesen (§ 203 StGB) und öffentliche Beschaffung
- **Rechtsstreitigkeiten** aus SLA-Verletzungen, Datenverlust oder einseitiger Dienstbeendigung

Compound unterstützt gerne bei der Prüfung, Verhandlung und Strukturierung von SaaS-Verträgen, die die Interessen des Kunden nach deutschem und EU-Recht schützen.
