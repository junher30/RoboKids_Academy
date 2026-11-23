# HU-008 – Entregar evidencias de actividades

| Campo | Valor |
|---|---|
| RF asociado | [RF-028](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-003](../01-requerimientos/RNF.md), [RNF-005](../01-requerimientos/RNF.md), [RNF-015](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **estudiante**, quiero **entregar la evidencia admitida por una actividad**, para **demostrar el trabajo que realicé**.

## Criterios de aceptación

### HU-008-CA-01
**Dado** una actividad asignada que admite archivos y una evidencia válida, **cuando** el estudiante realiza la entrega, **entonces** el sistema conserva el archivo asociado al estudiante y a la actividad y confirma la recepción.
**Prueba vinculada:** [CP-022](../05-pruebas/plan-pruebas.md).

### HU-008-CA-02
**Dado** una actividad que admite enlaces y una URL válida, **cuando** el estudiante entrega el enlace, **entonces** el sistema registra el enlace sin exigirle publicar el video dentro de la plataforma.
**Prueba vinculada:** [CP-023](../05-pruebas/plan-pruebas.md).

### HU-008-CA-03
**Dado** una evidencia con tipo no permitido por la actividad, **cuando** el estudiante intenta enviarla, **entonces** el sistema rechaza la entrega y explica el formato admitido.
**Prueba vinculada:** [CP-024](../05-pruebas/plan-pruebas.md).

### HU-008-CA-04
**Dado** una actividad asignada a otro estudiante, **cuando** un usuario intenta entregar evidencia en su nombre sin autorización, **entonces** el sistema deniega la operación.
**Prueba vinculada:** [CP-025](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-028 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
