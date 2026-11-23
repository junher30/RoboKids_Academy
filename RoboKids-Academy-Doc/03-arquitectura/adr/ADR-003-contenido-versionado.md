# ADR-003 — Versionado de experiencias y kits

| Campo | Valor |
|---|---|
| Estado | Propuesto |
| Fecha | 2026-11-23 |
| Relacionado | [Arquitectura](../arquitectura.md), [RNF](../../../01-requerimientos/RNF.md), [RF](../../../01-requerimientos/RF.md) |

## Contexto

Los manuales y narrativas evolucionan mientras los estudiantes tienen actividades en curso.

## Decisión

Proponer asignaciones vinculadas a `VersionKit` publicado e inmutable; ediciones generan otra versión.

> PENDIENTE: aprobación formal y parámetros técnicos; esta decisión no está aceptada ni implementada.

## Alternativas

Edición de contenido en sitio sin historia; duplicar cada kit completo.

## Consecuencias

Permite reproducibilidad y auditoría pedagógica; requiere migración de versiones y almacenamiento adicional.
