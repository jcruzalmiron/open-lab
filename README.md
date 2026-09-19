# Open Lab - Fundación para la Democratización de la Inteligencia Artificial

Este repositorio contiene el blueprint operativo para una organización abierta de proyectos de inteligencia artificial impulsados por la Fundación y la comunidad Birria.

La propuesta no es crear un repositorio gigante donde se acumule código. Es construir una arquitectura repetible: cada proyecto real tiene su propio repositorio, comparte una plantilla común y aparece en un catálogo público central.

## Arquitectura

```text
fundacion-open-lab/
├── .github/                 # reglas generales, issues y PRs
├── open-lab/                # catálogo público de proyectos
├── project-template/        # plantilla oficial para nuevos repos
├── docs/                    # arquitectura, operación y políticas
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
└── CHANGELOG.md
```

## Principios

- GitHub Organization institucional: los repositorios pertenecen a la Fundación, no a personas particulares.
- Open source por defecto, no indiscriminadamente.
- Credenciales, datos personales, datasets sensibles e información contractual privada nunca se publican.
- Cada proyecto debe tener un README orientado a personas, una licencia clara y un estado visible.
- Issues sirven para trabajo concreto; Discussions para propuestas, preguntas y búsqueda de colaboradores.
- GitHub Projects permite seguir el ciclo Idea -> En desarrollo -> Demo -> Publicado -> Mantenimiento -> Archivado.
- La trazabilidad de IA es parte del producto: herramientas, modelos, prompts relevantes y decisiones humanas deben quedar registrados.

## Primeros repositorios sugeridos

- `open-lab`: catálogo y puerta de entrada pública.
- `project-template`: plantilla oficial para usar en talleres, hackatones y actividades.
- `evento-tecnoteca-2026`: materiales y resultados del encuentro de BIRRIA EcoLabs.
- `agente-ia-educacion`: proyecto educativo, si se confirma como línea de trabajo.
- `taller-n8n-agentes`: automatizaciones y agentes para experimentar.
- `datasets-abiertos`: datasets publicados con licencia y procedencia documentadas.

Los nombres de proyectos son propuestas de organización, no repositorios publicados todavía.

## Estado actual

Este workspace contiene el andamiaje local. Todavía no crea una GitHub Organization, no publica repositorios y no configura accesos externos.

## Próximo paso institucional

Crear la organización de GitHub de la Fundación, activar Discussions y Projects, definir los equipos con permisos mínimos y luego crear `open-lab` y `project-template` desde esta base.
