# Referencias externas revisadas para BIRRIA EcoLabs

**Revisión:** 24 de septiembre de 2026
**Uso:** insumo para coordinación y diseño; no implica alianza, aval ni validación técnica de BIRRIA.

Esta nota distingue lo observado en recursos públicos de las recomendaciones para el primer EcoLab. Las páginas pueden cambiar; las afirmaciones siguientes describen lo que mostraban al revisarlas, no una auditoría del código, los datos o su operación.

## Recursos observados

### Cota · riesgo hídrico de Rosario

- **Recurso compartido:** [demo web de Cota](https://piano-parents-quantitative-link.trycloudflare.com/).
- **Qué mostraba:** un panel de riesgo hídrico para Rosario. Su sección explicativa describía la combinación de nivel/tendencia del Paraná, pronóstico de precipitación, caudal modelado y capas o mapas locales.
- **Fuentes que declara la propia demo:** INA, Open-Meteo, GloFAS y datos/mapas de Rosario. Esta revisión no comprobó la actualización, licencia, calidad ni integración de esas fuentes.
- **Límites observados:** los valores del panel son dinámicos; no deben copiarse como evidencia estable. La demo se presentó como orientativa, no como alerta oficial, y la dirección `trycloudflare.com` es temporal.
- **Relación con EcoLabs:** referencia para conversar sobre visualización y límites del desafío de lluvias/anegamientos, que continúa siendo el nivel de complejidad más alto. No es una herramienta oficial de EcoLabs ni debe usarse para decidir acciones de emergencia.

### Eco-Labs---Chatbot · residuos y compostaje

- **Repositorio:** [Foraxo/Eco-Labs---Chatbot](https://github.com/Foraxo/Eco-Labs---Chatbot).
- **Qué describe su README:** un chatbot sobre residuos y compostaje, junto con un inspector de solicitudes a Gemini y sus costos; la página revisada mostraba una aplicación React/Vite y un servidor Express.
- **Relación con EcoLabs:** antecedente temático del nivel inicial. No corresponde al nivel intermedio, cuyo desafío acordado es diseñar una campaña de comunicación ambiental comunitaria.
- **Licencia y reutilización:** en la página revisada no se identificó un archivo `LICENSE` visible. No copiar ni redistribuir su código hasta confirmar con la persona mantenedora una licencia que lo permita.

### Separá Bien Rosario · implementación pública del desafío inicial

- **Estado observado:** el repositorio compartido por el equipo bajo `andreassale/EcoLabs_inicial` era público y su README describía un asistente de separación de residuos/compostaje con Streamlit, Python, Gemini y materiales de datos/prompts. En la página revisada figuraba Apache-2.0.
- **Implicancia para la dinámica:** ya hay una implementación relacionada disponible antes del encuentro. No enlazarla en el QR, la convocatoria ni las diapositivas reduce la exposición, pero no garantiza que los grupos no la encuentren por búsqueda o por otros medios.
- **Límite de autoridad:** este trabajo no cambia permisos ni contenido del repositorio de otra persona. Si el ejercicio requiere evitar toda referencia previa, la coordinación debe acordar una medida temporal con quien lo mantiene o elegir/adaptar una consigna. Si el repositorio sigue público, registrar con transparencia cualquier influencia previa y mantener separados el desarrollo preexistente y el trabajo del grupo.

## Herramientas y modelo de trabajo

| Capa | Estado | Uso propuesto |
|---|---|---|
| PCs de Tecnoteca y modelos de IA a elección | Aclaración de coordinación del 24 de septiembre | Hay PCs disponibles. Cada grupo elige el modelo según sus preferencias y la disponibilidad de acceso; no se requiere computadora personal. Confirmar cantidad de puestos y conectividad. |
| Documentos o planilla compartida | Recomendación práctica, sujeta a disponibilidad | Capturar decisiones, fuentes, supuestos y aportes del grupo sin exigir programación. |
| Mapa o herramienta visual | Opcional, según el nivel y el acceso | Representar observaciones generales; para lluvias, usar datos sintéticos o anonimizados al preparar el prototipo. |
| GitHub Issues, Discussions, Pull Requests y Projects | Habilitados en `comunidad-birria/openlab` al 24 de septiembre de 2026 | Separar tareas concretas, conversación, revisión de cambios y seguimiento del ciclo de vida. |
| GitHub Actions | Parcialmente presente en el repositorio central | Los workflows actuales comprueban archivos requeridos y buscan secretos. No ejecutan pruebas de una aplicación EcoLabs ni validan fuentes, datos o alertas. |

No hay un modelo de IA ni un stack único obligatorio, y no hace falta llegar con una aplicación terminada. Para el nivel alto, empezar por el esquema de datos, criterios explicables, un croquis y casos límite antes de integrar fuentes o desarrollar un mapa operativo.

## Decisiones de comunicación

- Mantener el QR y los enlaces proyectados apuntando al hub neutral del primer EcoLab, no a soluciones de referencia.
- Presentar los niveles como complejidad de los productos —inicial: guía de residuos; intermedio: campaña ambiental; alto: mapa comunitario de lluvias/anegamientos—, no como categorías de capacidad personal.
- Llamar a Cota y al chatbot “referencias externas revisadas”, nunca “herramientas oficiales”, “soluciones validadas” ni proyectos propios de BIRRIA.
- Después del encuentro, identificar por separado los materiales preexistentes, los aportes del grupo, la asistencia de IA, las decisiones humanas y las validaciones pendientes.
