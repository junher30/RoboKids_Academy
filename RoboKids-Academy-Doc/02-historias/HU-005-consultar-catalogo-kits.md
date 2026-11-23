# HU-005 – Consultar catálogo de kits educativos

| Campo | Valor |
|---|---|
| RF asociado | [RF-011](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-006](../01-requerimientos/RNF.md), [RNF-009](../01-requerimientos/RNF.md), [RNF-010](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **estudiante**, quiero **consultar los kits educativos publicados**, para **explorar las experiencias STEM disponibles**.

## Criterios de aceptación

### HU-005-CA-01
**Dado** al menos un kit publicado y accesible, **cuando** el estudiante abre el catálogo, **entonces** el sistema presenta los kits publicados con título e imagen o marcador alternativo.
**Prueba vinculada:** [CP-013](../05-pruebas/plan-pruebas.md).

### HU-005-CA-02
**Dado** un kit en estado borrador, **cuando** el estudiante consulta el catálogo, **entonces** el sistema no incluye ese kit entre los publicados.
**Prueba vinculada:** [CP-014](../05-pruebas/plan-pruebas.md).

### HU-005-CA-03
**Dado** el catálogo sin kits publicados visibles, **cuando** el estudiante lo abre, **entonces** el sistema muestra un estado vacío comprensible sin producir un error.
**Prueba vinculada:** [CP-015](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-011 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
- Las reglas exactas de validación y los contratos de API se definirán en arquitectura y API; no se consideran decisiones aprobadas.
- Las pruebas deberán incluir verificaciones de autorización, especialmente para información de menores cuando aplique.

> PENDIENTE: Confirmar reglas de negocio, diseño de pantallas, responsable, estimación y sprint.

## Definición de Hecho

- [ ] PR aprobado en `develop`, con ID de la historia en el título.
- [ ] Implementación con controles de acceso y manejo de errores necesarios.
- [ ] Prueba ejecutada y aprobada para **cada** criterio de aceptación.
- [ ] Documentación y matriz de trazabilidad actualizadas.
- [ ] RF, RNF, arquitectura, modelo de datos y API revisados cuando tengan impacto.
- [ ] Evidencias vinculadas al PR y seguimiento semanal actualizado.
