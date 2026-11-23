# Contrato de API — RoboKids Academy

**Estado:** Propuesto · **Versión documental:** 0.3.0  
**Base propuesta:** `/v1` · **Formato:** JSON HTTPS · **Fuente futura:** OpenAPI (`openapi.yaml`, PENDIENTE).

> PENDIENTE: aprobar mecanismo de autenticación, estructura de errores, límites de tamaño, paginación, contratos de cada campo y HTTP status aplicables. Las rutas son propuestas de diseño, **no endpoints implementados**.

## 1. Convenciones

- Acceso protegido en backend: RBAC y pertenencia a grupo/asignación.
- `POST` de entregas y recompensas: clave `Idempotency-Key`, si aplica.
- `401` sin sesión válida; `403` sin privilegios; `404` recurso inexistente o no visible, según política; `409` conflicto de versión/idempotencia; `422` contenido inválido; `429` límite de tasa (cuando aplique).
- Los roles abreviados: `E` estudiante, `P` profesor, `A` administrador. El superadministrador permanece como posible variante no aprobada.
- Contratos resumidos, con campos **propuestos**, aún no normativos.

## 2. Rutas propuestas

| Método | Ruta | Rol | Request propuesto | Response propuesto | Errores principales | RF |
|---|---|---|---|---|---|---|
| POST | `/auth/login` | Público | `{email,password}` | `{session,user}` | 401, 429 | RF-001 |
| POST | `/auth/recover` | Público | `{email}` | `{accepted:true}` | 422, 429 | RF-004 |
| GET | `/me` | E/P/A | — | `{id,roles,groups}` | 401 | RF-002,005,006 |
| POST | `/groups` | P/A | `{name,courseId?}` | `{id,name}` | 403,422 | RF-007 |
| POST | `/groups/{id}/members` | P/A | `{studentId}` | `{membershipId}` | 403,404,409 | RF-008 |
| GET | `/kits` | E/P/A | `?category=&level=&page=` | `{items,pagination}` | 401,422 | RF-011,049 |
| GET | `/kits/{id}` | E/P/A | — | `{kit,publicVersion}` | 403,404 | RF-012,013 |
| GET | `/kits/{id}/stages` | E/P/A | `?version=` | `{stages,resources,materials}` | 403,404 | RF-014 a RF-019,023,024 |
| POST | `/kits` | A | `{title,category,level}` | `{id,version}` | 403,422 | RF-020 |
| POST | `/kits/{id}/publish` | A | `{version}` | `{publishedVersion}` | 403,409,422 | RF-021,022 |
| POST | `/assignments` | P/A | `{kitVersionId,groupId?,studentId?}` | `{id}` | 403,422 | RF-010 |
| POST | `/activities` | P | `{assignmentId,type,instructions}` | `{id}` | 403,422 | RF-026,027 |
| POST | `/activities/{id}/submissions` | E | `{evidenceRefs,links}` | `{id,status}` | 403,409,422 | RF-028 |
| POST | `/submissions/{id}/reviews` | P | `{feedback,grade?}` | `{reviewId}` | 403,409,422 | RF-029,031 |
| GET | `/progress/me` | E | — | `{assignments,goals}` | 401,403 | RF-032,038 |
| GET | `/groups/{id}/progress` | P | — | `{students,progress}` | 403,404 | RF-033 |
| POST | `/goals` | P/A | `{activityId?,learningOutcomeId?,condition}` | `{id}` | 403,422 | RF-034 |
| POST | `/goals/{id}/validate` | P/A | `{studentId,evidenceId?}` | `{goalProgressId,status}` | 403,409 | RF-035 |
| GET | `/rewards/me` | E | — | `{rewards,xp,badges,level}` | 401 | RF-036 a RF-040,050 |
| POST | `/projects` | E | `{type,title}` | `{id}` | 403,422 | RF-041,044 |
| PUT | `/projects/{id}/versions` | E propietario | `{content,language,expectedVersion}` | `{versionId}` | 403,409,422 | RF-042,046 |
| POST | `/projects/{id}/runs` | E propietario | `{versionId}` | `{jobId,status}` | 403,422,429 | RF-043,045 |
| GET | `/runs/{id}` | E propietario | — | `{status,outputLimited}` | 403,404 | RF-043,045 |
| POST | `/simulations/{id}/start` | E autorizado | `{projectId}` | `{sessionId}` | 403,409,422 | RF-047,048 |

> PENDIENTE: endpoints para CRUD completo de contenidos, recursos, cuestionarios, versiones, roles, sesiones y creación de recompensas. La tabla describe la superficie **inicial**, no cobertura contractual exhaustiva.

## 3. Ejemplos de esquemas propuestos

```json
{
  "error": {
    "code": "CONFLICT",
    "message": "La operación entra en conflicto con el estado actual",
    "requestId": "example-id"
  }
}
```

Ejemplo de evento interno para validar adjudicación (no endpoint público):

```json
{
  "studentId": "uuid",
  "goalId": "uuid",
  "ruleId": "uuid",
  "achievementKey": "unique-business-key",
  "source": "teacher-review"
}
```

## 4. Privacidad, evolución y pruebas

- Recursos protegidos: URL firmada de corta duración o descarga autenticada; no enlaces permanentes para evidencias privadas.
- Los videos YouTube enlazan al origen público, pero el enlace debe ser validado al registrarse.
- La API evolucionará con versionado de contrato; cambios incompatibles requieren evaluación y ADR.
- Cada operación debe vincularse al RF/HU/CP correspondiente a través de [trazabilidad.md](../01-requerimientos/trazabilidad.md).
- Las respuestas de éxito por caso y los ejemplos completos se detallarán en OpenAPI aprobado.
