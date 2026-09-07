---
name: dsgvo-auskunft
description: 'DSGVO-Auskunftsanfragen fristgerecht beantworten: Art. 15-Pflichten, 30-Tage-Frist und Pflichtangaben rechtssicher umsetzen — für Unternehmen in Deutschland.'
---


## Überblick

Dieser Skill leitet durch die vollständige Bearbeitung von Auskunftsanfragen nach Art. 15 DSGVO (in Deutschland auch als "DSGVO-Auskunftsanfrage" oder "Betroffenenanfrage" bezeichnet). Er deckt den gesamten Prozess ab — vom Eingang der Anfrage bis zur fristgerechten, rechtssicheren Antwort — und berücksichtigt aktuelle Rechtsprechung des EuGH und der deutschen Gerichte.

**Rechtsgrundlagen:** Art. 15 DSGVO, Art. 12 DSGVO, BDSG §§ 29, 34.

**Risiko bei Fehlern:** Bußgelder bis 20 Mio. EUR oder 4 % des weltweiten Jahresumsatzes (Art. 83 Abs. 5 DSGVO) sowie Schadensersatzansprüche der Betroffenen (Art. 82 DSGVO).

Werden personenbezogene Daten an externe Auftragsverarbeiter weitergegeben, verpflichtet Art. 28 Abs. 3 lit. e DSGVO den Auftragsverarbeiter zur Unterstützung bei der Auskunftserteilung — die Grundlagen regelt der [Auftragsverarbeitungsvertrag (AVV)](/de-DE/skills/auftragsverarbeitung/). KI-Systeme mit automatisierten Entscheidungen nach Art. 22 DSGVO erzeugen zusätzliche Offenlegungspflichten — den Bewertungsrahmen liefert der [KI-Verordnung Compliance-Check](/de-DE/skills/ki-verordnung-compliance/). Hinweisgebersysteme begründen spezifische Ausnahmen vom Auskunftsanspruch — das HinSchG-Framework beschreibt der Skill [Hinweisgebersystem-Einrichtung](/de-DE/skills/hinweisgebersystem/).

## Prozess Schritt für Schritt

### Schritt 1: Eingang und Dokumentation

- Anfrage sofort dokumentieren: Eingangsdatum, Kanal (E-Mail, Post, Webformular, mündlich), Absender, Wortlaut.
- Art. 15-Anfragen haben keine Formvorschrift — auch mündliche, beiläufige oder unspezifische Anfragen wie "Welche Daten haben Sie über mich?" lösen die Pflicht aus.
- Eingangsdatum ist fristauslösend. Bei E-Mail gilt der Zeitpunkt des Eingangs auf dem Server, nicht der Kenntnisnahme.
- Zuständige Stelle intern sofort informieren (Datenschutzbeauftragter, Rechtsabteilung).
- Ticket oder Vorgang anlegen mit Fristüberwachung.

### Schritt 2: Identitätsprüfung

Die Identitätsprüfung muss **verhältnismäßig** sein (Art. 12 Abs. 6 DSGVO). Der BfDI stellt klar: Kein pauschales Verlangen einer Ausweiskopie (vgl. PAuswG § 20 Abs. 2 — kein allgemeines Recht, Ausweis zu kopieren).

**Nach Kanal differenzieren:**

| Anfrage-Kanal | Geeignete Verifizierung |
|---|---|
| Registrierter Kundenaccount | Login-Authentifizierung genügt |
| Bekannte geschäftliche E-Mail-Adresse | Bestätigungsmail an die bekannte Adresse |
| Unbekannte E-Mail-Adresse | Rückfrage mit Identifikationsmerkmalen (Kundennr., Vertragsnr., Geburtsdatum) |
| Postalisch | Abgleich mit Bestandsdaten, ggf. Rückschreiben an hinterlegte Adresse |
| Telefonisch | Sicherheitsfragen auf Basis vorhandener Daten |
| Über Anwalt | Schriftliche Vollmacht prüfen |

**Wichtig:** Die Frist läuft auch während der Identitätsprüfung weiter. Die Prüfung muss daher zügig erfolgen. Nur wenn begründete Zweifel an der Identität bestehen, darf die Bearbeitung bis zur Klärung zurückgestellt werden (Art. 12 Abs. 6 DSGVO). Die Frist läuft dann ab Identitätsbestätigung.

### Schritt 3: Fristen berechnen

