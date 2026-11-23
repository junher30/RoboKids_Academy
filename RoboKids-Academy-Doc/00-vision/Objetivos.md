# Objetivos — RoboKids Academy

**Proyecto:** RoboKids Academy  
**Documento:** Objetivos del proyecto  
**Estado:** Propuesto  
**Versión del documento:** 0.1.0

## 1. Objetivo general

Diseñar, desarrollar e implementar una plataforma web educativa que integre entornos de programación visual y textual, simulación, gestión académica y experiencias de aprendizaje basadas en kits educativos STEM, mediante narrativas pedagógicas, recursos multimedia y mecanismos de evaluación que permitan a estudiantes y profesores desarrollar, gestionar y evidenciar procesos de aprendizaje teórico-prácticos.

## 2. Objetivos específicos

### OE-01. Diseñar la arquitectura de la plataforma

Definir una arquitectura de software modular que permita integrar los diferentes entornos educativos, los servicios de autenticación, la gestión académica y el almacenamiento de recursos y evidencias de aprendizaje.

**Resultado esperado:** Arquitectura documentada, componentes definidos y modelo de información inicial.

### OE-02. Implementar la gestión de usuarios y roles

Desarrollar mecanismos de autenticación y autorización que permitan gestionar los accesos y funcionalidades correspondientes a estudiantes, profesores y administradores.

**Resultado esperado:** Sistema de acceso con permisos diferenciados según el rol.

### OE-03. Desarrollar el entorno de programación por bloques

Integrar un espacio de programación visual que permita a los estudiantes construir programas mediante bloques gráficos y experimentar con conceptos fundamentales de programación.

**Resultado esperado:** Editor visual que permita crear, ejecutar y guardar proyectos compatibles con el entorno.

### OE-04. Integrar entornos de programación textual

Incorporar un entorno de programación textual que permita escribir, ejecutar y gestionar programas educativos, iniciando con Python como lenguaje propuesto.

**Resultado esperado:** Editor de código con ejecución controlada, visualización de resultados y almacenamiento de proyectos.

### OE-05. Integrar experiencias de simulación

Desarrollar o integrar un entorno de simulación que permita experimentar con conceptos y programas mediante representaciones virtuales.

**Resultado esperado:** Módulo de simulación conectado con las actividades de aprendizaje correspondientes.

### OE-06. Desarrollar el laboratorio de experiencias STEM

Implementar un catálogo de kits educativos que permita consultar, seleccionar y desarrollar experiencias de aprendizaje asociadas con proyectos físicos.

**Resultado esperado:** Módulo RoboKids Discovery Lab con catálogo, fichas de kits y rutas de aprendizaje.

### OE-07. Estructurar pedagógicamente los kits educativos

Diseñar un modelo de contenido que permita transformar los manuales técnicos en experiencias educativas con narrativas, saberes previos, fundamentación científica, materiales, construcción, experimentación, conexión STEM y reflexión.

**Resultado esperado:** Estructura pedagógica reutilizable para documentar y publicar diferentes kits.

### OE-08. Implementar actividades y mecanismos de evaluación

Desarrollar funcionalidades para que los profesores asignen actividades y los estudiantes presenten evidencias de aprendizaje mediante cuestionarios, trabajos, proyectos, imágenes, videos y exposiciones.

**Resultado esperado:** Sistema de actividades, entregas y evaluaciones asociado con las experiencias educativas.

### OE-09. Desarrollar el seguimiento académico

Permitir que profesores y estudiantes consulten el avance de sus experiencias educativas, las actividades realizadas y los resultados de aprendizaje alcanzados.

**Resultado esperado:** Paneles de seguimiento académico con información individual y por grupo, según el rol.

### OE-10. Integrar recursos educativos multimedia

Implementar mecanismos para organizar y consultar manuales, imágenes, documentos y videos educativos vinculados con cada experiencia de aprendizaje.

**Resultado esperado:** Biblioteca de recursos que incluya enlaces externos a videos de YouTube.

### OE-11. Validar funcional y pedagógicamente la plataforma

Diseñar y ejecutar pruebas funcionales y de aceptación que permitan verificar el cumplimiento de los requerimientos y la utilidad de los módulos educativos dentro de los escenarios establecidos.

**Resultado esperado:** Evidencias de pruebas, hallazgos documentados y resultados de validación.

### OE-12. Implementar un sistema de metas y recompensas educativas

Desarrollar un sistema de gamificación que permita establecer metas de aprendizaje, registrar su cumplimiento y otorgar recompensas digitales por la realización de actividades, trabajos, proyectos y experiencias educativas.

**Resultado esperado:** Sistema de metas, puntos de experiencia, insignias y progreso, integrado con las actividades académicas y las experiencias STEM.

**Necesidad relacionada:** N-09.

> **PENDIENTE:** Definir si las metas serán establecidas por el profesor, por el sistema o mediante ambos mecanismos.

## 3. Relación entre objetivos y necesidades

| Objetivo | Necesidades relacionadas |
|---|---|
| OE-01 | N-01, N-08 |
| OE-02 | N-05 |
| OE-03 | N-02 |
| OE-04 | N-02 |
| OE-05 | N-03 |
| OE-06 | N-04, N-08 |
| OE-07 | N-04 |
| OE-08 | N-06 |
| OE-09 | N-05, N-06 |
| OE-10 | N-07 |
| OE-11 | N-01 a N-08 |

Las relaciones se encuentran propuestas y deberán verificarse cuando se construyan los requerimientos y la matriz de trazabilidad.

## 4. Criterios generales de cumplimiento

El cumplimiento de los objetivos deberá sustentarse mediante:

1. Requerimientos funcionales y no funcionales aprobados.
2. Historias de usuario con criterios de aceptación verificables.
3. Componentes implementados y documentados.
4. Casos de prueba ejecutados.
5. Evidencias de funcionamiento de los módulos.
6. Validación de las experiencias pedagógicas.
7. Matriz de trazabilidad actualizada.

> PENDIENTE: Establecer las métricas de éxito del proyecto, la cobertura del piloto y los criterios de evaluación pedagógica.

> PENDIENTE: Definir el alcance exacto de los lenguajes, tipos de simuladores y modalidades de ejecución.

## 5. Consideraciones de implementación

Los objetivos descritos corresponden a la visión funcional del proyecto.

Su implementación se organizará por entregas y prioridades MoSCoW. No se considera que todos los objetivos deban estar completamente implementados en la primera versión del producto.

Las características del MVP quedarán determinadas en `01-requerimientos/moscow.md`, con base en el esfuerzo estimado y los recursos disponibles.

**Estado de aprobación:** Pendiente.