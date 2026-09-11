# Caso práctico: tu primera memoria de verdad

El encargo real del que hablaste en el taller: el edificio de dos alturas en
esquina, adaptación al Plan General, presillado de pilares, nueva entrada,
ventanas Cortizo y las 54 placas.

Tienes toda esa información en un Word. Vamos a convertirla en el sistema, y
después en la memoria.

## Antes de empezar, dos minutos

Crea una carpeta dentro de `encargos/` con la referencia del expediente, y
dentro de ella una carpeta `entrada/`. Mete ahí:

- El Word con los datos de la obra, tal cual, sin tocarlo.
- Tus planos del estado actual y del reformado, en PDF.
- Las imágenes de catálogo de la carpintería: la serie de Cortizo, las puertas.
- Los documentos básicos del CTE que apliquen a este proyecto. **Solo los que
  apliquen.**

Desordenado está bien. Es el punto de partida normal.

## Paso 1 · Partir el Word en dos

Abre Claude Code en esta carpeta y pega esto:

```
Tengo en encargos/⟨tu carpeta⟩/entrada/ un Word con toda la información de una
obra, mezclada con instrucciones de redacción y con condicionantes marcados por
colores.

Sepáralo en dos archivos, sin inventar ni completar nada:

1. INFORMACION-OBRA.md en la carpeta del encargo, siguiendo la estructura de
   plantillas/INFORMACION-OBRA.md. Solo datos de esta obra.

2. Lo que sean instrucciones de redacción —el "actúa como...", las reglas, la
   estructura que pido— no lo copies a ningún sitio todavía: enséñamelo en
   pantalla y dime si ya está cubierto por las reglas de CLAUDE.md o si hay algo
   que merezca añadirse.

Los condicionantes que vengan en color, pásalos a etiquetas CONDICIÓN:,
RESTRICCIÓN: o PENDIENTE:, porque los colores se pierden en texto plano. Si no
puedes saber qué significaba un color, pregúntamelo.

Las imágenes de catálogo déjalas donde están y referéncialas por nombre desde
la tabla de carpintería.

Todo dato que no esté en el Word, márcalo [DATO: qué falta]. No lo rellenes.
```

**Por qué se parte en dos:** las instrucciones son las mismas para todos tus
encargos y ya viven en `CLAUDE.md`. Los datos cambian con cada obra. Si los
mantienes mezclados, cada encargo nuevo te obliga a reescribir las reglas.

## Paso 2 · Revisar la ficha

Léete el `INFORMACION-OBRA.md` que ha salido. Busca los `[DATO]` y rellena los
que sepas. Los que no, déjalos: son la lista de lo que te falta por decidir, y
ese es su valor.

## Paso 3 · El índice

```
Con INFORMACION-OBRA.md y los DB del CTE de entrada/, usa la skill
memoria-descriptiva y propón el índice de la memoria adaptado a este encargo.

Marca los apartados que no apliquen y di por qué los quitas. En este proyecto no
se actúa sobre la cimentación, así que empieza por ahí.

No redactes contenido todavía.
```

Corrígelo a mano. Cinco minutos aquí te ahorran una hora después.

## Paso 4 · Redactar

```
Redacta el apartado ⟨1.1 Agentes⟩. Al final, la lista de PENDIENTE DE VERIFICAR.
```

Y vas subiendo por el índice. Empieza por los apartados cortos y mecánicos
—agentes, información previa— para ver cómo escribe antes de meterte en
cumplimiento del CTE, que es el delicado.

**Ve mirando los créditos** en Ajustes → Facturación y uso mientras lo haces. La
primera vez es la única forma de saber lo que te cuesta una memoria.

## Paso 5 · El Word

```
Genera el .docx con todo lo redactado: estilos reales Título 1/2/3, índice
automático, numeración de páginas, ⟨tu tipografía⟩ a ⟨tu tamaño⟩, tablas como
tablas, y las marcas [VERIFICAR] y [DATO] resaltadas en amarillo.
```

Ábrelo en Word. **Ese es el momento de la verdad**: si puedes editarlo,
corregirlo y aplicarle tu plantilla, el sistema funciona.

## Paso 6 · La auditoría

Conversación nueva. El que ha escrito no puede ser el que revisa.

```
Usa la skill auditoria-normativa sobre el borrador de
encargos/⟨tu carpeta⟩/salida/, contra los documentos de normativa/ y de
entrada/.
```

Recorre la tabla con los PDF abiertos. Veinte minutos.

---

## Lo que hay que medir al terminar

Apunta tres números y compáralos con lo que te costaba antes:

1. Cuánto has tardado en total.
2. Cuántos créditos has gastado.
3. Cuántas correcciones de fondo has tenido que hacer.

Y una cosa más: **los tres sitios donde te has atascado.** Eso es la agenda de
la siguiente sesión.
