---
name: nda-pruefung
description: 'KI-gestützte NDA-Analyse nach deutschem Recht. Identifiziert Risiken, fehlende Klauseln und marktunübliche Bedingungen.'
---


## Überblick

Dieser Skill leitet die systematische Prüfung von Geheimhaltungsvereinbarungen (NDAs) nach deutschem Recht an. Er deckt einseitige und gegenseitige NDAs ab, vorvertragliche Geheimhaltung, M&A-NDAs und Arbeitnehmer-Geheimhaltungsvereinbarungen. Ziel ist es, Risiken, fehlende Klauseln und marktunübliche Bedingungen zu identifizieren, bevor sie zum Problem werden.

NDAs gelten als **angemessene Geheimhaltungsmaßnahme** im Sinne von **§ 2 Nr. 1 lit. b GeschGehG** und sind damit eine Grundvoraussetzung für den gesetzlichen Geheimnisschutz. Eine fehlerhafte NDA kann dazu führen, dass Geschäftsgeheimnisse ihren Schutzstatus verlieren.

NDAs begleiten häufig Gesellschafterverhandlungen und M&A-Transaktionen — den gesellschaftsrechtlichen Rahmen liefert der Skill [Gesellschaftervereinbarung-Prüfung](/de-DE/skills/gesellschaftervereinbarung/). Soweit die NDA personenbezogene Daten der Parteien umfasst, kann ergänzend ein [Auftragsverarbeitungsvertrag (AVV)](/de-DE/skills/auftragsverarbeitung/) nach Art. 28 DSGVO erforderlich sein. Arbeitnehmer-NDAs mit Wettbewerbsverbotscharakter im Zusammenhang mit einer Kündigung sind nach dem Skill [Kündigungsprüfung](/de-DE/skills/kuendigungspruefung/) hinsichtlich Karenzentschädigung und Formerfordernissen zu bewerten.


## Systematische Prüfung

### Schritt 1: Grundlegende Struktur

Prüfe zunächst die formalen Grundlagen:

- **Parteien:** Vollständiger Firmenname mit Rechtsform (GmbH, AG, UG etc.), Sitz, Handelsregisternummer, Vertretungsberechtigung. Bei Konzernen: Ist nur die Muttergesellschaft Partei oder auch Tochtergesellschaften?
- **Einseitig oder gegenseitig:** Wer offenbart, wer empfängt? Bei gegenseitigen NDAs prüfen, ob die Pflichten tatsächlich symmetrisch sind oder ob eine Seite stärker belastet wird.
- **Zweckbestimmung:** Ist der Zweck der Offenlegung klar definiert? Ein NDA ohne konkreten Zweck (z.B. "Prüfung einer möglichen Kooperation im Bereich X") ist zu weit gefasst und schwer durchsetzbar.
- **Gegenstand:** Bezieht sich das NDA auf ein konkretes Projekt, eine Due Diligence oder eine allgemeine Geschäftsbeziehung?

**Flagge als Risiko:**
- Fehlende oder unklare Vertretungsberechtigung
- Zweckklausel fehlt vollständig
- Einseitige NDA wird als "gegenseitig" bezeichnet, obwohl nur eine Partei offenlegt

### Schritt 2: Definition vertraulicher Informationen

Die Definition ist das Herzstück jeder NDA. Prüfe:

- **Bestimmtheit:** Ist klar erkennbar, welche Informationen geschützt sind? Eine reine Generalklausel ("alle Informationen, die im Rahmen der Zusammenarbeit ausgetauscht werden") ist problematisch.
- **Kennzeichnungspflicht:** Muss die offenlegende Partei Informationen als "vertraulich" kennzeichnen? Falls ja: Gilt dies auch für mündliche Informationen (üblich: nachträgliche schriftliche Bestätigung innerhalb von 14-30 Tagen)?
- **Umfang:** Sind folgende Kategorien angemessen erfasst?
  - Technische Informationen (Quellcode, Prototypen, Algorithmen)
  - Geschäftliche Informationen (Kundenlisten, Preise, Strategien)
  - Mündlich offenbarte Informationen
  - Visuell wahrgenommene Informationen (z.B. bei Werksbesichtigungen)

**Flagge als Risiko:**
- Definition ist so weit gefasst, dass praktisch jede Information erfasst wird -- das ist aus AGB-Sicht angreifbar (§ 307 BGB)
- Keine Kennzeichnungspflicht und keine Einschränkung auf den definierten Zweck
- "Residual Knowledge"-Klausel erlaubt dem Empfänger, alles zu nutzen, was ein Mitarbeiter im Gedächtnis behält -- das höhlt den Schutz aus

