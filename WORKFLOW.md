# WORKFLOW.md
---
version: 1.0
updated: 2025-09-07T00:15:00Z
---

## Zweck
Kompakte Anleitung zur Nutzung von `agents.md` und den Templates in der IDE (TDD-zentrierter Dokument-/Modell-Workflow).

## Schritte (Iterationen)
1. **Planungsphase**
   - `templates/plan.template.md` → als `plan.md` instanziieren, Projektbrief füllen.
   - P-Items definieren (Akzeptanzkriterien & Referenzen eintragen).

2. **Aufgabe starten**
   - Für das nächste P-Item `templates/current-task.template.md` → als `current-task.md` instanziieren.
   - Tests/Checks zuerst in Abschnitt (2) definieren (**TDD-first**).

3. **Umsetzung**
   - Aus Tests Implementierungsschritte (3) ableiten und Artefakte (`architektur.md`, Modelle, Doku) gezielt aktualisieren.
   - Nur vollständige, DoD-konforme Änderungen an `architektur.md`.

4. **Validierung**
   - Tests/Checks ausführen, Ergebnisse in (4) dokumentieren; Review-Hinweise ergänzen & adressieren.
   - Offenes → nach `backlog.md` (BL-IDs) übertragen und in `current-task.md` als *übertragen* markieren.

5. **Abschluss**
   - CT als `done/current-task.<ISO8601-UTC>.md` archivieren.
   - Passendes P-Item in `plan.md` abhaken.

## Konventionen
- **IDs:** `P-###`, `CT-###`, `T-###-m`, `BL-###` (fortlaufend, lückenlos).
- **Zeitstempel:** ISO-8601 (UTC), z. B. `2025-09-07T00:15:00Z`.
- **Commits:** Referenzen zu relevanten IDs; kurze, präzise Messages.
- **Dateinamen:** lowercase, UTF-8, LF.

## Qualitätsgates (pro Iteration)
- Konsistenz: IDs, Referenzen, Versionsstände.
- Testabdeckung: mind. ein Test pro Akzeptanzkriterium.
- Risiken/Annahmen: aktualisiert & mitigiert.
- Review: kurze To-Dos dokumentiert.
