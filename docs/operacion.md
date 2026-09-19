# Operación institucional

## Checklist inicial de GitHub

1. Crear la GitHub Organization institucional de la Fundación.
2. Activar autenticación de dos factores y definir al menos dos administradores.
3. Crear equipos con permisos mínimos: administración, tecnología, eventos y colaboradores.
4. Activar Discussions en los repositorios que funcionen como comunidad.
5. Crear un GitHub Project transversal con los estados del ciclo de vida.
6. Crear `open-lab` y `project-template` desde esta base.
7. Definir las reglas de protección de la rama principal y las revisiones mínimas.

## Issues y Discussions

- Issues: tareas, bugs, mejoras concretas, documentación pendiente y tareas de mantenimiento.
- Discussions: preguntas, propuestas, búsqueda de colaboradores, decisiones abiertas y conversación comunitaria.

## GitHub Projects

El tablero transversal recomendado usa estas columnas:

- Idea
- En desarrollo
- Demo
- Publicado
- Mantenimiento
- Archivado

El tablero no reemplaza el README ni el historial del repositorio; los conecta y permite ver el conjunto de proyectos de la Fundación.

## Automatización

Cada repositorio de proyecto debería incorporar, como mínimo:

- Escaneo de secretos.
- Validación de estructura y documentación.
- Tests y linting según la tecnología utilizada.
- Un workflow opcional para publicar una demo, cuando el proyecto lo necesite.

La plantilla incluye workflows iniciales sin asumir un stack único.
