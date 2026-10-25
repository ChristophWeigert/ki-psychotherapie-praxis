# Arbeitsweise in diesem Repository

Nutzer:innen sind approbierte Psychologische Psychotherapeut:innen in Deutschland, meist ohne technischen Hintergrund. Antworte auf Deutsch, knapp und ohne Fachjargon aus der Softwareentwicklung.

## Praxisdaten
Wenn `praxis.md` existiert, Absenderangaben (Name, Titel, Praxis, Adresse, Bundesland) daraus übernehmen statt nachzufragen. Fehlt sie, einmalig anbieten, sie aus `praxis.example.md` anzulegen.

## Schreibregeln für alle Dokumente
- Fachsprache nach Psychotherapie-Richtlinie, ICD-10-GM für Diagnosen (mit Sicherheitsgrad G/V/A/Z).
- Gendern mit Doppelpunkt (Patient:in), außer die Vorlage legt das Geschlecht der Person fest.
- Nichts erfinden: fehlende oder unsichere Angaben als `[bitte ergänzen]` bzw. „_(bitte prüfen)_“ markieren und gesammelt nachfragen.
- Ergebnisse als Markdown unter `berichte/` speichern (Dateiname wie im jeweiligen Skill).

## Datenschutz
- `berichte/` und `praxis.md` niemals committen oder pushen; `.gitignore` nicht aufweichen.
- Wenn Klarnamen, Adressen oder Geburtsdaten eingegeben werden, einmal pro Sitzung kurz auf Pseudonymisierung hinweisen (siehe README), dann normal weiterarbeiten.
