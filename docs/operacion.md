# Operación del Open Lab

## Checklist inicial de GitHub

1. [x] Alojar el repositorio central en `comunidad-birria/openlab`.
2. [ ] Confirmar autenticación de dos factores y conservar métodos de recuperación seguros.
3. [ ] Definir colaboradores y permisos mínimos para tecnología, eventos y colaboradores externos.
4. [x] Habilitar Issues, Discussions y Projects en el repositorio central.
5. [ ] Crear el GitHub Project transversal con los estados del ciclo de vida.
6. [ ] Usar `project-template` para cada proyecto nuevo cuando tenga un alcance inicial claro.
7. [ ] Definir las reglas de protección de la rama principal y las revisiones mínimas.

Al 24 de septiembre de 2026, el repositorio central es público y está alojado en la organización de GitHub `comunidad-birria`; Issues, Discussions y Projects están habilitados. El tablero transversal y las reglas de protección de `main` siguen pendientes. Los repositorios de proyectos derivados pueden crearse bajo la misma organización cuando tengan alcance, responsables y documentación suficientes.

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
