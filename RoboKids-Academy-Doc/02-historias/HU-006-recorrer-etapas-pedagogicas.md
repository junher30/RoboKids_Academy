# HU-006 – Consultar la ruta pedagógica de un kit

| Campo | Valor |
|---|---|
| RF asociado | [RF-013](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-006](../01-requerimientos/RNF.md), [RNF-009](../01-requerimientos/RNF.md), [RNF-010](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **estudiante**, quiero **recorrer las etapas pedagógicas de un kit**, para **comprender y desarrollar el proyecto en la secuencia prevista**.

## Criterios de aceptación

### HU-006-CA-01
**Dado** un kit publicado con etapas ordenadas, **cuando** el estudiante abre la experiencia, **entonces** el sistema presenta las etapas según el orden definido.
**Prueba vinculada:** [CP-016](../05-pruebas/plan-pruebas.md).

### HU-006-CA-02
**Dado** una etapa con contenido educativo publicado, **cuando** el estudiante selecciona la etapa, **entonces** el sistema presenta su contenido y conserva la identificación de la etapa.
**Prueba vinculada:** [CP-017](../05-pruebas/plan-pruebas.md).

### HU-006-CA-03
**Dado** un kit sin una etapa requerida configurada, **cuando** un editor autorizado intenta publicarlo, **entonces** el sistema señala la falta y bloquea la publicación hasta completar la estructura obligatoria.
**Prueba vinculada:** [CP-018](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-013 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