### Schritt 3: Ausnahmen prüfen

Ein NDA muss **fünf Standardausnahmen** enthalten. Fehlt eine davon, ist das ein Warnsignal:

1. **Bereits öffentlich bekannt** -- Information war zum Zeitpunkt der Offenlegung bereits allgemein zugänglich
2. **Nachträglich öffentlich geworden** -- ohne Verschulden des Empfängers
3. **Bereits im Besitz** -- Empfänger hatte die Information vor Offenlegung bereits (Nachweis erforderlich)
4. **Unabhängig entwickelt** -- Empfänger hat die Information eigenständig erarbeitet
5. **Von Dritten rechtmäßig erhalten** -- ohne Verstoß gegen Geheimhaltungspflichten

**Zusätzlich prüfen:**
- **Behördliche/gerichtliche Offenlegungspflicht:** Ist eine Ausnahme für gesetzlich angeordnete Offenlegung vorgesehen? Der Empfänger sollte die offenlegende Partei vor der Offenlegung informieren dürfen (soweit gesetzlich zulässig).
- **Whistleblower-Schutz:** Ein NDA kann den Schutz nach **§ 5 GeschGehG** und dem **Hinweisgeberschutzgesetz (HinSchG)** nicht wirksam ausschließen. Klauseln, die Whistleblowing verbieten, sind unwirksam. Prüfe, ob das NDA hier zu weit geht.

**Flagge als Risiko:**
- Ausnahme für "bereits im Besitz" fehlt -- das ist ein erhebliches Risiko für den Empfänger
- Beweislast für Ausnahmen wird vollständig auf den Empfänger verlagert
- Keine Ausnahme für gesetzliche Offenlegungspflichten

### Schritt 4: Laufzeit und Nachwirkung

Prüfe die Gesamtlaufzeit (Vertragslaufzeit + Nachwirkungsfrist) anhand dieser Richtwerte:

| Kontext | Marktübliche Nachwirkung | Obergrenze |
|---|---|---|
| **B2B-Kooperation** | 2-5 Jahre nach Vertragsende | 3 Jahre am häufigsten |
| **Arbeitsvertrag** | Vertragsdauer + 1-2 Jahre | 2 Jahre nach Ausscheiden |
| **M&A / Due Diligence** | 2-3 Jahre nach Abschluss/Abbruch | 3 Jahre |
| **Technologie-Lizenz** | 3-5 Jahre nach Vertragsende | 5 Jahre |

**Prüfpunkte:**
- Ist die Nachwirkungsfrist klar definiert, oder gilt das NDA "unbefristet"? Unbefristete NDAs sind in Deutschland grundsätzlich zulässig, aber nach deutschem Verständnis unüblich und bergen Durchsetzungsrisiken.
- Gibt es ein ordentliches Kündigungsrecht? Bei Dauerschuldverhältnissen kann ein Fehlen problematisch sein (§ 314 BGB: Recht zur außerordentlichen Kündigung bleibt unberührt).
- Bei Arbeitnehmer-NDAs: Übersteigt die Nachwirkung 2 Jahre, ist besondere Vorsicht geboten.

**Flagge als Risiko:**
- Unbefristete Laufzeit ohne Kündigungsrecht
- Nachwirkung über 5 Jahre ohne sachliche Rechtfertigung
- Arbeitnehmer-NDA mit Nachwirkung über 2 Jahre

### Schritt 5: Vertragsstrafe

Die Vertragsstrafe (§§ 339-345 BGB) ist das zentrale Durchsetzungsinstrument in deutschen NDAs. Prüfe systematisch:

**Existenz und Struktur:**
- Ist überhaupt eine Vertragsstrafe vereinbart? Fehlt sie, hat die offenlegende Partei nur Schadensersatzansprüche, die einen konkreten Nachweis erfordern -- bei Geheimhaltungsverstößen oft schwierig.
- Ist die Strafe als Pauschalbetrag oder nach **Hamburger Brauch** (Höhe wird im Streitfall vom Gläubiger bestimmt und gerichtlich auf Angemessenheit überprüft) vereinbart?

**Angemessenheit der Höhe:**

| Kontext | Marktüblicher Bereich | Obergrenze (Richtwert) |
|---|---|---|
| **Arbeitsvertrag** | 1-3 Bruttomonatsgehälter | Pro Verstoß |
| **B2B KMU** | EUR 10.000 - 50.000 | Pro Verstoß |
| **B2B Großunternehmen** | EUR 50.000 - 500.000 | Pro Verstoß |
| **M&A** | Individuell, oft höher | Am Transaktionswert orientiert |

