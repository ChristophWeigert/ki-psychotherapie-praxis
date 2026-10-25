# Arbeitsweise in diesem Repository

Nutzer:innen sind approbierte Psychologische Psychotherapeut:innen in Deutschland, meist ohne technischen Hintergrund. Antworte auf Deutsch, knapp und ohne Fachjargon aus der Softwareentwicklung.

## Ablageordner
Praxisangaben und Entwürfe liegen nicht in diesem Ordner, sondern in einem eigenen Ablageordner der Nutzer:in (so geht beim Aktualisieren nichts verloren).
- Der Pfad steht in `ablageordner.txt` in diesem Ordner. Fehlt die Datei, vor dem ersten Speichern einmal fragen (Vorschlag: `Dokumente/Praxis-KI` im Benutzerordner), den Ordner anlegen und den vollständigen Pfad in `ablageordner.txt` schreiben.
- Als Plugin installiert (dieser Ordner liegt dann z. B. unter `.claude/plugins/`, `.codex/plugins/` oder `.cursor/plugins/` und wird bei Updates ersetzt): `ablageordner.txt` hier weder lesen noch schreiben. Stattdessen `Dokumente/Praxis-KI` (bzw. `Documents/Praxis-KI`) im Benutzerordner verwenden, wenn es dort `praxis.md` gibt; sonst einmal nach dem Ablageordner fragen.
- `praxis.md` und `berichte/` beziehen sich immer auf diesen Ablageordner.
- Gibt es dort schon `praxis.md` und `berichte/`, einfach weiterverwenden.

## Praxisdaten
Wenn `praxis.md` im Ablageordner existiert, Absenderangaben (Name, Titel, Praxis, Adresse, Bundesland) daraus übernehmen statt nachzufragen. Fehlt sie, einmalig anbieten, sie aus `praxis.example.md` anzulegen.

## Schreibregeln für alle Dokumente
- Fachsprache nach Psychotherapie-Richtlinie, ICD-10-GM für Diagnosen (mit Sicherheitsgrad G/V/A/Z).
- Gendern mit Doppelpunkt (Patient:in), außer die Vorlage legt das Geschlecht der Person fest.
- Nichts erfinden: fehlende oder unsichere Angaben als `[bitte ergänzen]` bzw. „_(bitte prüfen)_“ markieren und gesammelt nachfragen.
- Ergebnisse als Markdown im Ablageordner unter `berichte/` speichern (Dateiname wie im jeweiligen Skill).

## Datenschutz
- Patientendaten und `praxis.md` nie in diesem Ordner ablegen; `ablageordner.txt` nie committen oder pushen; `.gitignore` nicht aufweichen.
- Wenn Klarnamen, Adressen oder Geburtsdaten eingegeben werden, einmal pro Sitzung kurz auf Pseudonymisierung hinweisen (siehe README), dann normal weiterarbeiten.
