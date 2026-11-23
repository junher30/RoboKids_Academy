# HU-011 – Registrar cumplimiento de metas

| Campo | Valor |
|---|---|
| RF asociado | [RF-035](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-013](../01-requerimientos/RNF.md), [RNF-014](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **estudiante**, quiero **ver el cumplimiento de mis metas según evidencias validadas**, para **conocer mi avance real**.

## Criterios de aceptación

### HU-011-CA-01
**Dado** una meta cuya regla exige revisión del profesor y una entrega aún no validada, **cuando** el estudiante entrega el trabajo, **entonces** la meta permanece pendiente hasta cumplir la condición de validación.
**Prueba vinculada:** [CP-032](../05-pruebas/plan-pruebas.md).

### HU-011-CA-02
**Dado** una meta con todas sus condiciones verificadas, **cuando** el sistema procesa el evento de cumplimiento, **entonces** el sistema registra la meta como alcanzada para el estudiante.
**Prueba vinculada:** [CP-033](../05-pruebas/plan-pruebas.md).

### HU-011-CA-03
**Dado** un evento de cumplimiento ya registrado, **cuando** el sistema recibe el mismo evento de nuevo, **entonces** el estado de la meta permanece consistente y no se registra un segundo cumplimiento.
**Prueba vinculada:** [CP-034](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-035 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
