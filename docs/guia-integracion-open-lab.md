# Guía de integración y colaboración en el Open Lab

- **Versión:** 1.2
- **Actualizada:** 24 de septiembre de 2026
- **Estado:** guía operativa de referencia. Las propuestas que aún requieren aprobación se identifican como tales.
- **Repositorio central:** [`comunidad-birria/openlab`](https://github.com/comunidad-birria/openlab)

Esta guía explica cómo sumarse al Open Lab, elegir dónde trabajar, proponer cambios y mantener la documentación. El repositorio es público y colaborativo: cada aporte debe ser comprensible, revisable y seguro para que otra persona pueda continuarlo.

## 1. Qué es el Open Lab

El Open Lab es el espacio público de proyectos de inteligencia artificial impulsados por la Fundación y la comunidad Birria. En esta etapa funciona principalmente como catálogo, documentación, coordinación y plantilla para proyectos. No tiene una aplicación única ni un solo stack técnico.

La organización `comunidad-birria` mantiene el repositorio central. Las personas pueden participar mediante propuestas, Issues y Pull Requests; las personas mantenedoras revisan e incorporan los cambios. Los proyectos con código pueden tener repositorios propios y enlazarse desde el catálogo central.

La regla de trabajo es simple: una idea puede empezar en una conversación; una tarea concreta se registra; un cambio se propone con su documentación y se incorpora después de revisión.

## 2. Dónde participar

Usá cada espacio de GitHub para el tipo de colaboración que necesita el trabajo:

| Espacio | Para qué sirve | Ejemplo |
|---|---|---|
| Discussions | Preguntas, propuestas, decisiones abiertas y búsqueda de colaboradores. | Proponer un nuevo taller o debatir el alcance de un proyecto. |
| Issues | Trabajo concreto, errores, mejoras y documentación pendiente. | Corregir una guía o preparar un ejemplo verificable. |
| Pull Requests | Presentar cambios para revisión antes de incorporarlos a la rama principal. | Actualizar un README y adjuntar evidencia de revisión. |
| GitHub Projects | Función habilitada; tablero transversal recomendado, todavía pendiente de creación. | Idea, En desarrollo, Demo, Publicado, Mantenimiento, Archivado. |

### BIRRIA EcoLabs: ubicación de los tres niveles

| Nivel | Proyecto | Lugar de trabajo |
|---|---|---|
| Inicial / básico | Guía de residuos y compostaje, incluido Separá Bien Rosario. | El hub comparte la consigna sin enlazar la referencia preparada. Después: integrar al hub los resultados del grupo y el desarrollo de referencia revisado en [`01-guia-residuos/`](../open-lab/birria-ecolabs/primer-ecolab/01-guia-residuos/). Ya existe una implementación externa pública relacionada. |
| Intermedio | Campaña de comunicación ambiental comunitaria. | [`02-comunicacion-ambiental/`](../open-lab/birria-ecolabs/primer-ecolab/02-comunicacion-ambiental/). |
| Avanzado | Mapa comunitario de lluvias y anegamientos. | [`03-lluvias-anegamientos/`](../open-lab/birria-ecolabs/primer-ecolab/03-lluvias-anegamientos/). |

Para cuidar la exploración del grupo, el hub no enlaza una implementación resuelta, demo o respuesta modelo del nivel básico antes de la actividad. Sin embargo, al 24 de septiembre de 2026 ya existe una implementación externa pública relacionada: esta práctica reduce la exposición, pero no garantiza una exploración a ciegas. Si evitar cualquier referencia previa es indispensable, acordá una medida con quien mantiene ese repositorio o adaptá el desafío. Después de la actividad, los resultados revisados y el desarrollo de referencia del hub se pueden incorporar por separado, con procedencia, asistencia de IA, decisiones humanas y validaciones; una solución preexistente nunca se atribuye al grupo participante. Ver el análisis en [Referencias externas revisadas para EcoLabs](referencias-externas-ecolabs.md).

## 3. Primeros pasos

1. Leé el [`README.md`](../README.md) y [`AGENTS.md`](../AGENTS.md) para entender el propósito, el mapa de archivos y las reglas de trabajo.
2. Consultá [`CONTRIBUTING.md`](../CONTRIBUTING.md) y [`SECURITY.md`](../SECURITY.md) antes de proponer cambios.
3. Para EcoLabs, abrí la [propuesta operativa](birria-ecolabs.md) y el README del nivel correspondiente.
4. Definí un resultado pequeño y revisable. Si el alcance no está claro, conversalo en Discussions antes de desarrollar.
5. Usá una cuenta de GitHub protegida. Como buena práctica, activá autenticación de dos factores y mantené seguros los métodos de recuperación.

No hace falta saber programar para participar. Se puede contribuir con observaciones del territorio, revisión de lenguaje, fuentes, pruebas de comprensión, diseño, documentación o desarrollo técnico.

## 4. Flujo de contribución

1. **Acordá el alcance.** Para una idea nueva, iniciá una Discussion. Para una tarea concreta, abrí un Issue con el problema y el resultado esperado.
2. **Elegí el repositorio y la carpeta.** Trabajá en el proyecto correcto y evitá mezclar cambios de líneas distintas.
3. **Creá una rama o un fork.** No prepares el cambio directamente sobre `main`. Si no tenés permiso de escritura, usá un fork.
4. **Hacé un cambio enfocado.** Incluí solo los archivos necesarios y actualizá el Markdown que explica el resultado.
5. **Revisá antes de enviar.** Comprobá enlaces, seguridad, fuentes, uso de IA y qué pudiste validar.
6. **Abrí un Pull Request.** Explicá qué cambia, por qué, cómo revisarlo y qué queda pendiente. La persona mantenedora revisa el aporte antes de incorporarlo.

### Edición desde GitHub

Podés corregir o agregar un Markdown desde la web de GitHub con **Edit** o **Add file**. Elegí la opción para proponer el cambio en una rama o en un fork, revisá la vista previa y abrí un Pull Request. No publiques directamente en la rama principal.

### Edición con Git

Para contribuir al hub, primero creá un fork de `comunidad-birria/openlab` en GitHub. Reemplazá `USUARIO` por tu nombre de usuario de GitHub al clonar tu fork y creá una rama:

```bash
git clone https://github.com/USUARIO/openlab.git
cd openlab
git switch -c docs/descripcion-breve
```

Después de editar, revisá el estado y el formato, agregá solo los archivos del aporte, creá un commit y subí la rama a tu fork:

```bash
git status --short
git diff --check
git add ruta/al/archivo
git commit -m "docs: describe el aporte"
git push -u origin docs/descripcion-breve
```

Abrí el Pull Request hacia `comunidad-birria/openlab`, rama `main`. Si un proyecto se deriva más adelante a un repositorio propio, usá ese destino solo cuando la persona mantenedora lo confirme. Seguí los comandos de ejecución y pruebas que documenta el proyecto real; el Open Lab no tiene comandos universales de instalación o test.

## 5. Documentación que debe acompañar un cambio

Actualizá el `README.md` del proyecto cuando cambien su propósito, alcance, estado, forma de revisar o límites. Según el cambio, actualizá también:

- `docs/`: alcance, arquitectura, decisiones, fuentes o validación;
- `prompts/`: instrucciones reutilizables y despersonalizadas;
- `examples/`: ejemplos ficticios o anonimizados;
- `tests/`: checklist o casos de prueba realmente revisados;
- `open-lab/README.md` y `open-lab/projects.yml`: punto de entrada o información estructurada del catálogo;
- `docs/birria-ecolabs.md`: dinámica, alcance, productos o decisiones comunes del programa.

En la documentación, indicá el estado del proyecto, qué puede revisar una persona, fuentes y fechas, validaciones realizadas, limitaciones y siguiente paso. Usá estos rótulos cuando corresponda:

- **Confirmado:** consta en una fuente o fue acordado por quienes tienen responsabilidad sobre esa decisión.
- **Propuesta:** recomendación que todavía debe revisarse.
- **Pendiente de validación:** dato, permiso, fuente o decisión que aún falta confirmar.

No presentes como acuerdo una sugerencia de una reunión ni como probado un flujo que no ejecutaste. Para afirmaciones locales sobre Rosario, agregá fuente y fecha o marcá explícitamente qué falta validar.

## 6. Uso responsable y trazabilidad de IA

La IA puede ayudar a explorar, ordenar o redactar. La decisión y la responsabilidad del resultado siguen en las personas que contribuyen. Si usaste IA, completá en el README del proyecto una sección como esta:

```markdown
## Trazabilidad de IA

- Partes asistidas por IA:
- Herramientas o modelos utilizados:
- Prompts relevantes: ver `prompts/`
- Decisiones y correcciones humanas:
- Validaciones realizadas:
- Limitaciones conocidas:
```

Guardá solo prompts útiles y despersonalizados. No subas conversaciones privadas ni uses salidas de IA como fuente de verdad sin verificarlas. Consultá [`docs/trazabilidad-ia.md`](trazabilidad-ia.md) para el criterio completo.

## 7. Seguridad, privacidad y cuidado

El repositorio y sus Issues, Discussions y Pull Requests son públicos. No publiques:

- contraseñas, tokens, claves API, archivos `.env` ni archivos de secretos;
- DNI, domicilios, teléfonos, correos personales o datos de inscripción;
- datasets identificables o sensibles, logs privados o información contractual;
- imágenes, diseños, código o textos de terceros sin autorización o licencia compatible;
- carpetas locales de dependencias como `venv/`, `.venv/` o `node_modules/`.

Si encontrás una credencial expuesta, no la copies en un Issue o Pull Request. Avisá por un canal privado al equipo responsable. Revocá la clave solo si tenés autorización para hacerlo.

En EcoLabs, los ejemplos sobre residuos deben diferenciar información general de reglas locales y puntos de recepción confirmados. El prototipo de lluvias y anegamientos no es un pronóstico, una alerta oficial, un diagnóstico profesional ni un sistema de emergencia. Usá datos sintéticos o anonimizados y nunca publiques domicilios particulares.

## 8. Licencias, atribución y reutilización

Revisá la licencia del repositorio concreto antes de reutilizar o incorporar materiales. Que un archivo esté disponible en internet no significa que tengas permiso para copiarlo. Conservá la procedencia, autoría, fecha y condiciones de uso de datos, código, imágenes y documentos externos.

La propuesta de [`docs/licenciamiento.md`](licenciamiento.md) recomienda licencias para código y materiales, pero indica que la política debe ser ratificada. Por eso, no supongas que esa propuesta ya es la licencia aprobada de todos los proyectos. Si la licencia del material no está clara, dejalo fuera del repositorio hasta confirmar autorización.

## 9. Código de conducta y reconocimiento

Mantené una colaboración respetuosa, accesible y abierta a distintos niveles de experiencia. Aceptá preguntas y desacuerdos de buena fe, evitá acoso o discriminación y reconocé las contribuciones de otras personas. No uses el repositorio para exponer o perjudicar a alguien.

Para reportar una situación, usá un mecanismo privado disponible o contactá al equipo responsable. La referencia completa está en [`CODE_OF_CONDUCT.md`](../CODE_OF_CONDUCT.md).

## 10. Lista de revisión antes del Pull Request

- [ ] El cambio está en el repositorio y la carpeta correctos.
- [ ] Expliqué qué cambia y por qué.
- [ ] Actualicé el README o el documento que corresponde.
- [ ] Los enlaces relativos funcionan y la vista previa Markdown se entiende.
- [ ] Las afirmaciones locales tienen fuente y fecha, o están marcadas como pendientes.
- [ ] Registré herramientas de IA, decisiones humanas, validaciones y limitaciones.
- [ ] Revisé que no haya secretos, datos personales ni material sin permiso.
- [ ] Ejecuté las verificaciones disponibles o indiqué qué no pude probar.
- [ ] `git diff --check` no informa errores de formato.
- [ ] Otra persona puede entender el aporte sin depender de una explicación oral.

Para cambios solo de documentación, revisá el contenido, los enlaces y el formato. Para código, seguí la documentación del proyecto y describí evidencia reproducible. Los workflows automáticos ayudan, pero no reemplazan la revisión humana.

## 11. Documentos de referencia

- [`README.md`](../README.md): propósito y entrada general.
- [`AGENTS.md`](../AGENTS.md): reglas para agentes y mapa de edición.
- [`CONTRIBUTING.md`](../CONTRIBUTING.md): proceso de contribución y Pull Requests.
- [`SECURITY.md`](../SECURITY.md): datos y respuesta ante secretos.
- [`CODE_OF_CONDUCT.md`](../CODE_OF_CONDUCT.md): convivencia y reportes.
- [`docs/operacion.md`](operacion.md): Issues, Discussions, Projects y automatización.
- [`docs/trazabilidad-ia.md`](trazabilidad-ia.md): registro del uso de IA.
- [`docs/licenciamiento.md`](licenciamiento.md): propuesta de licencias y estado de ratificación.
- [`docs/guia-aportes-ecolabs.md`](guia-aportes-ecolabs.md): pasos específicos para los tres niveles del primer EcoLab.

La persona mantenedora puede orientar el destino de un aporte, pedir ajustes o dejarlo pendiente de validación. Ante una duda sobre seguridad, datos, licencias o alcance, consultá antes de publicar.
