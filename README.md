# Open Lab - Fundación para la Democratización de la Inteligencia Artificial

Este repositorio contiene el blueprint operativo para un Open Lab de proyectos de inteligencia artificial impulsados por la Fundación y la comunidad Birria.

En esta primera etapa, el repositorio se crea, publica y mantiene desde la cuenta personal [`jcruzalmiron`](https://github.com/jcruzalmiron). La colaboración es abierta, pero la propiedad y continuidad del espacio permanecen en esa cuenta.

La propuesta no es crear un repositorio gigante donde se acumule código. Es construir una arquitectura repetible: cada proyecto real tiene su propio repositorio, comparte una plantilla común y aparece en un catálogo público central.

## BIRRIA EcoLabs

La primera propuesta desarrollada en este Open Lab es **BIRRIA EcoLabs: Laboratorios Comunitarios de Inteligencia Artificial para la Acción Climática Local**.

EcoLabs combina educación ambiental, participación ciudadana y uso responsable de IA para trabajar sobre lluvias intensas y anegamientos, separación de residuos, compostaje y comunicación ambiental comunitaria.

- Propuesta operativa completa: [`docs/birria-ecolabs.md`](docs/birria-ecolabs.md).
- Catálogo del proyecto: [`open-lab/README.md`](open-lab/README.md).
- Primer EcoLab para clonar: [`open-lab/birria-ecolabs/primer-ecolab/`](open-lab/birria-ecolabs/primer-ecolab/).
- Primer piloto: encuentro de Tecnoteca del 24 de septiembre de 2026, con grupos de nivel inicial, intermedio y avanzado.

El documento distingue los elementos confirmados en el formulario y la reunión de trabajo de las recomendaciones que todavía deben validar las comisiones de Tecnología y Eventos.

## Cómo empezar

Este es un repositorio de planificación, documentación y coordinación. En esta etapa no contiene una aplicación lista para ejecutar ni un único stack de software.

1. Leé este README y [`AGENTS.md`](AGENTS.md).
2. Revisá [`docs/birria-ecolabs.md`](docs/birria-ecolabs.md) si vas a trabajar sobre EcoLabs.
3. Consultá [`CONTRIBUTING.md`](CONTRIBUTING.md) y [`SECURITY.md`](SECURITY.md) antes de abrir cambios.
4. Usá Discussions para ideas y preguntas, e Issues para tareas concretas.
5. Si una idea alcanza un alcance claro, creá un repositorio derivado desde [`project-template/`](project-template/).

Los agentes de desarrollo tienen instrucciones adicionales en [`CODEX.md`](CODEX.md) y [`CLAUDE.md`](CLAUDE.md).

## Arquitectura

```text
fundacion-open-lab/
├── .github/                 # reglas generales, issues y PRs
├── AGENTS.md                # instrucciones comunes para agentes
├── CODEX.md                 # orientación para Codex
├── CLAUDE.md                # orientación para Claude Code
├── open-lab/                # catálogo público de proyectos
│   └── birria-ecolabs/      # primer EcoLab y sus tres proyectos iniciales
├── project-template/        # plantilla oficial para nuevos repos
├── docs/                    # arquitectura, operación, EcoLabs y políticas
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
└── CHANGELOG.md
```

## Principios

- Propiedad y continuidad: el repositorio pertenece y es mantenido por `jcruzalmiron`; una GitHub Organization institucional podrá evaluarse más adelante, pero no es un requisito actual.
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

Las líneas de proyectos del catálogo son propuestas de organización. Los repositorios derivados de esos proyectos todavía deben crearse y validarse por separado.

## Estado actual

El repositorio público ya está creado bajo `jcruzalmiron`. La base incluye el catálogo `open-lab`, la plantilla `project-template`, la propuesta completa de EcoLabs, documentación operativa y workflows iniciales de higiene y seguridad.

## Mantenimiento y continuidad

La cuenta `jcruzalmiron` crea y mantiene este Open Lab. Las propuestas y contribuciones se gestionan mediante Issues, Discussions y Pull Requests, con permisos explícitos para quienes colaboren. No se prevé transferir el repositorio a una organización institucional en esta etapa.
