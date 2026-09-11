---
name: auditoria-normativa
description: Revisa un borrador de documento técnico buscando afirmaciones normativas y verifica una a una contra los PDFs de normativa disponibles, devolviendo una tabla con estado VERIFICADO, DISCREPANCIA o NO VERIFICABLE. Úsala antes de cerrar cualquier memoria, informe o documento que se vaya a firmar.
---

# Auditoría de normativa

## Cuándo se usa

Antes de dar por cerrado cualquier documento que lleve firma. **Siempre en una
conversación nueva**, no en la misma donde se redactó: el revisor no puede ser el
que ha escrito, porque arrastra sus propias suposiciones.

## Procedimiento

1. Lee el borrador y localiza **toda** afirmación de carácter normativo: valores
   límite, dimensiones mínimas, exigencias, clasificaciones, referencias a
   artículos, plazos, condiciones de habitabilidad.
2. Verifica cada una contra los documentos de `normativa/`.
3. Devuelve una tabla:

   | # | Afirmación literal del borrador | Documento y artículo | Cita literal de la fuente | Estado |

   Estado solo puede ser uno de estos tres:
   - **VERIFICADO** — encontrada literalmente en un documento disponible.
   - **DISCREPANCIA** — encontrada y no coincide. Explica en qué.
   - **NO VERIFICABLE** — no está en los documentos disponibles. Di qué documento
     haría falta.
4. Ordena al final por riesgo: qué habría que revisar primero con 20 minutos.
5. Ofrece exportar la tabla a Excel con dos columnas vacías: «Comprobado por mí»
   y «Observaciones».

## Regla única

No apruebes nada por parecerte razonable o por conocerlo de otras fuentes. **Si
no está en los documentos disponibles, es NO VERIFICABLE. Sin excepciones.**

Tu trabajo aquí es encontrar errores, no validar. Un informe de auditoría sin
ningún hallazgo es sospechoso: revisa otra vez.
