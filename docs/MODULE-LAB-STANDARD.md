# Module Lab Standard

This document defines the canonical model that all learning units must follow in this repository.

## Scope

- Applies to `modules/*`.
- Migration target for `trends-extras/*`.

## Canonical Folder Layout

Each learning unit must contain:

```text
<unit>/
  README.md
  STATUS.md
  theory/
    README.md
  examples/
    README.md
  practices/
    README.md
  mini-project/
    README.md
  evaluation/
    README.md
  notes/
    README.md
```

## Required README Headings

### Unit `README.md`

1. `# <Module Title>`
2. `## Objetivo del modulo`
3. `## Que vas a lograr`
4. `## Estructura interna`
5. `## Ruta de niveles (L1-L4)`
6. `## Plan recomendado (por progreso, no por semanas)`
7. `## Criterio de modulo completado`

### `theory/README.md`

1. `# Theory - <Module Title>`
2. `## Por que este modulo importa`
3. `## Checklist de comprension final`

### `examples/README.md`

1. `# Examples - <Module Title>`
2. `## Ejemplos disponibles`
3. `## Como usar estos ejemplos`
4. `## Proximos pasos`

### `practices/README.md`

1. `# Practices - <Module Title>`
2. `## Practicas`
3. `## Criterio de aprobacion`

### `mini-project/README.md`

1. `# Mini-project - <Module Title>`
2. `## Proyecto`
3. `## Objetivo`
4. `## Alcance`
5. `## Entregables`
6. `## Criterios de aceptacion`

### `evaluation/README.md`

1. `# Evaluation - <Module Title>`
2. `## Ponderacion`
3. `## Rubrica`
4. `## Evaluacion final`
5. `## Criterio de aprobacion`

### `notes/README.md`

1. `# Notes - <Module Title>`
2. `## Como usar esta carpeta`

### `STATUS.md`

1. `# Estado - <Module Title>`
2. `## Progreso actual`
3. `## Checklist`
4. `## Bloqueos`
5. `## Proximos pasos`

## Lab Completeness Definition

A unit is considered lab-complete when:

1. It is self-contained: all required folders and readmes exist.
2. It includes guided and autonomous practice instructions.
3. It includes an evaluation rubric and completion threshold.
4. It has status tracking (`STATUS.md`).
5. It passes automated contract checks.

## Testing Strategy (Incremental)

- Phase 1: Contract tests (structure + headings + required sections).
- Phase 2: Add smoke tests per unit for executable assets where present.
- Phase 3: Add stricter validation for `trends-extras/*` until parity with `modules/*`.

## Enforcement

- Local: pre-commit hook runs `scripts/validate_learning_labs.py`.
- Manual: `python scripts/validate_learning_labs.py --strict-core`.
- CI (future): run strict mode for both core and extras after migration.
