# ADR-001 — Monolito modular para gestión académica

| Campo | Valor |
|---|---|
| Estado | Propuesto |
| Fecha | 2026-11-23 |
| Relacionado | [Arquitectura](../arquitectura.md), [RNF](../../../01-requerimientos/RNF.md), [RF](../../../01-requerimientos/RF.md) |

## Contexto

El MVP agrupa múltiples dominios académicos con equipo, presupuesto y operación por definir.

## Decisión

Proponer `api` como monolito modular con PostgreSQL propio y límites internos de módulos; `web` separado.

> PENDIENTE: aprobación formal y parámetros técnicos; esta decisión no está aceptada ni implementada.

## Alternativas

Microservicios por dominio; backend monolítico sin separación de módulos.

## Consecuencias

Menor complejidad inicial y transacciones locales; requiere disciplina de límites; posible separación futura.
