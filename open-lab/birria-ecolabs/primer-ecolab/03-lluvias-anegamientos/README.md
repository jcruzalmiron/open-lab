# 03 - Lluvias intensas y anegamientos

**Nivel:** alto
**Estado:** preparado para prototipo
**Producto:** matriz comunitaria de riesgos y prototipo de mapa

## Propósito

Organizar observaciones territoriales sobre lluvias intensas y anegamientos para reconocer patrones, explicitar incertidumbres y pensar acciones comunitarias de bajo riesgo.

Este es el nivel alto porque combina datos territoriales, criterios de priorización, fuentes con distinta confiabilidad, incertidumbre temporal y una mayor responsabilidad sobre cómo se comunica el resultado.

## Alcance del primer prototipo

El equipo trabajará con datos ficticios o anonimizados y construirá:

- un esquema de datos;
- una matriz de priorización;
- un croquis o especificación de mapa;
- microacciones asociadas a cada prioridad;
- casos de prueba;
- límites visibles y derivaciones a organismos oficiales.

El prototipo no será una alerta oficial, un pronóstico meteorológico ni un diagnóstico de infraestructura.

## Dinámica de 150 minutos

| Tiempo | Etapa | Resultado |
|---|---|---|
| 0-20 min | Definir territorio y usuario | Alcance acotado, destinatario y producto mínimo. |
| 20-45 min | Estructurar observaciones | Tabla común con procedencia y fecha. |
| 45-75 min | Explorar patrones | Agrupaciones asistidas por IA y revisión humana. |
| 75-105 min | Priorizar | Criterios explícitos de severidad, recurrencia e impacto. |
| 105-130 min | Diseñar salida | Croquis, mapa conceptual o especificación de dashboard. |
| 130-145 min | Probar límites | Casos ambiguos, errores y situaciones de derivación. |
| 145-150 min | Presentar | Hallazgo, producto, límite y siguiente paso. |

## Esquema mínimo de datos

| Campo | Tipo | Regla |
|---|---|---|
| `zona_referencia` | texto | Usar referencia general, nunca domicilio particular. |
| `situacion_observada` | texto | Mantener el relato original y no convertirlo en dato oficial. |
| `fecha_observacion` | fecha | Registrar cuándo se observó. |
| `fuente_tipo` | categoría | Relato, observación, dato abierto u organismo. |
| `frecuencia_percibida` | categoría | Ocasional, frecuente o recurrente. |
| `impacto_observado` | categoría | Movilidad, acceso, escuela, comercio u otro. |
| `prioridad` | categoría | Baja, media o alta, con criterio documentado. |
| `accion_posible` | texto | Acción comunitaria de bajo riesgo o derivación. |
| `validacion_pendiente` | texto | Qué debería revisar una fuente competente. |

## Modelo de priorización para el taller

Usar una escala cualitativa, no una falsa precisión:

- **Baja:** observación aislada, impacto acotado y acción comunitaria simple.
- **Media:** patrón repetido o impacto relevante que requiere coordinación.
- **Alta:** situación recurrente, impacto significativo o necesidad de derivación urgente a un organismo competente.

La etiqueta no constituye una alerta. El equipo debe explicar por qué asignó cada prioridad y qué información falta.

## Entregables

- tabla documentada y anonimizada;
- criterios de priorización;
- mapa conceptual o especificación de visualización;
- tres microacciones posibles;
- casos de prueba claros, ambiguos y riesgosos;
- prompt de análisis;
- registro de errores y limitaciones;
- issue de continuidad técnica.

## Criterios de calidad

- Las observaciones conservan su fuente y fecha.
- El grupo diferencia testimonio, dato abierto y dato oficial.
- No se publican ubicaciones sensibles.
- La priorización es explicable.
- La salida no parece una alerta oficial.
- El prototipo puede ser continuado por otra persona.

## Siguiente paso

Conseguir un conjunto de datos público y autorizado, definir un esquema de actualización y validar los criterios con personas conocedoras del territorio y organismos competentes.