**Hamburger Brauch:**
- Der Gläubiger legt die Höhe bei Verstoß fest; der Schuldner kann gerichtliche Überprüfung verlangen.
- Vorteil: Flexibler als Pauschalbetrag. Nachteil: Unsicherheit über die tatsächliche Höhe.
- In der Praxis die häufigste Variante bei B2B-NDAs.

**Kaufleute beachten:** Zwischen Kaufleuten (§ 348 HGB) kann die Vertragsstrafe **nicht** durch das Gericht herabgesetzt werden (§ 343 BGB findet keine Anwendung). Das macht die Vereinbarung einer angemessenen Höhe besonders wichtig.

**Flagge als Risiko -- Offenlegende Partei:**
- Keine Vertragsstrafe vereinbart
- Vertragsstrafe nur bei Vorsatz (nicht bei Fahrlässigkeit)

**Flagge als Risiko -- Empfangende Partei:**
- Vertragsstrafe ohne Obergrenze ("unbegrenzt" oder kumulierend pro Verstoß ohne Cap)
- Keine Möglichkeit der gerichtlichen Überprüfung (unwirksam nach § 307 BGB in AGB)
- Vertragsstrafe auch bei leichter Fahrlässigkeit ohne Verschuldensabstufung

### Schritt 6: Rückgabe- und Vernichtungspflichten

Prüfe, was bei Vertragsende oder auf Anforderung mit den vertraulichen Informationen geschieht:

- **Rückgabe oder Vernichtung:** Ist geregelt, ob Unterlagen zurückgegeben, vernichtet oder beides werden müssen?
- **Bestätigungspflicht:** Muss die Vernichtung schriftlich bestätigt werden?
- **Ausnahmen für gesetzliche Aufbewahrungspflichten:** Der Empfänger muss Unterlagen behalten dürfen, wenn gesetzliche Aufbewahrungspflichten bestehen (z.B. handels- und steuerrechtlich: 6-10 Jahre). Fehlt diese Ausnahme, entsteht ein unlösbarer Konflikt.
- **Elektronische Kopien:** Ist geregelt, wie mit Backups, E-Mail-Archiven und Cloud-Speicher umzugehen ist? Vollständige Löschung elektronischer Kopien ist technisch oft nicht möglich (Backup-Systeme). Eine praxistaugliche Klausel erkennt das an.
- **Frist:** Ist eine angemessene Frist für die Rückgabe/Vernichtung vorgesehen (üblich: 14-30 Tage)?

**Flagge als Risiko:**
- Keine Rückgaberegelung vorhanden
- Keine Ausnahme für gesetzliche Aufbewahrungspflichten
- Unrealistische Löschungspflichten für elektronische Kopien

### Schritt 7: AGB-Kontrolle

Ein NDA unterliegt der **AGB-Kontrolle (§§ 305 ff. BGB)**, wenn es von einer Partei vorformuliert und der anderen gestellt wird. Das trifft auf die meisten NDAs zu.

**Prüfe auf typische AGB-Fallen:**

- **Überraschende Klauseln (§ 305c BGB):** Klauseln, die in einem NDA nicht zu erwarten sind, z.B. ein verstecktes Wettbewerbsverbot oder eine Exklusivitätsvereinbarung.
- **Unangemessene Benachteiligung (§ 307 BGB):**
  - Übermäßig weite Definition vertraulicher Informationen (alles ist vertraulich)
  - Unangemessen hohe Vertragsstrafe ohne gerichtliche Überprüfungsmöglichkeit
  - Umkehr der Beweislast zu Lasten des Empfängers für alle Ausnahmen
  - Einseitige Haftungsfreistellung ohne Begrenzung
- **Transparenzgebot (§ 307 Abs. 1 S. 2 BGB):** Unklare oder widersprüchliche Formulierungen gehen zu Lasten des Verwenders.

**Rechtsfolge bei Unwirksamkeit:** Unwirksame Klauseln fallen ersatzlos weg (§ 306 BGB). Der Rest des Vertrags bleibt bestehen. Geltungserhaltende Reduktion findet im AGB-Recht nicht statt -- die Klausel gilt also nicht "in reduziertem Umfang", sondern gar nicht.

**Flagge als Risiko:**
- NDA enthält ein verstecktes Wettbewerbsverbot
- Pauschalierte Schadensersatzklausel ohne Möglichkeit des Gegenbeweises
- Vollständige Beweislastumkehr für sämtliche Ausnahmetatbestände

### Schritt 8: GeschGehG-Konformität

