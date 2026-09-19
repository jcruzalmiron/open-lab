# Trazabilidad de inteligencia artificial

La trazabilidad de IA es una práctica central del Open Lab. No busca esconder que se usó IA, sino hacer visible cómo se usó y dónde intervino el criterio humano.

## Bloque mínimo para cada proyecto

Cada README debería incluir una sección como esta:

```markdown
## Trazabilidad de IA

- Partes asistidas por IA: [describir]
- Herramientas o modelos utilizados: [describir]
- Prompts relevantes: ver `prompts/`
- Decisiones humanas: [describir qué se definió o corrigió manualmente]
- Validaciones realizadas: [tests, revisión experta, prueba comunitaria, etc.]
- Limitaciones conocidas: [describir]
```

## Qué guardar

- Prompts reutilizables y suficientemente despersonalizados.
- Versiones o fechas de las herramientas cuando sean relevantes.
- Decisiones humanas que cambiaron una propuesta generada por IA.
- Evidencia de revisión y validación.

## Qué no guardar

- Datos personales usados como contexto.
- Tokens, claves, conversaciones privadas o archivos confidenciales.
- Prompts que expongan información contractual o sensible.
