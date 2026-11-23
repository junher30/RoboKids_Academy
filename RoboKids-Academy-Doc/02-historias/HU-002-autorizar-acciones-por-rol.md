# HU-002 – Restringir acciones según el rol

| Campo | Valor |
|---|---|
| RF asociado | [RF-002](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-003](../01-requerimientos/RNF.md), [RNF-005](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **administrador**, quiero **asignar permisos de acceso según el rol**, para **proteger la información y las operaciones de la plataforma**.

## Criterios de aceptación

### HU-002-CA-01
**Dado** un usuario con rol de estudiante, **cuando** intenta usar una operación exclusiva de profesor, **entonces** el sistema rechaza la operación sin modificar datos.
**Prueba vinculada:** [CP-004](../05-pruebas/plan-pruebas.md).

### HU-002-CA-02
**Dado** un profesor que tiene permiso sobre su grupo, **cuando** solicita consultar sus actividades, **entonces** el sistema muestra únicamente la información autorizada.
**Prueba vinculada:** [CP-005](../05-pruebas/plan-pruebas.md).

### HU-002-CA-03
**Dado** un usuario autenticado sin autorización sobre un recurso, **cuando** accede directamente a la URL o API del recurso, **entonces** el servidor deniega el acceso independientemente de los controles de interfaz.
**Prueba vinculada:** [CP-006](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-002 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