Seit dem **Geschäftsgeheimnisgesetz (GeschGehG)** von 2019 reicht ein NDA allein nicht aus, um Geschäftsgeheimnisse zu schützen. Prüfe:

- **Angemessene Geheimhaltungsmaßnahmen (§ 2 Nr. 1 lit. b GeschGehG):** Das NDA ist eine solche Maßnahme, aber nicht die einzige. Verweist das NDA auf ergänzende technische und organisatorische Maßnahmen?
- **Reverse Engineering (§ 3 Abs. 1 Nr. 2 GeschGehG):** Reverse Engineering eines rechtmäßig erlangten Produkts ist grundsätzlich erlaubt. Ein wirksamer Ausschluss muss im NDA explizit vereinbart werden. Prüfe: Ist ein Reverse-Engineering-Verbot enthalten, und ist es angemessen?
- **Erlaubte Handlungen (§ 5 GeschGehG):** Offenlegung zum Schutz eines berechtigten Interesses (Whistleblowing, Aufdeckung rechtswidriger Handlungen) kann nicht durch NDA ausgeschlossen werden.
- **Berechtigtes Interesse an Geheimhaltung (§ 2 Nr. 1 lit. a GeschGehG):** Die Information muss einen wirtschaftlichen Wert gerade wegen ihrer Geheimheit haben. Triviale Informationen können nicht durch NDA zu Geschäftsgeheimnissen erklärt werden.

**Flagge als Risiko:**
- NDA enthält keinen Verweis auf ergänzende Schutzmaßnahmen
- Reverse-Engineering-Ausschluss fehlt, obwohl Produkte/Software offengelegt werden
- NDA versucht, § 5 GeschGehG auszuschließen (unwirksam)


## Risikobewertung

### Red Flags: Perspektive der offenlegenden Partei

| Red Flag | Risiko | Handlungsempfehlung |
|---|---|---|
| Keine Vertragsstrafe | Durchsetzung nur über Schadensersatz (Beweisproblem) | Vertragsstrafe aufnehmen, mindestens Hamburger Brauch |
| Residual-Knowledge-Klausel | Empfänger darf alles nutzen, was im Kopf bleibt | Klausel streichen oder auf allgemeines Erfahrungswissen beschränken |
| Weite "Affiliates"-Weitergabe | Vertrauliche Informationen gelangen unkontrolliert an Konzerngesellschaften | Weitergabe nur an namentlich benannte Gesellschaften oder mit Zustimmung |
| Fehlender Reverse-Engineering-Ausschluss | Produkte dürfen analysiert werden (§ 3 Abs. 1 Nr. 2 GeschGehG) | Ausdrückliches Verbot aufnehmen |
| Keine Rückgabepflicht | Informationen verbleiben dauerhaft beim Empfänger | Rückgabe-/Vernichtungsklausel mit Bestätigungspflicht |
| Kein Unterlassungsanspruch | Nur Schadensersatz, keine Möglichkeit der schnellen Unterbindung | Vertragliche Unterlassungspflicht mit Eilrechtsschutz-Klausel |

### Red Flags: Perspektive der empfangenden Partei

| Red Flag | Risiko | Handlungsempfehlung |
|---|---|---|
| Übermäßig weite Definition | Praktisch jede Information ist vertraulich | Auf den definierten Zweck beschränken, Kennzeichnungspflicht fordern |
| Keine "Prior Knowledge"-Ausnahme | Empfänger haftet für Informationen, die er bereits hatte | Standardausnahmen vollständig aufnehmen |
| Vertragsstrafe ohne Cap | Existenzbedrohende Haftung bei Verstoß | Angemessene Obergrenze oder Hamburger Brauch |
| Unbefristete Laufzeit | Ewige Bindung ohne Ausstiegsmöglichkeit | Nachwirkung auf 2-3 Jahre begrenzen |
| Verstecktes Wettbewerbsverbot | Einschränkung der Geschäftstätigkeit ohne Gegenleistung | Als AGB unwirksam (§ 305c BGB); auf Streichung bestehen |
| Umfassende Freistellungspflicht | Empfänger haftet für alle Schäden, auch unverhältnismäßige | Auf Vorsatz und grobe Fahrlässigkeit beschränken |


## Besondere Konstellationen

### Arbeitnehmer-Geheimhaltungsvereinbarungen

Arbeitnehmer-NDAs unterliegen besonderen Einschränkungen:

