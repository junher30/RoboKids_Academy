# HU-001 – Iniciar sesión en la plataforma

| Campo | Valor |
|---|---|
| RF asociado | [RF-001](../01-requerimientos/RF.md) |
| RNF relacionados | [RNF-001](../01-requerimientos/RNF.md), [RNF-002](../01-requerimientos/RNF.md), [RNF-005](../01-requerimientos/RNF.md) |
| Prioridad MoSCoW | Must (propuesta; esfuerzo sin validar) |
| Estimación | PENDIENTE |
| Responsable | PENDIENTE |
| Sprint/semana | PENDIENTE |
| Estado | Propuesto |

## Historia
Como **usuario registrado**, quiero **iniciar sesión con mis credenciales**, para **acceder a las funcionalidades que me corresponden**.

## Criterios de aceptación

### HU-001-CA-01
**Dado** una cuenta habilitada y credenciales válidas, **cuando** el usuario envía el formulario de inicio de sesión, **entonces** el sistema autentica la identidad y habilita una sesión asociada con la cuenta.
**Prueba vinculada:** [CP-001](../05-pruebas/plan-pruebas.md).

### HU-001-CA-02
**Dado** credenciales incorrectas, **cuando** el usuario intenta iniciar sesión, **entonces** el sistema rechaza el acceso sin indicar cuál dato es incorrecto.
**Prueba vinculada:** [CP-002](../05-pruebas/plan-pruebas.md).

### HU-001-CA-03
**Dado** una cuenta deshabilitada, **cuando** la persona intenta autenticarse con credenciales correctas, **entonces** el sistema deniega el acceso y no crea una sesión.
**Prueba vinculada:** [CP-003](../05-pruebas/plan-pruebas.md).

## Notas técnicas

- Necesidad y componente: consultar la fila de RF-001 en [trazabilidad.md](../01-requerimientos/trazabilidad.md).
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
