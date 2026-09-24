# Instrucciones para agentes

## Propósito del repositorio

Este repositorio es el Open Lab público de la Fundación para la Democratización de la Inteligencia Artificial y la comunidad Birria. En esta etapa es principalmente un espacio de documentación, diseño de actividades, catálogo y plantillas reutilizables.

La primera línea de trabajo desarrollada en detalle es **BIRRIA EcoLabs: Laboratorios Comunitarios de Inteligencia Artificial para la Acción Climática Local**.

## Primeros archivos que leer

Antes de modificar algo, leer en este orden:

1. `README.md`
2. `docs/birria-ecolabs.md` si la tarea se relaciona con EcoLabs
3. `CONTRIBUTING.md`
4. `SECURITY.md`
5. `docs/trazabilidad-ia.md`
6. `CODEX.md` o `CLAUDE.md`, según el agente que esté trabajando

## Estado técnico actual

- No hay una aplicación ejecutable ni un stack único.
- No inventar comandos de instalación, servidores, APIs o tests que no existan.
- Los entregables actuales son Markdown, YAML, plantillas y workflows de GitHub Actions.
- `project-template/` es una plantilla para proyectos futuros; no asumir que sus carpetas vacías son código funcional.

## Mapa de trabajo

- `README.md`: entrada general y onboarding.
- `docs/birria-ecolabs.md`: propuesta operativa completa de EcoLabs, dinámica, piloto, riesgos y métricas.
- `open-lab/README.md`: catálogo explicado para personas.
- `open-lab/projects.yml`: catálogo estructurado.
- `project-template/`: estructura inicial para un repositorio derivado.
- `docs/arquitectura.md`: decisiones de arquitectura del Open Lab.
- `docs/operacion.md`: operación, Issues, Discussions, Projects y automatización.
- `docs/trazabilidad-ia.md`: registro de uso de IA.
- `.github/`: plantillas y validaciones automáticas.

## Cómo decidir dónde editar

- Cambios en el programa, la dinámica o el piloto de EcoLabs: `docs/birria-ecolabs.md`.
- Cambios en el listado de proyectos: `open-lab/projects.yml` y, si corresponde, `open-lab/README.md`.
- Cambios en la arquitectura general: `docs/arquitectura.md`.
- Cambios en normas de contribución o seguridad: `CONTRIBUTING.md` o `SECURITY.md`.
- Cambios en la estructura de proyectos futuros: `project-template/`.
- Cambios en la experiencia de un agente: `AGENTS.md`, `CODEX.md` y `CLAUDE.md`.

## Reglas de contenido

- Diferenciar hechos observados, decisiones tomadas, recomendaciones y pendientes.
- No convertir supuestos de una reunión en compromisos confirmados.
- No publicar nombres, DNI, domicilios, teléfonos, correos personales, datos de inscripción ni información privada de terceros.
- No publicar tokens, contraseñas, claves API, archivos `.env` ni logs sensibles.
- No presentar un prototipo de EcoLabs como alerta oficial, pronóstico, diagnóstico profesional o sistema de emergencia.
- Toda afirmación local debe tener una fuente, una fecha o una indicación explícita de que requiere validación.
- Si se utiliza IA, registrar herramienta, prompts relevantes, decisiones humanas, validaciones y limitaciones.

## Verificación mínima

Antes de entregar cambios:

```powershell
git status --short
git diff --check
```

Para cambios de documentación, revisar los enlaces relativos y comprobar que los bloques Markdown estén cerrados. Para cambios en workflows o YAML, validar la sintaxis disponible en el entorno y explicar cualquier validación que no haya sido posible ejecutar.

## Git y publicación

- Inspeccionar el estado antes de modificar o commitear.
- No incluir archivos ajenos, entregables locales, carpetas de render, temporales ni datos personales.
- Hacer cambios pequeños y con mensajes de commit específicos.
- No usar `reset --hard`, `force-push` ni borrar archivos sin autorización explícita.
- El repositorio central pertenece a la organización de GitHub `comunidad-birria`; `jcruzalmiron` es la persona administradora inicial.
- Un agente puede preparar un commit local; hacer `push` solo cuando la persona responsable lo haya solicitado.
