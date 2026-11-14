<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/branding/claude-code-skills-logo-dark.png">
    <img src="assets/branding/claude-code-skills-logo.png" alt="Claude Code Skills" width="420">
  </picture>
</h1>

<p align="center">
  Colección personal de skills para Claude Code.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue" alt="License: MIT"></a>
</p>

## Descripción

Una skill es una carpeta con un archivo `SKILL.md` que enseña a Claude Code a realizar una tarea concreta. Claude Code la carga cuando la tarea coincide con la descripción de la skill.

Este repositorio reúne las skills que uso en mis proyectos: algunas escritas por otros autores y otras escritas por mí.

## Estructura

```
claude-code-skills/
├── assets/branding/    # Logo
├── third-party/        # Skills de otros autores
├── custom/             # Skills escritas por mí
├── LICENSE
└── README.md
```

Cada skill vive en su propia carpeta:

```
nombre-de-la-skill/
├── SKILL.md            # Instrucciones (obligatorio)
└── ...                 # Archivos de apoyo que usa la skill (opcional)
```

## Skills

### De terceros

| Skill | Descripción |
|---|---|
| `grill-me` | Te interroga hasta que tu plan no tiene fallos |
| `to-prd` | Convierte una conversación en un documento de requisitos |
| `to-issues` | Convierte un plan en issues de GitHub |
| `tdd` | Desarrollo guiado por tests |
| `triage-issue` | Encuentra la causa raíz de un bug |
| `git-guardrails-claude-code` | Bloquea comandos git peligrosos |
| `write-a-skill` | Crea nuevas skills con la estructura correcta |
| `setup-pre-commit` | Configura hooks de pre-commit en Git |
| `improve-codebase-architecture` | Busca mejoras en la arquitectura de un proyecto existente |
| `request-refactor-plan` | Crea un plan de refactorización con commits pequeños |

### Propias

| Skill | Descripción |
|---|---|
| `conventional-commit` | Escribe mensajes de commit en inglés siguiendo Conventional Commits |
| `pr-description` | Escribe títulos y descripciones de Pull Requests |
| `english-review` | Revisa inglés técnico y explica cada corrección en español |
| `prompt-engineer` | Diseña y mejora prompts para modelos de IA |
| `ai-api-integrator` | Integra las APIs de OpenAI, Anthropic o Gemini |
| `agent-builder` | Crea agentes autónomos que ejecutan tareas |
| `jarvis-memory` | Gestiona memoria persistente para un asistente personal |

## Instalación

Copia la carpeta de la skill que quieras en una de estas ubicaciones:

- `.claude/skills/` dentro de un proyecto, para usarla solo en ese proyecto.
- `~/.claude/skills/`, para usarla en todos los proyectos.

## Agradecimientos

Las skills de `third-party/` proceden de [mattpocock/skills](https://github.com/mattpocock/skills). El mérito es del autor original.

## Aviso

Proyecto personal, sin relación con Anthropic. Claude y Claude Code son marcas de sus respectivos propietarios.

## Autor

Pablo Ubieto Foncillas ([@PabloUbieto](https://github.com/PabloUbieto)).

## Licencia

El contenido original de este repositorio se publica bajo la [licencia MIT](LICENSE). Las skills de `third-party/` mantienen la licencia de su autor original.
