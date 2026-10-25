# Psychotherapie-Skills – KI-Vorlagen für Psychotherapeut:innen in Deutschland

Vorlagen im offenen [Agent-Skills-Format](https://agentskills.io) (`SKILL.md`) für wiederkehrende Schreibarbeit in der psychotherapeutischen Praxis: Berichte, Anträge, Handouts. Nutzbar mit Claude Code, OpenAI Codex, GitHub Copilot, Cursor, Gemini CLI und anderen KI-Assistenten, die Skills unterstützen. Der Assistent fragt fehlende Angaben ab, schreibt einen Entwurf nach `berichte/` und überarbeitet ihn mit dir.

**Geltungsbereich:** Deutschland (GKV, Psychotherapie-Richtlinie, PTV-Formulare), alle Bundesländer. Für Österreich und die Schweiz passen die Vorlagen nicht ohne Anpassung (andere Kassen-, Antrags- und Behördenwege).

## Skills

| Befehl | Zweck | Region |
|---|---|---|
| `/arztbrief` | Bericht an überweisende/mitbehandelnde Ärzt:innen | DE |
| `/gutachterantrag-umwandlung-vt` | Bericht an Gutachter (PTV 3), Umwandlung KZT → LZT, VT | DE |
| `/indikationsschreiben-mastektomie` | Indikation Mastektomie bei Geschlechtsinkongruenz (S3-LL AWMF 138/001) | DE |
| `/hoeherstufung-gdb` | Stellungnahme zur GdB-Höherstufung bei der Versorgungsbehörde | DE (Behörde je nach Bundesland) |
| `/handout-suizidalitaet` | Handout mit regionalem Notfallplan | DE (Krisendienst/Kliniken je nach Wohnort) |

Regionale Angaben: Die Skills übernehmen das Bundesland aus `praxis.md` (sonst fragen sie nach). `/hoeherstufung-gdb` adressiert die zuständige Behörde (Bayern: ZBFS, sonst Landes- bzw. Versorgungsamt) laut Bescheid. `/handout-suizidalitaet` nutzt in Bayern den Krisendienst Bayern, anderswo einen regionalen Krisendienst oder ersatzweise 116 117, und schlägt Kliniken am Wohnort vor. Vorgeschlagene Nummern, Adressen und Kliniken vor der Ausgabe immer prüfen.

Die Skills starten nur, wenn du sie ausdrücklich aufrufst (in Claude Code per `/befehl`, in anderen Werkzeugen über deren Skill-Aufruf oder z.B. „Nutze den Skill arztbrief“).

## Einrichtung

1. Einen KI-Assistenten mit Skill-Unterstützung installieren und diesen Ordner öffnen. Die Skills liegen unter `.claude/skills/`; Claude Code findet sie dort direkt. Erwartet dein Werkzeug einen anderen Ordner (siehe dessen Dokumentation), den Ordner dorthin kopieren oder verlinken. Gemeinsame Regeln stehen in `AGENTS.md`, das die meisten Werkzeuge automatisch lesen.
2. `praxis.example.md` nach `praxis.md` kopieren und ausfüllen (Name, Titel, Praxisadresse, Bundesland). Die Skills übernehmen diese Angaben, statt jedes Mal nachzufragen.
3. Einen Skill aufrufen, z.B. `/arztbrief Verlaufsbericht` (Claude Code), und Unterlagen (Notizen, Vorbefunde) hineinkopieren oder als Datei angeben.

## Datenschutz – bitte lesen

- **Patientendaten verlassen deinen Rechner.** Alles, was du eingibst, wird zur Verarbeitung an den Anbieter des KI-Modells übertragen (z.B. Anthropic, OpenAI, Google, Microsoft). Prüfe vor dem Einsatz mit echten Daten DSGVO (Art. 9, Art. 28 – Auftragsverarbeitungsvertrag) und deine Schweigepflicht (§ 203 StGB). Private Consumer-Konten haben in der Regel keinen AVV; nutze ein Business/Enterprise- oder API-Konto mit AVV und ohne Datenspeicherung zu Trainingszwecken, oder arbeite nur mit **pseudonymisierten** Daten (Chiffre, Initialen, keine Adresse/Geburtsdatum – Echtdaten erst im fertigen Dokument in deiner Praxissoftware ergänzen).
- `berichte/` und `praxis.md` sind per `.gitignore` von Git ausgeschlossen. Lade dieses Repository mit Patientendaten **nie** auf GitHub o.Ä. hoch.
- Jeder Entwurf ist ein Entwurf: fachlich prüfen, Verantwortung bleibt bei dir.

## Eigene Skills ergänzen

Neuer Ordner unter `.claude/skills/<name>/SKILL.md`, am besten eine bestehende Vorlage kopieren. Gemeinsame Regeln (Sprache, Gendern, Speicherort) stehen in [AGENTS.md](AGENTS.md) und müssen nicht in jedem Skill wiederholt werden. Regional gebundene Inhalte (Krisendienste, Versorgungsämter) im Skill-Namen oder in der Beschreibung kennzeichnen.
