# Guía de colaboración y actualización de BIRRIA EcoLabs

- **Para quién:** integrantes de Tecnología, Eventos y personas colaboradoras.
- **Uso inmediato:** preparar, registrar y continuar los aportes del encuentro de Tecnoteca del 24 de septiembre de 2026.
- **Repositorio central:** [`comunidad-birria/openlab`](https://github.com/comunidad-birria/openlab).

Esta guía explica dónde guardar cada aporte, cómo proponer cambios y qué documentación actualizar. Está pensada para que el trabajo pueda continuar después del encuentro y otra persona pueda entenderlo sin depender de quien lo creó.

Para las reglas generales del repositorio, licencias, seguridad y convivencia, consultá la [guía de integración y colaboración en el Open Lab](guia-integracion-open-lab.md). Este documento complementa esa guía con las rutas y entregables específicos del primer EcoLab.

## 1. Primero: elegí el espacio correcto

El Open Lab central conserva el catálogo, la propuesta común y los materiales de los tres niveles. Los tres proyectos iniciales forman parte del mismo primer EcoLab y, por ahora, sus fichas y aportes se organizan dentro del hub. No mezcles cambios de una línea con los materiales de las otras.

| Línea | Nivel | Dónde aportar | Producto de referencia |
|---|---|---|---|
| Guía de residuos y compostaje | Inicial / básico | [`01-guia-residuos/`](../open-lab/birria-ecolabs/primer-ecolab/01-guia-residuos/). Antes de la actividad, esta carpeta expone la consigna y materiales neutrales, no la implementación de referencia. | Guía de decisión y microcampaña; puede incluir el asistente de separación de residuos. |
| Comunicación ambiental comunitaria | Intermedio | [`02-comunicacion-ambiental/`](../open-lab/birria-ecolabs/primer-ecolab/02-comunicacion-ambiental/) | Kit breve de campaña adaptado a públicos y canales. |
| Lluvias intensas y anegamientos | Avanzado | [`03-lluvias-anegamientos/`](../open-lab/birria-ecolabs/primer-ecolab/03-lluvias-anegamientos/) | Matriz comunitaria y prototipo de mapa o croquis de riesgos. |
| Dinámica, alcance y acuerdos del programa | Transversal | [`docs/birria-ecolabs.md`](birria-ecolabs.md) | Propuesta operativa común y registro de decisiones. |

### Secuencia de publicación del nivel inicial

- **Antes del encuentro:** publicar la consigna, el problema, los criterios y las instrucciones de trabajo. No publicar ni enlazar la solución preparada previamente, una demo resuelta ni respuestas modelo que puedan orientar las decisiones del grupo.
- **Durante el encuentro:** guardar por separado el trabajo del grupo y cualquier material preexistente. No presentar la solución de referencia como resultado de las personas participantes.
- **Después del encuentro:** una vez cerrada la exploración y resguardados los aportes, integrar en `01-guia-residuos/` el trabajo del grupo y, en una sección claramente diferenciada, el desarrollo de referencia revisado. Registrar qué se preparó antes, qué aportó el grupo, qué asistencia de IA hubo y qué validaciones faltan.

Esta secuencia busca reducir el sesgo de anclaje, pero no garantiza una exploración a ciegas: al 24 de septiembre de 2026 existe un repositorio externo público con una implementación relacionada con el desafío inicial. No se enlaza en el QR ni en el material proyectado, aunque se puede encontrar por búsqueda. Si la ausencia total de exposición es requisito, la coordinación debe acordar una medida con quien mantiene ese repositorio antes del encuentro; no alcanza con ocultar una carpeta o rama en un repositorio público. Si no es posible, conviene explicitar el límite y registrar cualquier referencia previa que aparezca durante la actividad.

## 2. Flujo simple para aportar

1. Elegí una de las líneas de la tabla y revisá su `README.md`, ejemplos, prompts y checklist.
2. Acordá con el grupo qué resultado pequeño quieren dejar. Registrá una persona de contacto o responsable del cambio mediante su usuario de GitHub, si corresponde; no publiques datos de contacto personales.
3. Abrí un Issue si el cambio requiere trabajo posterior o tiene varias partes. Para una corrección puntual de documentación, podés proponer directamente un Pull Request.
4. Trabajá en una rama o en un fork. No edites directamente la rama principal.
5. Actualizá el Markdown junto con el desarrollo. No dejes una función, demo o material nuevo explicado solamente durante la presentación oral.
6. Revisá el cambio con la lista de publicación de esta guía y solicitá revisión de otra persona.
7. Abrí un Pull Request hacia el repositorio correspondiente. La persona mantenedora confirma el destino y aprueba la incorporación.

### Opción A: desde la web de GitHub

1. Abrí el archivo dentro del repositorio correcto.
2. Usá **Edit** para corregirlo o **Add file** para crear documentación nueva.
3. Elegí crear una rama para el cambio; si GitHub te pide hacer un fork, aceptalo.
4. Escribí un título y una descripción que expliquen qué problema resuelve el aporte.
5. Revisá la vista previa y los cambios línea por línea.
6. Creá el Pull Request hacia `main` del repositorio correcto.

### Opción B: con Git

Para contribuir al hub, primero creá un fork de `comunidad-birria/openlab` en GitHub. Después cloná tu fork y abrí una rama propia:

```bash
git clone https://github.com/<tu-usuario>/openlab.git
cd openlab
git switch -c docs/ecolabs-<tema>
```

Reemplazá `<tu-usuario>` y `<tema>` por tus datos; por ejemplo, `docs/ecolabs-residuos`. Al terminar:

```bash
git status --short
git diff --check
git add <archivos-del-aporte>
git commit -m "docs(ecolabs): actualiza <tema>"
git push -u origin docs/ecolabs-<tema>
```

Luego abrí un Pull Request desde tu rama hacia `comunidad-birria/openlab`, rama `main`. Si más adelante un proyecto se convierte en repositorio propio, la persona mantenedora confirmará el nuevo destino y actualizará el catálogo; hasta entonces, los tres niveles se trabajan en el hub.

## 3. Qué documentación actualizar

Actualizá primero el `README.md` de la línea donde trabajaste. Si agregaste material, código o datos de ejemplo, completá también el documento específico correspondiente:

- **Inicial:** [`01-guia-residuos/README.md`](../open-lab/birria-ecolabs/primer-ecolab/01-guia-residuos/README.md), `docs/alcance.md`, los ejemplos, prompts y checklist. Al publicar el material posterior a la actividad, separá explícitamente el resultado del grupo del desarrollo de referencia y documentá la procedencia de ambos.
- **Intermedio:** [`02-comunicacion-ambiental/README.md`](../open-lab/birria-ecolabs/primer-ecolab/02-comunicacion-ambiental/README.md), `docs/brief-campana.md`, `examples/kit-demo.md`, el prompt y el checklist.
- **Avanzado:** [`03-lluvias-anegamientos/README.md`](../open-lab/birria-ecolabs/primer-ecolab/03-lluvias-anegamientos/README.md), `docs/modelo-datos.md`, los ejemplos sintéticos, el prompt y el checklist.
- **Cambios al encuentro o al programa completo:** actualizá [`docs/birria-ecolabs.md`](birria-ecolabs.md), no solo el README del proyecto.
- **Cambio visible en el catálogo o en el punto de entrada:** actualizá también [`open-lab/README.md`](../open-lab/README.md) y, si cambia un dato estructurado del catálogo, [`open-lab/projects.yml`](../open-lab/projects.yml).

En cada Markdown que cambie, indicá con claridad:

- qué cambió y por qué;
- estado del material: idea, en desarrollo, demo, publicado, mantenimiento o archivado;
- cómo revisar o reproducir el resultado, usando comandos que realmente existan;
- fuentes y fechas para afirmaciones locales, o qué falta validar;
- limitaciones, riesgos y siguiente paso;
- qué parte se trabajó con IA y qué revisó o decidió el equipo.

Para el documento común, diferenciá siempre **confirmado**, **propuesta** y **pendiente de validación**. No conviertas una sugerencia del taller en un acuerdo institucional sin confirmación.

### Plantilla breve para registrar un aporte

Podés copiar este bloque en el `README.md` del proyecto o en el documento que corresponda:

```markdown
## Estado del aporte

- Estado: idea / en desarrollo / demo / publicado
- Actualizado: AAAA-MM-DD
- Cambio realizado:
- Cómo revisar o reproducirlo:
- Fuentes y fecha de consulta:
- Qué falta validar:
- Limitaciones conocidas:
- Próximo paso:
```

No agregues esta plantilla si la misma información ya está completa en una sección existente; editá la sección actual para evitar duplicaciones.

## 4. Trazabilidad de IA

Si usaste un modelo o una herramienta de IA generativa, completá en el README del proyecto la sección de trazabilidad. Indicá cuál eligió el grupo y registrá solo información necesaria y despersonalizada:

```markdown
## Trazabilidad de IA

- Partes asistidas por IA:
- Herramientas o modelos utilizados:
- Prompts relevantes: ver `prompts/`
- Decisiones y correcciones humanas:
- Validaciones realizadas:
- Limitaciones conocidas:
```

Guardá los prompts reutilizables en la carpeta `prompts/`. No publiques conversaciones privadas, nombres de participantes, datos de inscripción ni información sensible como contexto de un prompt.

## 5. Qué no subir

El repositorio es público. Antes de agregar archivos, verificá que no incluyan:

- contraseñas, tokens, claves API, `.env` ni archivos de secretos;
- datos personales, domicilios particulares, teléfonos, correos o planillas de inscripción;
- datasets sensibles, logs privados o información contractual;
- fotos, audios, diseños o textos de terceros sin autorización;
- carpetas de entorno o dependencias instaladas como `venv/`, `.venv/` o `node_modules/`.

Para residuos, no inventes puntos verdes, horarios ni reglas municipales: citá una fuente local y su fecha, o dejá el dato como pendiente. Para lluvias y anegamientos, usá ejemplos sintéticos o datos anonimizados; no publiques domicilios ni presentes el prototipo como pronóstico, alerta oficial o herramienta de emergencia.

Si encontrás una clave o dato sensible ya publicado, no lo copies a un Issue ni a un Pull Request. Avisá por un canal privado a la persona mantenedora para que se gestione la exposición.

## 6. Lista de revisión antes del Pull Request

- [ ] El aporte está en el repositorio y la carpeta del nivel correctos.
- [ ] El `README.md` describe el resultado y su estado actual.
- [ ] La documentación coincide con lo que realmente se puede probar o mostrar.
- [ ] Los enlaces relativos funcionan y la vista previa Markdown se lee bien.
- [ ] Las afirmaciones locales tienen fuente y fecha, o están marcadas para validar.
- [ ] Registré la asistencia de IA, las decisiones humanas y las limitaciones.
- [ ] Eliminé datos personales, credenciales, archivos sensibles y dependencias locales.
- [ ] Probé el flujo disponible o expliqué qué no pude verificar.
- [ ] `git diff --check` no informa errores de formato.
- [ ] Otra persona revisó el contenido antes de pedir que se incorpore.

En este repositorio no hay un único stack ni una suite universal de pruebas. Para cambios de documentación, la revisión de contenido, enlaces y formato es suficiente. Para código, seguí las instrucciones reales del proyecto correspondiente y no declares como probado algo que no ejecutaste.

## 7. Para cerrar el trabajo de mañana

Cada grupo debería poder compartir, como mínimo:

1. el nivel y el problema que eligió;
2. un enlace al archivo o demo que produjo;
3. el `README.md` actualizado con estado, alcance y próximo paso;
4. fuentes, supuestos y validaciones pendientes;
5. la trazabilidad de IA y las decisiones humanas;
6. un Issue o tarea concreta para continuar.

La meta del encuentro es dejar aportes preparados, comprensibles y continuables. No hace falta presentar una aplicación terminada ni publicar un cambio sin revisión.
