# Arquitectura del Open Lab

## Decisión principal

El repositorio central está alojado en la organización de GitHub `comunidad-birria`, bajo el nombre [`comunidad-birria/openlab`](https://github.com/comunidad-birria/openlab). La organización conserva la continuidad del Open Lab aunque cambien las personas que colaboran.

La colaboración se organiza mediante Issues, Discussions, Projects y Pull Requests. La organización permite administrar accesos compartidos; cada proyecto puede definir sus responsables y permisos de acuerdo con su alcance.

La unidad de trabajo madura es el repositorio de proyecto. Para actividades iniciales como el primer EcoLab, las consignas y primeros aportes se agrupan en carpetas del hub para facilitar el acceso y la coordinación. El catálogo central presenta proyectos, estados, enlaces, áreas y formas de colaborar; cuando una línea madura, puede extraerse a un repositorio propio desde la plantilla.

## Capas

### Gobernanza del repositorio

Identidad, permisos, políticas, Discussions, Projects y workflows compartidos bajo la organización `comunidad-birria`. `jcruzalmiron` es administrador inicial; conviene sumar otras personas administradoras de confianza para asegurar continuidad.

### Catálogo

`open-lab` funciona como portada pública. Agrupa proyectos activos, experimentales y archivados, con una ficha breve y un enlace a su repositorio propio.

### Plantilla

`project-template` es el punto de partida oficial. Todo proyecto nacido en una actividad puede usarla para recibir README, licencia, estructura, issues, pull requests, prompts y workflows básicos.

### Proyectos

Los desarrollos que requieren un ciclo de vida autónomo pueden vivir en repositorios propios. Durante el piloto, el hub agrupa los tres desafíos del primer EcoLab; esta etapa acotada no convierte al catálogo en un monorepo de aplicaciones. La persona mantenedora decide la extracción cuando haya alcance, responsables y documentación suficientes.

## Ciclo de vida

```text
Idea -> En desarrollo -> Demo -> Publicado -> Mantenimiento -> Archivado
```

El estado debe aparecer en el catálogo y en el README de cada proyecto.
