# Instrucciones para OpenAI Codex

Estas instrucciones complementan [`AGENTS.md`](AGENTS.md), que es la guía común del repositorio.

## Contexto de trabajo

Este repositorio es documentation-first. Antes de proponer código, confirmar que la tarea realmente requiere crear un proyecto derivado o agregar una implementación. Para EcoLabs, la prioridad es que la propuesta, la dinámica y los productos del taller sean claros, ejecutables y continuables.

## Flujo recomendado

1. Revisar `git status --short` y preservar cambios no relacionados.
2. Leer el documento específico de la tarea antes de editar.
3. Explicitar en la respuesta qué es hecho, qué es recomendación y qué queda pendiente.
4. Editar con cambios pequeños y revisar el diff real.
5. Ejecutar `git diff --check` y las validaciones disponibles.
6. Commitear solo los archivos relacionados con la tarea.
7. No publicar cambios remotos salvo pedido explícito.

## Para tareas sobre EcoLabs

- Mantener separadas las dos escalas: programa completo de tres laboratorios y piloto Tecnoteca.
- Conservar el modelo de tres niveles: inicial, intermedio y avanzado.
- Recordar que el resultado del piloto es un prototipo o material preparado, no una aplicación productiva.
- No agregar datos territoriales no verificados.
- Registrar el uso de Claude u otra herramienta de IA sin exponer conversaciones privadas, credenciales o datos personales.

## Entrega

La respuesta final debe indicar archivos modificados, verificaciones realizadas, limitaciones y si el commit fue publicado o quedó solamente local.
