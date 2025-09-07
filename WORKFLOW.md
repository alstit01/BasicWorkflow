# WORKFLOW.md
---
version: 1.0
updated: 2025-09-07T00:15:00Z
---

## Purpose
Compact guide for using `agents.md` and the templates in the IDE (TDD-centered document/model workflow).

## Steps (iterations)
1. **Planning phase**
   - Instantiate `templates/plan.template.md` as `plan.md`, fill the project brief.
   - Define P-items (add acceptance criteria and references).

2. **Start a task**
   - For the next P-item, instantiate `templates/current-task.template.md` as `current-task.md`.
   - Define tests/checks first in section (2) (**TDD-first**).

3. **Implementation**
   - Derive implementation steps (3) from tests and update artifacts (`architektur.md`, models, docs) purposefully.
   - Only complete, DoD-compliant changes to `architektur.md`.

4. **Validation**
   - Run tests/checks, document results in (4); add and address review notes.
   - Transfer open items -> `backlog.md` (BL-IDs) and mark as *transferred* in `current-task.md`.

5. **Closure**
   - Archive the CT as `done/current-task.<ISO8601-UTC>.md`.
   - Check off the corresponding P-item in `plan.md`.

## Conventions
- **IDs:** `P-###`, `CT-###`, `T-###-m`, `BL-###` (sequential, gapless).
- **Timestamps:** ISO-8601 (UTC), e.g., `2025-09-07T00:15:00Z`.
- **Commits:** references to relevant IDs; short, precise messages.
- **Filenames:** lowercase, UTF-8, LF.

## Quality gates (per iteration)
- Consistency: IDs, references, versions.
- Test coverage: at least one test per acceptance criterion.
- Risks/assumptions: updated and mitigated.
- Review: brief to-dos documented.