- **Regelfrist:** 1 Monat ab Eingang der Anfrage (Art. 12 Abs. 3 DSGVO).
- **Fristverlängerung:** Um weitere 2 Monate möglich (max. 3 Monate insgesamt), wenn die Anfrage komplex ist oder viele Anfragen gleichzeitig eingehen.
- **Bei Verlängerung:** Der Betroffene muss innerhalb des ersten Monats über die Verlängerung und deren Gründe informiert werden.
- Fristberechnung nach §§ 187, 188 BGB: Eingang am 15. März bedeutet Fristablauf am 15. April (24:00 Uhr). Fällt das Ende auf einen Samstag, Sonntag oder Feiertag, verlängert sich die Frist bis zum nächsten Werktag (§ 193 BGB).

**Wann gilt eine Anfrage als "komplex"?**
- Datenverarbeitung in zahlreichen Systemen
- Umfangreiche Drittlandsübermittlungen
- Erheblicher Redaktionsbedarf (Rechte Dritter betroffen)
- Mehrere parallele Anfragen derselben Person

### Schritt 4: Datenerhebung

Das Verzeichnis von Verarbeitungstätigkeiten (Art. 30 DSGVO) dient als Checkliste. Folgende Systeme systematisch durchsuchen:

- **CRM-System** (Kundenstammdaten, Kommunikationshistorie, Notizen)
- **E-Mail-Systeme** (alle Postfächer, in denen Kommunikation mit der Person stattfand)
- **HR-/Personalsystem** (bei Mitarbeiteranfragen: Personalakte, Gehaltsabrechnung, Zeiterfassung, Krankmeldungen, Beurteilungen)
- **ERP-System** (Bestellungen, Rechnungen, Zahlungsverkehr)
- **Marketing-Tools** (Newsletter-Abonnements, Tracking-Daten, Consent-Datenbank)
- **Support-/Ticket-System** (Anfragen, Beschwerden, Gesprächsnotizen)
- **Webanalyse** (Nutzungsprofile, Cookies — soweit der Person zuordenbar)
- **Zugangs- und Logdaten** (Gebäudezutritt, IT-Zugriffsprotokolle)
- **Physische Akten** (Verträge, Korrespondenz, handschriftliche Notizen)
- **Auftragsverarbeiter** (Art. 28 DSGVO — Pflicht, auch dort verarbeitete Daten einzubeziehen)
- **Videoüberwachung / CCTV** (soweit Aufnahmen noch vorhanden und die Person identifizierbar ist)
- **Backup-/Archivsysteme** (siehe Schritt 5 zu Ausnahmen nach BDSG § 34)

**BGH VI ZR 576/19:** Interne Vermerke, Gesprächsnotizen und Aktennotizen über die Person sind personenbezogene Daten und grundsätzlich auskunftspflichtig.

### Schritt 5: Ausnahmen prüfen

Nicht alle gefundenen Daten müssen oder dürfen herausgegeben werden:

**Art. 15 Abs. 4 DSGVO — Rechte Dritter:**
Das Recht auf eine Kopie darf die Rechte und Freiheiten anderer Personen nicht beeinträchtigen. Daten Dritter sind zu schwärzen (aber nicht übermäßig — nur die personenbezogenen Daten des Dritten, nicht den gesamten Kontext).

**BDSG § 34 Abs. 1 — Unverhältnismäßiger Aufwand:**
- Daten in Backup- oder Archivsystemen, die nur noch aus technischen Gründen oder zu Aufbewahrungszwecken gespeichert werden und deren Herausgabe unverhältnismäßigen Aufwand erfordern würde.
- Diese Ausnahme ist eng auszulegen und zu dokumentieren.

**BDSG § 29 Abs. 1 S. 2 — Beschäftigtendaten bei Rechtsstreitigkeiten:**
- Das Auskunftsrecht kann eingeschränkt werden, soweit die Daten ausschließlich der Geltendmachung, Ausübung oder Verteidigung von Rechtsansprüchen dienen und deren Offenlegung den Rechtsanspruch gefährden würde.
- Diese Ausnahme ist restriktiv anzuwenden (BAG 2 AZR 342/20: grundsätzlich weites Auskunftsrecht von Arbeitnehmern).

**Geschäftsgeheimnisse:**
- Geschäftsgeheimnisse begründen kein pauschales Verweigerungsrecht, können aber bei der Art und Weise der Auskunftserteilung berücksichtigt werden (z. B. Zusammenfassung statt Rohdaten bei Scoring-Algorithmen).

### Schritt 6: Daten aufbereiten

**Redaktion:**
- Personenbezogene Daten Dritter konsequent schwärzen.
- Nicht über-redaktieren: Der EuGH (C-487/21) verlangt eine "originalgetreue und verständliche Reproduktion" — im Zweifel sind vollständige Dokumente (nicht nur Zusammenfassungen) herauszugeben.
- Schwärzungen nachvollziehbar kennzeichnen (z. B. "[Name Dritter geschwärzt]").

