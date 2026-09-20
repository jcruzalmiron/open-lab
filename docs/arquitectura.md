# Arquitectura del Open Lab

## Decisión principal

El repositorio inicial se crea, publica y mantiene bajo la cuenta personal `jcruzalmiron`. Esta decisión permite validar el modelo Open Lab con continuidad y control claros, sin depender de una organización institucional en esta etapa.

La colaboración permanece abierta mediante Issues, Discussions y Pull Requests. Si más adelante la Fundación necesita equipos, permisos centralizados o facturación institucional, podrá evaluarse una GitHub Organization; no forma parte de la implementación actual.

La unidad de trabajo es el repositorio de proyecto. El catálogo central no contiene todo el código: presenta los proyectos, sus estados, enlaces, áreas y formas de colaborar.

## Capas

### Gobernanza del repositorio

Identidad, permisos, políticas, Discussions, Projects y workflows compartidos bajo la cuenta propietaria `jcruzalmiron`.

### Catálogo

`open-lab` funciona como portada pública. Agrupa proyectos activos, experimentales y archivados, con una ficha breve y un enlace a su repositorio propio.

### Plantilla

`project-template` es el punto de partida oficial. Todo proyecto nacido en una actividad puede usarla para recibir README, licencia, estructura, issues, pull requests, prompts y workflows básicos.

### Proyectos

Cada desarrollo real vive en su propio repositorio. Esto evita que el catálogo se convierta en un monorepo difícil de entender y facilita que cada iniciativa tenga su ciclo de vida.

## Ciclo de vida

```text
Idea -> En desarrollo -> Demo -> Publicado -> Mantenimiento -> Archivado
```

El estado debe aparecer en el catálogo y en el README de cada proyecto.
