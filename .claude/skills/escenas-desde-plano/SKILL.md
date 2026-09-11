---
name: escenas-desde-plano
description: Convierte un plano exportado de AutoCAD en PDF en un conjunto de imágenes fotorrealistas para presentación o concurso, analizando el plano, eligiendo las escenas de venta y generándolas por MCP de imagen. Úsala cuando haya que ilustrar un proyecto a partir de planos sin pasar por Photoshop ni por el modelado 3D.
---

# Escenas desde plano

Sustituye al flujo antiguo: exportar de AutoCAD → colorear en Photoshop árbol a
árbol → levantar volumetría en Rhinoceros → renderizar → pedir «dale apariencia
real» a una IA. Tres semanas de volumetría para un TFG, horas por lámina.

## Lo que casi nadie sabe

**Un PDF exportado de AutoCAD lleva capa de texto vectorial.** Los rótulos de
estancia, el cajetín, la escala y el autor están ahí como texto extraíble con
sus coordenadas exactas. No hay que interpretar el dibujo a ojo ni colorearlo
para que se entienda: hay que **leerlo**.

Ese es el paso que sustituye a Photoshop. No era un problema pictórico, era que
nadie estaba leyendo los datos que el archivo ya traía.

## Procedimiento

1. **Extrae el texto y la geometría.** Con PyMuPDF: `page.get_text()` para el
   programa completo, `page.get_text("words")` para situar cada rótulo por
   coordenadas, y `get_pixmap` con `clip` para recortes en alta resolución de
   las zonas que necesites entender.
2. **Reconstruye el proyecto:** qué es, dónde está, quién lo firma, qué
   contiene cada pieza. Sitúa cada rótulo en el dibujo antes de decidir nada.
3. **Mira los recortes.** El texto da el programa; la geometría da la forma.
   Hacen falta los dos.
4. **Elige las escenas.** Entre seis y ocho. Un plano no se vende como plano: se
   vende como una secuencia de imágenes que cuenta el edificio en un orden.
   Como mínimo: una aérea del conjunto, el espacio central, un interior
   representativo, la pieza singular del proyecto, y la escala de calle.
5. **Enséñale la lista al arquitecto antes de generar.** El orden es suyo.
6. **Genera.** Sube el recorte limpio del plano como referencia visual para las
   escenas de conjunto: eso es lo que hace que la geometría sea la del proyecto
   y no una inventada. Las interiores pueden ir solo con texto.
7. **Guarda PNG originales y una copia JPG** a la misma resolución. El JPG es el
   que va a la memoria y a la presentación; el PNG pesa demasiado.

## Qué meter en cada prompt

- Uso y programa reales del edificio, sacados del plano.
- Emplazamiento concreto, con los hitos del entorno que salgan en el plano
  (río, vías, mar, preexistencias). Anclan la imagen y se notan.
- **Materiales.** El plano de distribución no dice acabados: pregúntalos. Si no
  hay respuesta, propón una paleta y **di explícitamente que es tu suposición**.
- Hora del día, tiempo, actividad humana.
- Y al final: sin texto, sin rótulos, sin marcas de agua.

## Después de la primera tanda

La primera tanda es un borrador, no el entregable. Se corrige por escrito y se
relanza solo la escena que falle: «el puente está demasiado alto, bájalo a nivel
de asfalto», «esa pared blanca circular es toda de vidrio», «el óculo del techo
no existe, son vigas metálicas».

Cuanto más contexto del proyecto se le dé —volumetrías, fotos de maqueta,
alzados— menos correcciones hacen falta.
