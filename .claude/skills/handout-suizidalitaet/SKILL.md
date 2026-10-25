---
name: handout-suizidalitaet
description: "Erstellt ein individuell angepasstes Handout für suizidgefährdete Patient:innen mit regionalem Notfallplan (regionaler Krisendienst, Telefonseelsorge, psychiatrische Notaufnahmen), optional in einer Autismus-Version. Verwenden, wenn die Therapeut:in einen Notfallplan, Krisenplan oder ein Handout bei akuter Suizidalität benötigt."
argument-hint: "[Region]"
disable-model-invocation: true
---

# Handout: Akute Suizidalität

Du erstellst ein individuell angepasstes Handout für suizidgefährdete Patient:innen mit einem regionalen Notfallplan für den Wohnort der Patient:in in Deutschland.

## Vorgehen

1. **Geführte Abfrage** mit Auswahloptionen, sofern das Werkzeug das anbietet (max. 4 Fragen pro Runde; Freitext ist über "Other" immer möglich). Falls das Tool nicht verfügbar ist oder die Fragen unbeantwortet bleiben: nummerierte Fragen direkt im Chat stellen
2. Erstelle das Handout nach dem festgelegten Schema (siehe [references/schema.md](references/schema.md)) und halte die Formatierungsregeln ein
3. **Speicherort:** Handout als Markdown-Datei im Ablageordner (Regeln in `AGENTS.md`, drei Ordnerebenen über dieser Datei; vorher lesen, falls noch nicht bekannt) unter `berichte/handout-akute-suizidalitaet-[region].md` ablegen (bei Autismus-Version Suffix `-autismus`)

## Informationen abfragen

### 1. Region
- In welchem Bundesland und welcher Stadt / welchem Landkreis wohnt die Patient:in? (Bundesland aus `praxis.md` vorschlagen)
- Wie soll die Region im Handout-Titel heißen?
- Regionaler Krisendienst für Schritt 3: in Bayern immer der Krisendienst Bayern (0800 655 3000). Anderswo einen passenden Dienst vorschlagen (landesweiter oder städtischer Krisendienst, sonst Sozialpsychiatrischer Dienst mit Erreichbarkeit) und bestätigen lassen; gibt es keinen, die Zeile durch den ärztlichen Bereitschaftsdienst 116 117 ersetzen.

### 2. Autismus-Diagnose
- Liegt eine Autismus-Diagnose vor? (Beeinflusst Schritt 1, Schritt 3 und die Überbrückungsstrategien)

### 3. Psychiatrische Kliniken
Relevante Kliniken in der Region (1–4 Einrichtungen) – Vorschläge machen und bestätigen lassen:
- Name der Einrichtung
- Adresse
- Telefonnummer
- Art der Notaufnahme (psychiatrische Notaufnahme 24h / über Allgemeine Notaufnahme)

**Wichtig:** Telefonnummern und Adressen nie raten. Vorgeschlagene Nummern als „vor Aushändigung prüfen“ kennzeichnen und die Therapeut:in ausdrücklich darauf hinweisen.

## Formatierungsregeln

- Keine `---` zwischen den Schritten; `---` nur zwischen den Hauptabschnitten
- Keine Fettung bei Feldbezeichnungen (Name:, Erreichbar per:)
- Blockquote (`>`) für die Musternachricht in Schritt 2
- Fettung in „Wichtig zu wissen“ erhalten
- Ausfüllfelder direkt unter der Frage, ohne Leerzeile
- Kein abschließender Hinweis auf die Praxis
