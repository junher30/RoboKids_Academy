# ADR-002 — Aislamiento de código de estudiantes

| Campo | Valor |
|---|---|
| Estado | Propuesto |
| Fecha | 2026-11-23 |
| Relacionado | [Arquitectura](../arquitectura.md), [RNF](../../../01-requerimientos/RNF.md), [RF](../../../01-requerimientos/RF.md) |

## Contexto

La ejecución de programas no confiables puede comprometer información académica y disponibilidad.

## Decisión

Proponer `runner` independiente, trabajo efímero, sin privilegios ni acceso a BD y red cerrada por defecto; evaluar sandbox/VM endurecida antes de habilitar la función.

> PENDIENTE: aprobación formal y parámetros técnicos; esta decisión no está aceptada ni implementada.

## Alternativas

Ejecución dentro de api; Pyodide u otro sandbox en navegador para casos compatibles; proveedor externo de ejecución.

## Consecuencias

Mayor coste operativo y pruebas de seguridad; limita daño potencial. Contenedor ordinario por sí solo no garantiza aislamiento.
