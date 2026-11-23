# HU-012 – Otorgar recompensas por metas alcanzadas

| Campo | Valor |
|---|---|
| RF asociado | [RF-036](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-013](../01-requerimientos/RNF.md), [RNF-014](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **estudiante**, quiero **recibir una recompensa por una meta validada**, para **reconocer el esfuerzo y mis logros de aprendizaje**.

## Criterios de aceptación

### HU-012-CA-01
**Dado** una meta validada con recompensa configurada, **cuando** se confirma el cumplimiento de la meta, **entonces** el sistema registra la recompensa a nombre del estudiante.
**Prueba vinculada:** [CP-035](../05-pruebas/plan-pruebas.md).

### HU-012-CA-02
**Dado** una meta aún pendiente de validación, **cuando** se consulta o procesa la asignación de recompensas, **entonces** el sistema no entrega la recompensa.
**Prueba vinculada:** [CP-036](../05-pruebas/plan-pruebas.md).

### HU-012-CA-03
**Dado** una recompensa ya adjudicada y cuya regla permite una sola adjudicación, **cuando** se vuelve a procesar el mismo cumplimiento, **entonces** el sistema no crea otra adjudicación.
**Prueba vinculada:** [CP-037](../05-pruebas/plan-pruebas.md).

### HU-012-CA-04
**Dado** una recompensa correctamente otorgada, **cuando** el estudiante consulta su registro de recompensas, **entonces** el sistema muestra la recompensa asociada a su cuenta.
**Prueba vinculada:** [CP-038](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-036 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
