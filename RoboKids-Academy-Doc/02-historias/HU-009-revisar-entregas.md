# HU-009 – Revisar y retroalimentar entregas

| Campo | Valor |
|---|---|
| RF asociado | [RF-029](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-003](../01-requerimientos/RNF.md), [RNF-014](../01-requerimientos/RNF.md), [RNF-015](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **profesor**, quiero **revisar entregas y registrar observaciones**, para **orientar la mejora del aprendizaje**.

## Criterios de aceptación

### HU-009-CA-01
**Dado** una entrega presentada por un estudiante de su grupo, **cuando** el profesor abre la entrega, **entonces** el sistema muestra la evidencia autorizada para revisión.
**Prueba vinculada:** [CP-026](../05-pruebas/plan-pruebas.md).

### HU-009-CA-02
**Dado** una entrega del grupo que administra, **cuando** el profesor guarda su retroalimentación, **entonces** el sistema registra el comentario asociado a la entrega y al profesor.
**Prueba vinculada:** [CP-027](../05-pruebas/plan-pruebas.md).

### HU-009-CA-03
**Dado** una entrega de un grupo ajeno, **cuando** el profesor intenta evaluarla, **entonces** el sistema rechaza la lectura o modificación según corresponda.
**Prueba vinculada:** [CP-028](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-029 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
