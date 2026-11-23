# ADR-004 — Recompensas transaccionales e idempotentes

| Campo | Valor |
|---|---|
| Estado | Propuesto |
| Fecha | 2026-11-23 |
| Relacionado | [Arquitectura](../arquitectura.md), [RNF](../../../01-requerimientos/RNF.md), [RF](../../../01-requerimientos/RF.md) |

## Contexto

Reintentos y simultaneidad pueden otorgar XP o recompensas repetidos.

## Decisión

Proponer transacción de base de datos con clave única de adjudicación, detección de idempotencia y auditoría.

> PENDIENTE: aprobación formal y parámetros técnicos; esta decisión no está aceptada ni implementada.

## Alternativas

Comprobación previa en aplicación sin restricción; cola eventual sin unicidad en BD.

## Consecuencias

Evita duplicados y permite reintentos; requiere definir política de repetición por meta/hito.
