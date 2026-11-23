# HU-004 – Asignar experiencias de aprendizaje

| Campo | Valor |
|---|---|
| RF asociado | [RF-010](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-003](../01-requerimientos/RNF.md), [RNF-006](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **profesor**, quiero **asignar una experiencia a un grupo o estudiante**, para **orientar las actividades que deben desarrollar**.

## Criterios de aceptación

### HU-004-CA-01
**Dado** un profesor autorizado y una experiencia publicada, **cuando** asigna la experiencia a un grupo que administra, **entonces** el sistema registra la asignación y la hace visible a sus estudiantes.
**Prueba vinculada:** [CP-010](../05-pruebas/plan-pruebas.md).

### HU-004-CA-02
**Dado** una experiencia no publicada, **cuando** el profesor intenta asignarla, **entonces** el sistema impide la asignación e informa el motivo.
**Prueba vinculada:** [CP-011](../05-pruebas/plan-pruebas.md).

### HU-004-CA-03
**Dado** un profesor sin permiso sobre el grupo, **cuando** intenta asignarle una experiencia, **entonces** el sistema rechaza la operación.
**Prueba vinculada:** [CP-012](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-010 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
