# Requerimientos no funcionales — RoboKids Academy

**Estado del documento:** Propuesto · **Versión documental:** 0.1.0

> **IMPORTANTE:** Los siguientes son **candidatos RNF**, no RNF válidos/aprobados todavía: sus umbrales y unidades marcados como PENDIENTE requieren acuerdos y pruebas. La categoría se basa en ISO/IEC 25010 (terminología de trabajo; revisión de versión aplicable pendiente). El mecanismo técnico propuesto no constituye decisión arquitectónica hasta registrar ADR cuando corresponda.

| ID | Categoría (ISO 25010) | Requerimiento | Métrica/umbral | Cómo se verifica |
|---|---|---|---|---|
| RNF-001 | Seguridad | El sistema debe proteger las contraseñas almacenadas. | Algoritmo, parámetros y política: PENDIENTE (unidades/criterio a aprobar) | Inspección de configuración y prueba de verificación de contraseñas |
| RNF-002 | Seguridad | El sistema debe limitar intentos de autenticación fallidos. | Máximo de intentos por ventana de minutos: PENDIENTE | Prueba automatizada de intentos sucesivos y bloqueo temporal |
| RNF-003 | Seguridad | El sistema debe impedir que una cuenta acceda a recursos de otro rol o grupo. | 0 accesos indebidos en una batería definida de casos; cobertura de la batería: PENDIENTE | Pruebas de autorización positivas y negativas por rol/grupo |
| RNF-004 | Seguridad | El sistema debe aislar la ejecución de código de estudiante de los servicios principales. | Límites de CPU, RAM, duración y red: PENDIENTE | Pruebas de límites, terminación y aislamiento |
| RNF-005 | Seguridad | El sistema debe proteger los datos personales de estudiantes. | Plazo de retención y política de minimización: PENDIENTE | Auditoría de flujos de datos, autorizaciones y políticas |
| RNF-006 | Eficiencia de desempeño | El sistema debe responder a las consultas usuales de catálogo y dashboard dentro del objetivo de latencia acordado. | Percentil, milisegundos y concurrencia: PENDIENTE | Prueba de carga con escenario y usuarios concurrentes definidos |
| RNF-007 | Fiabilidad | El sistema debe mantener una disponibilidad mensual mínima acordada. | Porcentaje mensual de disponibilidad: PENDIENTE | Monitorización y reporte mensual |
| RNF-008 | Recuperabilidad | El sistema debe permitir recuperar datos después de una falla. | RPO en horas y RTO en horas: PENDIENTE | Simulación de restauración y medición del tiempo/pérdida |
| RNF-009 | Usabilidad | El sistema debe permitir completar tareas educativas principales con un nivel de éxito acordado. | Porcentaje de éxito, tamaño de muestra y tiempo de tarea: PENDIENTE | Pruebas moderadas con usuarios representativos |
| RNF-010 | Accesibilidad | El sistema debe cumplir el nivel de accesibilidad acordado para su interfaz web. | Versión/nivel WCAG y número de incidencias toleradas: PENDIENTE | Auditoría automática y manual de accesibilidad |
| RNF-011 | Compatibilidad | El sistema debe funcionar en los navegadores y dispositivos objetivo. | Lista de versiones de navegador, resolución y tasa de aprobación: PENDIENTE | Matriz de pruebas entre navegadores y dispositivos |
| RNF-012 | Mantenibilidad | El sistema debe disponer de pruebas automatizadas sobre funciones críticas. | Cobertura o criterios mínimos por componente: PENDIENTE | Reporte CI y pruebas de aceptación |
| RNF-013 | Integridad de datos | El sistema debe registrar metas cumplidas y recompensas sin adjudicaciones duplicadas. | 0 adjudicaciones duplicadas bajo prueba concurrente; concurrencia de prueba: PENDIENTE | Prueba concurrente de doble adjudicación |
| RNF-014 | Trazabilidad | El sistema debe registrar modificaciones relevantes a calificaciones y recompensas. | Eventos auditados y retención en días: PENDIENTE | Inspección de bitácora y pruebas de auditoría |
| RNF-015 | Fiabilidad | El sistema debe preservar consistencia al recibir envíos repetidos de entregas o actividades. | Número de reintentos del escenario y porcentaje de consistencia: PENDIENTE | Pruebas de idempotencia y simultaneidad |

## Mecanismos técnicos propuestos para RNF críticos

| RNF | Mecanismo propuesto (no aprobado) |
|---|---|
| RNF-001 | Hash de contraseña mediante algoritmo de derivación robusto; decisión técnica pendiente |
| RNF-002 | Limitación de tasa por identidad/IP; umbral pendiente |
| RNF-003 | Comprobación de permisos en backend en cada recurso |
| RNF-004 | Ejecución en contenedor/sandbox sin privilegios; arquitectura por aprobar |
| RNF-005 | Control de accesos, cifrado en tránsito y políticas de retención; detalle pendiente |
| RNF-006 | Paginación, caché y consultas optimizadas; por decidir |
| RNF-007 | Monitoreo, health checks y recuperación de servicio |
| RNF-008 | Copias de seguridad verificadas y procedimiento de restauración |
| RNF-009 | Diseño guiado y pruebas de usabilidad iterativas |
| RNF-010 | HTML semántico, navegación por teclado y contraste; política pendiente |
| RNF-011 | Diseño responsivo y pruebas de compatibilidad |
| RNF-012 | Pipeline CI, pruebas unitarias e integración |
| RNF-013 | Restricción única e idempotencia transaccional en BD |
| RNF-014 | Auditoría con actor, acción y marca temporal |
| RNF-015 | Identificador de operación y transacciones |

> PENDIENTE: Completar métricas y umbrales, validar categorías ISO 25010, fijar entornos de prueba y registrar las decisiones de arquitectura que correspondan.
