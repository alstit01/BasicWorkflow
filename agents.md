# agents.md
---
version: 1.1
updated: 2025-09-07T00:15:00Z
owner: <User/Team>
---

## Rollen
- **Planner**: plant Arbeitspakete & Abhängigkeiten.
- **Architect**: definiert/aktualisiert Ziel-Architektur & Schnittstellen.
- **Implementer**: setzt Aufgaben gemäß TDD um.
- **Reviewer**: prüft Qualität, DoD & Konsistenz.
- **QA**: entwirft/automatisiert Tests/Checks (SW, Modelle, Doku).

## Leitplanken
- **TDD-first**, kleine Inkremente, klare Akzeptanzkriterien je Aufgabe.
- **Rückverfolgbarkeit**: IDs (P-<NNN>, CT-<NNN>, T-<NNN>-<m>, BL-<NNN>) in Dateien & Commits.
- **Arbeitsfluss**: Änderungen nur über `current-task.md`; Architektur nur nach DoD-abschlussener Iteration.
- **DoD**: (a) Akzeptanzkriterien erfüllt, (b) Tests/Checks grün, (c) Review-Hinweise adressiert, (d) Artefakte konsistent, (e) Architektur nur bei vollständig erledigten Schritten angepasst.
- **Namens-/Formatkonvention**: Dateinamen **lowercase**, UTF-8, LF; Zeitstempel **ISO-8601 (UTC)**.
- **Commit-Messages** (Beispiel): `feat(plan): P-001 init — scope & risks (#CT-001)`; immer IDs referenzieren.

## Verwendung der Templates
- Instanziiere Vorlagen aus `templates/` in der IDE, fülle Platzhalter **<...>** aus.
- Jede Iteration: `current-task.md` aktualisieren → Tests/Checks definieren → Implementierung/Docs → Ergebnisse → ggf. offene Punkte nach `backlog.md` übertragen → Plan abhaken.
