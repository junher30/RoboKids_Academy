# HU-003 – Crear y administrar grupos educativos

| Campo | Valor |
|---|---|
| RF asociado | [RF-007](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-003](../01-requerimientos/RNF.md), [RNF-006](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **profesor**, quiero **crear y consultar los grupos que administro**, para **organizar a mis estudiantes y actividades**.

## Criterios de aceptación

### HU-003-CA-01
**Dado** un profesor autenticado y datos válidos del grupo, **cuando** solicita crear un grupo, **entonces** el sistema registra el grupo asociado al profesor y lo muestra en su panel.
**Prueba vinculada:** [CP-007](../05-pruebas/plan-pruebas.md).

### HU-003-CA-02
**Dado** un formulario de grupo sin un nombre requerido, **cuando** el profesor intenta guardar, **entonces** el sistema informa los campos obligatorios y no crea el grupo.
**Prueba vinculada:** [CP-008](../05-pruebas/plan-pruebas.md).

### HU-003-CA-03
**Dado** un profesor que no administra cierto grupo, **cuando** intenta modificar dicho grupo, **entonces** el sistema rechaza la modificación.
**Prueba vinculada:** [CP-009](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-007 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
