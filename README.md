# Schmerz- und Verlaufsdokumentation

Eine private Web-App zur täglichen Schmerz- und Funktionserfassung nach schwerer Rückfußverletzung,
mit druckfertigem Arzt-Dossier, standardisierten Fragebögen und einem Gesprächsbogen für die
Sprechstunde.

**Live:** siehe GitHub-Pages-Adresse dieses Repositories
**Datei:** `index.html` — eine einzige, in sich geschlossene Datei

---

## Datenschutz

Das ist der wichtigste Punkt, deshalb steht er oben:

- Die Seite lädt **keine einzige externe Datei** — keine Schriftarten, keine Diagrammbibliothek,
  kein Analyse-Skript. Sie funktioniert vollständig offline.
- Alle Eingaben liegen **ausschließlich im Browser des jeweiligen Geräts** (`localStorage`).
  Es gibt keinen Server, keine Datenbank, keine Übertragung an GitHub.
- Im Repository steht damit nur das leere Werkzeug, niemals ein Gesundheitsdatum.
- Kehrseite: Browserdaten löschen, privater Modus oder Gerätewechsel bedeuten Datenverlust.
  Deshalb regelmäßig unter **Daten & Export → Sicherung** eine JSON-Datei erzeugen und
  außerhalb des Geräts ablegen.

---

## Was drin ist

| Bereich | Inhalt |
|---|---|
| **Übersicht** | Kennzahlen über 7/14/30/90 Tage, Schmerz- und Funktionsverlauf als Diagramm, automatisch erkannte Muster |
| **Tageseintrag** | Ruhe-, Belastungs- und Maximalschmerz (NRS 0–10), Schmerzcharakter und Lokalisation, Nachtschmerz mit Weckzeit, Gehstrecke, Stehdauer, Hilfsmittel, Medikation und Wirkung, Lokalbefund mit CRPS-Merkmalen, Alltagsbeeinträchtigung, seelische Belastung |
| **Verlauf** | Vollständige Tabelle aller Einträge, editierbar, CSV-Export |
| **Fragebögen** | Fuß-Funktions-Index (FFI-orientiert), AOFAS Ankle-Hindfoot Score, schmerzbedingte Beeinträchtigung (PROMIS-orientiert), PHQ-9, Selbstbeobachtung zu neuropathischem Schmerz und CRPS entlang der Budapest-Symptomgruppen |
| **Arzt-Dossier** | Druckfertige Fallzusammenfassung: Fragestellung voran, Unfallhergang, OP-Zeitstrahl, Diagnosen, Bildgebung, ausgeschöpfte Therapien, Messwerte automatisch aus dem Tagebuch, Teilhabe, Anlagen-Checkliste |
| **Arztgespräch** | 25 vorbereitete Fragen in 6 Blöcken mit Begründung und Platz für die Antworten des Arztes |
| **Evidenz & Studien** | Aufbereitete Studienlage zum Vergleich Extremitaetenerhalt gegen Amputation bei Rueckfussverletzungen (OUTLET, LEAP, METALS, Bennett, Dickens), Ergebnisse der Amputation bei therapierefraktaerem Schmerz, ehrliche Gegenrechnung der Risiken, Erfolgsraten weiterer Arthrodeseversuche, publizierter Entscheidungsalgorithmus, deutsche Leitlinien, Zweitmeinungswege, spezialisierte Kliniken, GdB und MdE, Patientenrechte, Peer-Support |
| **Daten & Export** | JSON-Sicherung und -Wiederherstellung, CSV, Gesamtdokumentation als PDF |

---

## Nutzung im Alltag

1. **Täglich**, am besten abends zur gleichen Zeit: Tageseintrag ausfüllen. Zwei Minuten reichen.
2. **Alle vier Wochen**: einen oder zwei Fragebögen ausfüllen, damit ein Verlauf entsteht.
3. **Vor einem Termin**: Arzt-Dossier aktualisieren, dann *Gesamtdokumentation drucken* und im
   Druckdialog „Als PDF sichern“ wählen. Zweimal ausdrucken — eine Kopie bleibt beim Arzt.
4. **Nach dem Termin**: Antworten im Gesprächsbogen nachtragen.
5. **Monatlich**: JSON-Sicherung herunterladen.

Ein Hinweis zur Wirkung: Die Dokumentation überzeugt durch Konstanz und Differenzierung, nicht
durch hohe Zahlen. Gute Tage einzutragen macht die schlechten glaubwürdig.

---

## Fachliche Grundlagen

Die Begründungstexte im Gesprächsbogen stützen sich unter anderem auf:

- **LEAP-Studie** (Lower Extremity Assessment Project), MacKenzie/Bosse et al., *NEJM* 2002 und
  Folgearbeiten: kein signifikanter Funktionsunterschied zwischen Rekonstruktion und Amputation
  nach zwei Jahren (SIP 12,6 vs. 11,8; p = 0,53), jedoch höhere Rate an Wiederaufnahmen wegen
  Komplikationen nach Rekonstruktion (47,5 % vs. 33,9 %).
- **Revision der subtalaren Arthrodese**: Durchbauungsraten von bis über 90 % bei Primäreingriffen
  gegenüber rund 71 % bei Revisionen (Easley et al.); strukturelle Allografts mit hoher
  Pseudarthroserate in kleinen Serien; patientenspezifische 3D-gedruckte Titanimplantate bei
  Defekten über 2 cm; Entnahmemorbidität an der Tibia (ca. 6,8 %) geringer als am Beckenkamm.
- **TMR und RPNI** (Targeted Muscle Reinnervation, Regenerative Peripheral Nerve Interface) zum
  Zeitpunkt der Amputation: Reduktion von Phantom- und Stumpfschmerz sowie symptomatischer Neurome.
- **Budapest-Kriterien** zur Klassifikation des komplexen regionalen Schmerzsyndroms.

Die Fragebögen sind Selbsteinschätzungsinstrumente in an die Originalinstrumente angelehnter
Struktur. Für formale Begutachtungen sollte die offizielle validierte Fassung über die Behandler
bezogen werden. Der PHQ-9 ist frei verwendbar.

---

## Haftungsausschluss

Dieses Werkzeug dokumentiert eigene Beobachtungen. Es stellt keine Diagnose, ersetzt keine
ärztliche Beratung und trifft keine Behandlungsentscheidung. Bei akuter Verschlechterung, Fieber,
zunehmender Rötung, Wundsekret oder plötzlichem Funktionsverlust gehört der Fuß sofort ärztlich
untersucht.
