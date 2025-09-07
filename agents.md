# agents.md
---
version: 1.1
updated: 2025-09-07T00:15:00Z
owner: <User/Team>
---

## Roles
- **Planner**: plans work packages and dependencies.
- **Architect**: defines/updates target architecture and interfaces.
- **Implementer**: implements tasks following TDD.
- **Reviewer**: reviews quality, DoD, and consistency.
- **QA**: designs/automates tests/checks (software, models, docs).

## Guardrails
- **TDD-first**, small increments, clear acceptance criteria per task.
- **Traceability**: IDs (P-<NNN>, CT-<NNN>, T-<NNN>-<m>, BL-<NNN>) in files and commits.
- **Workflow**: changes only via `current-task.md`; architecture only after a DoD-complete iteration.
- **DoD**: (a) acceptance criteria met, (b) tests/checks green, (c) review notes addressed, (d) artifacts consistent, (e) architecture adjusted only when steps are fully completed.
- **Naming/formatting conventions**: filenames **lowercase**, UTF-8, LF; timestamps **ISO-8601 (UTC)**.
- **Commit messages** (example): `feat(plan): P-001 init - scope & risks (#CT-001)`; always reference IDs.

## Using the Templates
- Instantiate templates from `templates/` in the IDE and fill placeholders **<...>**.
- Each iteration: update `current-task.md` -> define tests/checks -> implementation/docs -> results -> transfer open items to `backlog.md` if needed -> check off the plan.
