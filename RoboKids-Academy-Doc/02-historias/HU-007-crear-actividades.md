# HU-007 – Crear actividades de aprendizaje

| Campo | Valor |
|---|---|
| RF asociado | [RF-026](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-003](../01-requerimientos/RNF.md), [RNF-014](../01-requerimientos/RNF.md), [RNF-015](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **profesor**, quiero **crear actividades vinculadas con experiencias STEM**, para **evaluar los conocimientos y el trabajo de mis estudiantes**.

## Criterios de aceptación

### HU-007-CA-01
**Dado** un profesor autorizado y una experiencia editable, **cuando** registra una actividad con título, instrucciones y modalidad, **entonces** el sistema guarda la actividad vinculada a la experiencia.
**Prueba vinculada:** [CP-019](../05-pruebas/plan-pruebas.md).

### HU-007-CA-02
**Dado** una actividad sin instrucciones obligatorias, **cuando** el profesor intenta guardarla, **entonces** el sistema indica la validación y no publica la actividad.
**Prueba vinculada:** [CP-020](../05-pruebas/plan-pruebas.md).

### HU-007-CA-03
**Dado** un usuario estudiante, **cuando** intenta crear una actividad mediante la API, **entonces** el sistema rechaza la operación.
**Prueba vinculada:** [CP-021](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-026 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
