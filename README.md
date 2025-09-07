# README.md
---
version: 1.0
updated: 2025-09-07T00:20:00Z
---

## Zweck
Dieses Paket enthält alle notwendigen Vorlagen und die `agents.md`-Definitionen für einen TDD-zentrierten, modell- und dokumentationsgestützten Entwicklungs-Workflow.

## Inhalt
- **agents.md** → Rollen, Leitplanken und Governance
- **WORKFLOW.md** → Schritt-für-Schritt-Anleitung
- **templates/**
  - **plan.template.md** → Vorlage für `plan.md`
  - **architektur.template.md** → Vorlage für `architektur.md`
  - **current-task.template.md** → Vorlage für `current-task.md`
  - **backlog.template.md** → Vorlage für `backlog.md`

## Verwendung
1. **Initialisieren**
   - Instanziiere `plan.template.md` als `plan.md` → Projektbrief & P-Items füllen.
   - `agents.md` lesen, um Rollen & Leitplanken zu verstehen.

2. **Arbeiten mit Tasks**
   - Für jedes Arbeitspaket ein `current-task.md` aus dem Template erstellen.
   - TDD: Tests zuerst definieren, dann Umsetzung.

3. **Architektur & Doku**
   - Änderungen an `architektur.md` nur nach DoD-konformen Abschlüssen.
   - Rückverfolgbarkeit über IDs sicherstellen (P, CT, T, BL).

4. **Backlog & Abschluss**
   - Offene Punkte in `backlog.md` übertragen.
   - Abgeschlossene `current-task.md`-Dateien archivieren.

## Konventionen
- **Dateinamen:** lowercase, UTF-8, LF
- **IDs:** `P-###`, `CT-###`, `T-###-m`, `BL-###`
- **Zeitstempel:** ISO-8601 (UTC)
- **Commits:** Referenzen zu relevanten IDs
