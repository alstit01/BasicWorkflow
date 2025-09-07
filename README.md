# README.md
---
version: 1.0
updated: 2025-09-07T00:20:00Z
---

## Purpose
This package contains all necessary templates and the `agents.md` definitions for a TDD-centered, model- and documentation-driven development workflow.

## Contents
- **agents.md** -> roles, guardrails, and governance
- **workflow.md** -> step-by-step guide
- **templates/**
  - **plan.template.md** -> template for `plan.md`
  - **architecture.template.md** -> template for `architecture.md`
  - **current-task.template.md** -> template for `current-task.md`
  - **backlog.template.md** -> template for `backlog.md`

## Usage
1. **Initialize**
   - Instantiate `plan.template.md` as `plan.md` -> fill project brief and P-items.
   - Read `agents.md` to understand roles and guardrails.

2. **Working with tasks**
   - For each work package, create a `current-task.md` from the template.
   - TDD: define tests first, then implement.

3. **Architecture & docs**
   - Changes to `architecture.md` only after DoD-compliant completions.
   - Ensure traceability via IDs (P, CT, T, BL).

4. **Backlog & closure**
   - Transfer open items to `backlog.md`.
   - Archive completed `current-task.md` files.

## Conventions
- **Filenames:** lowercase, UTF-8, LF
- **IDs:** `P-###`, `CT-###`, `T-###-m`, `BL-###`
- **Timestamps:** ISO-8601 (UTC)
- **Commits:** references to relevant IDs
