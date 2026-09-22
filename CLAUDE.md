# Instrucciones para Claude Code

Seguí primero [`AGENTS.md`](AGENTS.md), que contiene las reglas comunes del repositorio.

## Alcance

El repositorio es un Open Lab público y documentation-first. La línea principal actual es BIRRIA EcoLabs, una propuesta de laboratorios comunitarios de IA para acción climática local.

## Antes de trabajar

- Leer `README.md`, `AGENTS.md`, `CONTRIBUTING.md` y `SECURITY.md`.
- Leer `docs/birria-ecolabs.md` para tareas de EcoLabs.
- Revisar `git status --short`.
- Preservar archivos no relacionados y no incluir carpetas locales de entregables o temporales.

## Criterios para EcoLabs

- No inventar datos sobre Rosario, puntos de recepción, riesgos, alertas ni fuentes municipales.
- Diferenciar observaciones comunitarias, supuestos y datos oficiales.
- Mantener tres niveles de participación y un producto mínimo por mesa.
- Priorizar guías, matrices, prompts, prototipos y documentación reproducible.
- Aplicar revisión humana antes de cualquier publicación.
- No guardar PII, secretos, credenciales ni información privada en el repositorio.

## Verificación y Git

Ejecutar como mínimo:

```powershell
git diff --check
git status --short
```

Usar commits pequeños y descriptivos. No hacer `reset --hard`, `force-push` ni borrados destructivos. Hacer push solamente cuando la persona responsable lo solicite explícitamente.
