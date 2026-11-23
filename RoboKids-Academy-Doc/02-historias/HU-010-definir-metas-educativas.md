# HU-010 – Definir metas educativas

| Campo | Valor |
|---|---|
| RF asociado | [RF-034](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-013](../01-requerimientos/RNF.md), [RNF-014](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **profesor**, quiero **definir metas ligadas a actividades o resultados de aprendizaje**, para **orientar el progreso de mis estudiantes**.

## Criterios de aceptación

### HU-010-CA-01
**Dado** una actividad existente y un profesor autorizado, **cuando** define una meta con su condición verificable de cumplimiento, **entonces** el sistema registra la meta vinculada a la actividad.
**Prueba vinculada:** [CP-029](../05-pruebas/plan-pruebas.md).

### HU-010-CA-02
**Dado** una meta sin condición de cumplimiento, **cuando** el profesor intenta activarla, **entonces** el sistema rechaza su activación y solicita la condición.
**Prueba vinculada:** [CP-030](../05-pruebas/plan-pruebas.md).

### HU-010-CA-03
**Dado** un usuario sin permisos de edición de metas, **cuando** intenta modificar una meta, **entonces** el sistema deniega la operación.
**Prueba vinculada:** [CP-031](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-034 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
