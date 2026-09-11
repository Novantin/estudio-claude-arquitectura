---
name: memoria-descriptiva
description: Redacta memorias descriptivas y constructivas de proyecto de edificación siguiendo la estructura del Anejo I del CTE, a partir de la ficha de encargo y la normativa disponible. Úsala para redactar, ampliar o revisar una memoria de proyecto, un anejo o un apartado de cumplimiento normativo.
---

# Memoria descriptiva de proyecto

## Antes de empezar

1. **Ficha de encargo.** Si no existe, usa primero la skill `ficha-encargo`.
2. **Normativa aplicable disponible** en `normativa/` o adjunta. Sin los
   documentos delante no se redacta ningún apartado de cumplimiento.
3. **Índice aprobado.** Se propone, el arquitecto lo corrige, y solo entonces se
   redacta.

## Procedimiento

1. Propón el índice adaptado a este encargo, partiendo de
   `plantillas/INDICE-MEMORIA.md`. Marca los apartados que no aplican y explica
   por qué se quitan. **No redactes contenido en este paso.**
2. Espera la corrección del índice.
3. Redacta **apartado por apartado**, nunca el documento entero de una vez.
   Cadencia recomendada: agentes → información previa → descripción del proyecto
   → prestaciones → cumplimiento del CTE → resto.
4. Cierra cada apartado con el bloque `PENDIENTE DE VERIFICAR`.
5. Cuando el borrador esté completo, genera el `.docx` en la carpeta del encargo:
   estilos reales Título 1/2/3, índice automático, numeración de páginas, tablas
   como tablas, y las marcas `[VERIFICAR]` y `[DATO]` resaltadas en amarillo.
6. Recomienda la auditoría (`auditoria-normativa`) antes de dar nada por cerrado.

## Reglas que no se saltan

- Ninguna cita normativa sin documento disponible. Documento, artículo, tabla y
  cita literal. Si no está: `[VERIFICAR: falta X]`.
- Ningún dato de obra inventado. Si falta: `[DATO: qué falta]`.
- No estimar, no aproximar, no poner "valores habituales", no disimular un hueco
  con una frase vaga.

## Estructura de referencia (Anejo I del CTE)

1. Memoria descriptiva — agentes, información previa, descripción del proyecto,
   prestaciones del edificio.
2. Memoria constructiva — sustentación, sistema estructural, envolvente,
   compartimentación, acabados, acondicionamiento e instalaciones, equipamiento.
3. Cumplimiento del CTE — DB por DB, solo los que apliquen.
4. Cumplimiento de otros reglamentos y disposiciones.
5. Anejos.