**Format:**
- Art. 12 Abs. 1 DSGVO: Auskunft in "präziser, transparenter, verständlicher und leicht zugänglicher Form in einer klaren und einfachen Sprache."
- Bei elektronischer Anfrage: Antwort in einem gängigen elektronischen Format (Art. 15 Abs. 3 S. 3 DSGVO), z. B. PDF.
- Die erste Kopie ist unentgeltlich (Art. 15 Abs. 3 S. 1 DSGVO). Für weitere Kopien darf ein angemessenes Entgelt auf Basis der Verwaltungskosten verlangt werden.

**Aufbau der Antwort:** Anschreiben + strukturierte Auskunft (Pflichtangaben) + Datenkopie.

### Schritt 7: Antwort erstellen

Die Antwort besteht aus drei Teilen:

**Teil 1 — Anschreiben:**
- Bezugnahme auf die Anfrage (Datum, Kanal)
- Bestätigung, ob personenbezogene Daten verarbeitet werden
- Hinweis auf beigefügte Auskunft und Datenkopie
- Ansprechpartner für Rückfragen
- Hinweis auf das Beschwerderecht bei der zuständigen Aufsichtsbehörde

**Teil 2 — Strukturierte Auskunft nach Art. 15 Abs. 1 a-h:** (siehe Pflichtangaben-Checkliste unten)

**Teil 3 — Datenkopie (Art. 15 Abs. 3):**
- Vollständige Kopie der verarbeiteten personenbezogenen Daten.
- EuGH C-487/21: "originalgetreue und verständliche Reproduktion" — bei Dokumenten kann das die Herausgabe ganzer Dokumente (nicht nur Auszüge) bedeuten.

### Schritt 8: Versand und Dokumentation

- **Sicherer Versandweg:** Verschlüsselte E-Mail, sicheres Portal oder Einschreiben. Niemals unverschlüsselt per E-Mail an ungeprüfte Adressen.
- **Versandnachweis:** Sendungsbeleg (Einschreiben-Beleg, E-Mail-Zustellbestätigung, Portal-Download-Log).
- **Interne Dokumentation:** Vollständige Akte anlegen mit Anfrage, internem Bearbeitungsverlauf, versandter Antwort, Versandnachweis und ggf. Begründung für etwaige Einschränkungen.
- **Aufbewahrung:** Dokumentation mindestens 3 Jahre aufbewahren (Verjährungsfrist für Schadensersatzansprüche, § 195 BGB).

## Pflichtangaben-Checkliste

Folgende Informationen müssen in der Auskunft enthalten sein (Art. 15 Abs. 1 a-h DSGVO):

| Nr. | Pflichtangabe | Inhalt / Hinweis |
|---|---|---|
| a | Verarbeitungszwecke | Alle Zwecke je Datenkategorie benennen |
| b | Datenkategorien | Stammdaten, Kontaktdaten, Vertragsdaten, Zahlungsdaten, Nutzungsdaten, etc. |
| c | Empfänger | Konkrete Empfänger benennen, nicht nur Kategorien (EuGH C-154/21). Empfänger in Drittländern gesondert angeben |
| d | Speicherdauer | Konkrete Dauer oder Kriterien für deren Festlegung |
| e | Betroffenenrechte | Hinweis auf Recht auf Berichtigung (Art. 16), Löschung (Art. 17), Einschränkung (Art. 18), Widerspruch (Art. 21) |
| f | Beschwerderecht | Recht auf Beschwerde bei einer Aufsichtsbehörde |
| g | Datenherkunft | Wenn Daten nicht beim Betroffenen erhoben wurden: Herkunftsquelle angeben |
| h | Automatisierte Entscheidungen | Automatisierte Einzelentscheidungen inkl. Profiling (Art. 22): Logik, Tragweite und Auswirkungen erläutern |
| — | Drittlandtransfers | Geeignete Garantien nach Art. 46 DSGVO nennen (Art. 15 Abs. 2) |

## Sonderfälle

**Anfrage durch aktuelle Mitarbeiter:**
- BAG 2 AZR 342/20: Breites Auskunftsrecht. Die Personalakte ist grundsätzlich vollständig offenzulegen.
- BDSG § 29 nur in engen Grenzen anwendbar (nur bei konkretem Rechtsstreit und nur für streitrelevante Daten).
- Leistungsbeurteilungen, interne Vermerke und Abmahnungen sind personenbezogene Daten.