- **Allgemeines Berufs- und Erfahrungswissen** kann nachvertraglich nicht eingeschränkt werden. Ein NDA, das dem Arbeitnehmer verbietet, erworbene Fähigkeiten und allgemeines Branchenwissen in einer neuen Stelle zu nutzen, ist unwirksam.
- **Verdecktes Wettbewerbsverbot:** Wenn ein NDA faktisch verhindert, dass ein Arbeitnehmer in seinem Berufsfeld tätig wird, handelt es sich um ein nachvertragliches Wettbewerbsverbot. Dieses erfordert eine **Karenzentschädigung** (§ 74 Abs. 2 HGB) von mindestens 50% der zuletzt bezogenen Vergütung. Ohne Karenzentschädigung ist die Klausel nach BAG-Rechtsprechung nichtig.
- **Vertragsstrafe:** Bei Arbeitnehmern maximal 1-3 Bruttomonatsgehälter pro Verstoß. Höhere Strafen werden regelmäßig als unangemessen eingestuft.
- **AGB-Kontrolle:** Arbeitsverträge und ihre Anlagen (einschließlich NDAs) unterliegen stets der AGB-Kontrolle (§ 310 Abs. 4 BGB mit Besonderheiten des Arbeitsrechts).

**Prüffrage:** Kann der Arbeitnehmer nach Ausscheiden realistisch in seinem Berufsfeld arbeiten, ohne gegen das NDA zu verstoßen? Falls nein: verdecktes Wettbewerbsverbot.

### Grenzüberschreitende NDAs

US-amerikanische und angelsächsische NDAs weisen typischerweise Merkmale auf, die im deutschen Rechtsrahmen problematisch sind:

- **Unbefristete Laufzeit** ("in perpetuity") -- in Deutschland unüblich und bei Arbeitnehmer-NDAs bedenklich.
- **Fehlende Standardausnahmen** -- US-NDAs lassen häufig die Ausnahme "bereits im Besitz" oder "unabhängig entwickelt" weg.
- **Extensive Definitionen** -- "Confidential Information means any and all information" ist nach deutschem AGB-Recht angreifbar.
- **Injunctive Relief-Klausel** -- Verweis auf einstweiligen Rechtsschutz nach US-Recht hat in Deutschland keine Wirkung.
- **Rechtswahlklausel:** Prüfe, welches Recht gilt. Bei Arbeitnehmern mit gewöhnlichem Arbeitsort in Deutschland gilt deutsches Arbeitsrecht zwingend (Art. 8 Rom I-VO), unabhängig von der Rechtswahl.

**Empfehlung:** US-Standard-NDAs für den deutschen Rechtsraum anpassen. Mindestens: Standardausnahmen ergänzen, Laufzeit begrenzen, AGB-Konformität herstellen.

### M&A / Due Diligence

M&A-NDAs haben besondere Anforderungen:

- **Non-Solicitation:** Abwerbeverbot für Mitarbeiter und Kunden ist in M&A-NDAs üblich, aber zeitlich zu begrenzen (12-24 Monate).
- **Standstill-Klausel:** Verbot feindlicher Übernahmen für einen definierten Zeitraum. Gesondert prüfen, ob angemessen.
- **Weitergabe an Berater:** Regelung zur Einschaltung von Anwälten, Wirtschaftsprüfern und Finanzberatern mit eigener Vertraulichkeitsverpflichtung.
- **Clean-Team-Regelung:** Bei Wettbewerbern, die in Due Diligence eintreten, muss geregelt sein, welche Personen Zugang zu welchen Informationen erhalten.
- **Kürzere Nachwirkung:** 2-3 Jahre sind marktüblich, da M&A-Informationen schneller an Aktualität verlieren.


## Grenzen dieses Skills

Dieser Skill liefert eine strukturierte Erstanalyse. In folgenden Fällen ist die Hinzuziehung eines Anwalts erforderlich:

- **Verhandlung und Anpassung** komplexer NDA-Klauseln, insbesondere bei Vertragsstrafen und Haftungsregelungen
- **M&A-Transaktionen** mit erheblichem Transaktionswert oder mehreren Jurisdiktionen
- **Grenzüberschreitende NDAs**, bei denen mehrere Rechtsordnungen zusammenwirken
- **Branchenspezifische Anforderungen** (regulierte Branchen wie Pharma, Verteidigung, Finanzdienstleistungen)
- **Streitigkeiten** aus bestehenden NDAs, insbesondere bei Vertragsstrafeansprüchen
- **Arbeitnehmer-NDAs mit Wettbewerbsverbotscharakter**, die eine individuelle Prüfung der Karenzentschädigung erfordern

Compound hilft gerne bei der Prüfung, Verhandlung und Erstellung von NDAs, die den Anforderungen des deutschen Rechts standhalten.
