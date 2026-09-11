---
description: Para el formador — captura lo aprendido en la sesión, escribe la bitácora y publica
---

Cierre de una sesión de taller. Vas a capturar lo que ha salido hoy y a dejarlo
publicado para que el alumno lo reciba con un `git pull`.

## 1. Pregúntame qué ha salido hoy

De una en una:

- ¿Qué prompt o procedimiento ha funcionado hoy y no estaba en el kit?
- ¿Qué se ha atascado, y qué regla habría que añadir para que no vuelva a pasar?
- ¿Alguna plantilla nueva, o alguna que haya que corregir?
- ¿Hay que tocar alguna de las tres skills?

## 2. Aplícalo al repo

Escribe los cambios donde toquen: `CLAUDE.md` para reglas, `.claude/skills/` para
procedimientos, `plantillas/` para estructuras, `.claude/commands/` para atajos.

Cambios pequeños y concretos. No reescribas archivos enteros para retocar una
frase.

## 3. Bitácora

Añade una entrada nueva **arriba** en `BITACORA.md`, con la fecha de hoy y tres o
cuatro líneas en lenguaje llano: qué ha entrado y qué cambia para quien lo use.
Está escrita para el alumno, no para mí.

## 4. Comprobación antes de publicar

Ejecuta `git status` y **enséñame la lista de archivos**. Comprueba que no se
cuela nada de esto:

- `CLAUDE.local.md`
- nada de `encargos/`
- nada de `normativa/`
- `estilo/GUIA-DE-ESTILO.md`
- ningún dato de cliente dentro de un archivo que sí se sube

Si aparece alguno, **para y avísame**. No lo añadas al `.gitignore` por tu cuenta.

## 5. Publica

Commit con un mensaje que diga qué cambia y por qué, y `git push`.

Luego dame, listo para copiar, el mensaje de WhatsApp para el alumno: una frase
diciendo que hay novedades y que escriba `/actualizar` en Claude Code.
