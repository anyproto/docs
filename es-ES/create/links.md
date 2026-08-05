---
Description: La forma de conectar tus objetos.
description: Crea relaciones en tu base de conocimiento
---

# Enlaces

En Anytype, los enlaces son lo que convierte un montón de notas dispersas en una base de conocimiento conectada. Cuando vinculas un objeto «Tarea» a un objeto «Proyecto», estás indicando que están relacionados. Anytype registra esta relación como un enlace y lo hace visible en tu gráfico, que es un mapa mental de todo tu espacio.

Con el tiempo, estas conexiones adquieren un valor increíble. Te permiten rastrear las relaciones entre ideas, ver todo lo relacionado con un proyecto y descubrir patrones que no habías imaginado.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Links Intro Graph.gif" alt=""/><figcaption></figcaption></figure></div>

## Cómo crear enlaces

Anytype ofrece varias formas de crear enlaces con distinta utilidad según la situación:

|Método                 |Resultado                                          |Ideal para                                        |
|-----------------------|---------------------------------------------------|--------------------------------------------------|
|**Enlace de bloque**   |Añade una tarjeta o un enlace de texto en la página|Referencias importantes que quieres tener visibles|
|**Enlace de propiedad**|Añade una propiedad al objeto                      |Referencias sutiles que sirven para organizar     |
|**Enlace de fecha**    |Añade una referencia de fecha al objeto            |Referencias de tiempo para la cronología          |

## Cómo crear enlaces

### Enlace a un objeto

Directamente en el editor mediante uno de estos métodos:

1. **Enlaces de bloque**: escribe `/enlace`. Aparecen como tarjetas.
2. **Enlaces insertados**: escribe `@` y el nombre del objeto. Aparecen en línea con el texto de forma distintiva.
3. **Alias de enlace**: selecciona texto, pulsa `Cmd/Ctrl + Mayús + K` y selecciona el enlace. Aparecen como hipertexto que abre el objeto.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Linking Objects.jpg" alt=""/><figcaption></figcaption></figure></div>

### Enlace a una propiedad

Puedes vincular el objeto a [properties.md](../organize/properties.md "mention") de distintas formas:

1. **[Cabecera del objeto](../organize/properties.md#propiedades-en-la-cabecera-del-objeto)**: selecciona una propiedad en la cabecera. Si la propiedad no está visible, añádela a la cabecera desde los [ajustes del tipo](../organize/properties.md#cómo-crear-y-gestionar-las-propiedades).
2. **[Menú de bloque](editor/README.md#adding-blocks)**: inserta un bloque de propiedad desde el menú usando el botón «+» o el comando «/».

También puedes añadir una propiedad desde [views.md](../organize/views.md "mention"). Este es el mejor método para editar las propiedades de varios objetos.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Links Properties.gif" alt=""/><figcaption></figcaption></figure></div>

### Enlace a una fecha

Puedes enlazar a una fecha concreta con el atajo `@date` (fecha) en el editor. También puedes escribir `@today` (hoy), `@tomorrow` (mañana) o `@fecha específica`. Después podrás hacer clic en el bloque de fecha para ver todos los objetos relacionados con esa fecha.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Links Date.jpg" alt=""/><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Doc Link Date.gif" alt=""/><figcaption></figcaption></figure></div>

### Enlace a archivos externos

Si quieres añadir un enlace a un archivo externo en tu dispositivo de escritorio, usa un enlace que comience por **file:///**, seguido por la ruta del archivo local. Por ejemplo:

* `file:///Users/Nombre/Downloads/Protocol-Berg.pdf` para abrir ese PDF;
* `file:///Users/Nombre/Downloads/mi_presupuesto.xlsx` para abrir esa hoja de cálculo.

Para insertar un enlace de este tipo, selecciona «Enlace a sitio web», igual que cuando insertas un enlace a un sitio de Internet.

## Cómo ver los enlaces

#### Enlaces entrantes

Puedes usar la propiedad «Enlaces entrantes» de la cabecera del objeto para ver qué objetos contienen un enlace al objeto que tienes abierto. Si no encuentras la propiedad «Enlaces entrantes», ve a los ajustes del tipo y añádela a la sección «Cabecera». [Encontrarás más detalles aquí](../organize/properties.md#cómo-crear-y-gestionar-las-propiedades).

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Link Back.gif" alt=""/><figcaption></figcaption></figure></div>

#### Gráfico de conocimiento

Tus documentos pueden contener varias conexiones que los asocian a otros objetos de tu espacio. El gráfico es la mejor forma de visualizarlas, ya que muestra la red completa de conexiones entre todos tus objetos. Haz clic en el icono del gráfico, situado en la parte superior izquierda del editor, para acceder a tu gráfico.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Links Backlink Graph.gif" alt=""/><figcaption></figcaption></figure></div>

En esta documentación tienes más información sobre las [propiedades](../organize/properties.md "mention") y el [gráfico](../advanced/feature-list-by-platform/graph.md "mention").