# Arquitectura del Open Lab

## Decisión principal

La Fundación debería operar una GitHub Organization institucional, no una colección de repositorios pertenecientes a integrantes individuales.

La unidad de trabajo es el repositorio de proyecto. El catálogo central no contiene todo el código: presenta los proyectos, sus estados, enlaces, áreas y formas de colaborar.

## Capas

### Organización

Identidad, permisos, equipos, políticas, Discussions, Projects y workflows compartidos.

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