**Anfrage durch ehemalige Mitarbeiter:**
- Das Auskunftsrecht besteht auch nach Beendigung des Arbeitsverhältnisses fort, solange Daten verarbeitet werden.
- Aufbewahrungsfristen prüfen: Lohn- und Gehaltsunterlagen (6 bzw. 10 Jahre), Personalakte (keine gesetzliche Regelung, aber typisch 3 Jahre nach Austritt).

**Anfrage über einen Anwalt:**
- Schriftliche Vollmacht verlangen (Original oder beglaubigte Kopie).
- Antwort an den Anwalt, nicht direkt an den Betroffenen (es sei denn, der Betroffene wünscht dies).
- Frist läuft ab Eingang der Anfrage, nicht ab Vorlage der Vollmacht.

**Massenanfragen (z. B. DSGVO-Aktivismus):**
- Art. 12 Abs. 5 DSGVO: Bei offensichtlich unbegründeten oder exzessiven Anfragen darf ein angemessenes Entgelt verlangt oder die Bearbeitung verweigert werden.
- Die Beweislast für den "exzessiven" Charakter liegt beim Verantwortlichen.
- Hohe Schwelle: Eine einzelne, auch umfangreiche Anfrage ist in der Regel nicht exzessiv.

## Häufige Fehler

| Fehler | Risiko | Empfehlung |
|---|---|---|
| Unvollständige Systemsuche | Unvollständige Auskunft, Bußgeld | Art. 30-Verzeichnis als Checkliste nutzen |
| Daten von Auftragsverarbeitern fehlen | Unvollständige Auskunft | Auftragsverarbeiter einbeziehen und Frist berücksichtigen |
| Übermäßige Schwärzung | Verletzung des Auskunftsrechts | Nur personenbezogene Daten Dritter schwärzen, nicht den gesamten Kontext |
| Fristüberschreitung | Bußgeld, Schadensersatz | Fristverlängerung rechtzeitig kommunizieren |
| Pauschale Ausweiskopie verlangen | Datenschutzverstoß, Verzögerung | Verhältnismäßige, kanalabhängige Verifizierung |
| Verwechslung Art. 15 mit Art. 20 | Falsche Antwort | Art. 15 = alle verarbeiteten Daten; Art. 20 (Datenübertragbarkeit) = nur automatisiert verarbeitete, selbst bereitgestellte Daten |
| Nur Datenkategorien statt konkreter Empfänger | Verstoß seit EuGH C-154/21 | Konkrete Empfänger benennen, wo der Betroffene dies verlangt |
| Bloße Zusammenfassung statt Dokumentenkopie | Verstoß seit EuGH C-487/21 | Prüfen, ob vollständige Dokumente herauszugeben sind |
| Antwort an falschen Empfänger | Datenschutzverletzung (Art. 33/34) | Empfängeridentität immer verifizieren |

## Bußgeld- und Schadensersatzrisiko

**Bußgelder (Art. 83 Abs. 5 DSGVO):**
Verstöße gegen die Betroffenenrechte (Art. 12-22) gehören zur höchsten Bußgeldkategorie: bis zu 20 Mio. EUR oder 4 % des weltweiten Jahresumsatzes (je nachdem, welcher Betrag höher ist).

**Schadensersatz (Art. 82 DSGVO):**
- Jede Person, der durch einen DSGVO-Verstoß ein materieller oder immaterieller Schaden entstanden ist, hat einen Schadensersatzanspruch.
- EuGH C-300/21: Kein Bagatellvorbehalt — auch geringe immaterielle Schäden sind ersatzfähig.
- Deutsche Gerichte sprechen für verspätete oder unvollständige Auskünfte typischerweise 100 bis 5.000 EUR immateriellen Schadensersatz zu.
- Tendenz steigend: Klageindustrie und Legal-Tech-Anbieter machen Ansprüche zunehmend gebündelt geltend.

## Grenzen dieses Skills

Dieser Skill bietet eine strukturierte Arbeitshilfe für Standardfälle. Bei folgenden Szenarien empfehlen wir die Beratung durch einen Anwalt:

- Offensichtlich unbegründete oder exzessive Anfragen, bei denen eine Verweigerung erwogen wird
- Parallele Aufsichtsverfahren oder Beschwerden bei einer Datenschutzbehörde
- Komplexe Drittlandtransfers oder internationale Konzernstrukturen
- Konflikte zwischen Auskunftsrecht und Rechten Dritter, Geschäftsgeheimnissen oder laufenden Rechtsstreitigkeiten
- Schadensersatzklagen oder gerichtliche Durchsetzung des Auskunftsrechts
- Massenanfragen durch Legal-Tech-Dienstleister oder Aktivisten
