# Estudio · kit de trabajo con Claude Code

Esto es el estudio digital que montamos en el taller, en forma de carpeta.

Lo que en la web era «el Proyecto con sus instrucciones y su conocimiento», aquí
es una carpeta que puedes versionar, copiar a otro ordenador y mejorar con el
tiempo. Claude Code lee todo esto solo al arrancar dentro de la carpeta.

## Puesta en marcha (una vez)

```bash
git clone ⟨URL DEL REPO⟩ estudio-claude
cd estudio-claude
claude
```

Y dentro de Claude Code, la primera vez:

```
Lee el README y el CLAUDE.md. Luego ayúdame a crear mi CLAUDE.local.md
preguntándome mis datos: nombre, colegio, municipios donde trabajo,
y mis manías de redacción.
```

## Qué hay aquí

| Carpeta | Qué es |
|---|---|
| `CLAUDE.md` | Las reglas del estudio. Se aplican solas en cada conversación. **No lo edites**: se actualiza con `git pull`. |
| `CLAUDE.local.md` | Tus datos y tus manías. Solo tuyo, no se sube. |
| `.claude/skills/` | Los tres procedimientos del taller: ficha de encargo, memoria, auditoría. |
| `estilo/` | Tu guía de estilo, sacada de tus memorias antiguas. |
| `normativa/` | Tus PDFs de CTE, ordenanzas y autonómica. No se suben al repo. |
| `plantillas/` | Estructuras base de ficha e índice de memoria. |
| `encargos/` | Una carpeta por encargo. No se suben al repo. |

## Actualizar cuando yo mejore el kit

```bash
git pull
```

Nunca da conflictos: todo lo tuyo (`CLAUDE.local.md`, `encargos/`, `normativa/`,
tu guía de estilo) está fuera del control de versiones a propósito.

## Lo que no cambia

La IA redacta, tú firmas. Ninguna cita normativa sin el documento delante.
