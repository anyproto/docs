# Editor

Anytype es un editor basado en bloques y todas las [páginas](../objects/formats.md#formato-de-página) se construyen con bloques, de forma que tu contenido es flexible y fácil de usar. El editor es la forma principal de crear documentos en Anytype.

## Cómo funciona

Los **bloques** son los componentes básicos de todo objeto; piensa en ellos como las piezas de lego de cada documento. Cuando abres un objeto y empiezas a editarlo, lo que haces es añadir bloques y organizarlos: párrafos, títulos, imágenes, listas, contenido incrustado, etc. Cada bloque es independiente y se puede mover, cambiar de estilo o sustituir sin que esto afecte a los demás.

Si has usado Notion, este concepto te sonará. Si lo comparas con Microsoft Word o Google Docs, la diferencia es que los bloques son **unidades separadas**: puedes arrastrarlos, anidarlos, convertir un formato en otro o crear columnas colocándolos lado a lado.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks.gif" alt=""/><figcaption></figcaption></figure></div>

## Cómo añadir bloques

Los distintos tipos de bloques aparecen en el **Menú de bloque**, que se abre con un botón «+» o el comando «/».

#### Botón +

Pasa el puntero por el lado izquierdo de cualquier bloque y aparecerá un botón «+». Haz clic en él para insertar un bloque nuevo. Este mismo menú se abre también con el comando «/».

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks Plus Menu.jpg" alt=""/><figcaption></figcaption></figure></div>

#### Menú /

Escribe `/` en cualquier parte del editor. Aparece un menú con todos los tipos de bloque disponibles, organizados por categoría. Para filtrarlos, escribe algunos caracteres del tipo que busques: `/tít` para un bloque de título, `/cod` para un bloque de código, `/imag` para una imagen.

Esta es la forma más rápida si ya sabes lo que quieres.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/slshmenu-block.png" alt=""/><figcaption></figcaption></figure></div>

#### Atajos de teclado

Para los bloques de texto, puedes usar atajos de teclado estilo Markdown al inicio de la línea. Escribe un espacio detrás del atajo y el bloque se transformará.

|Escribe esto|Para crear esto     |
|------------|--------------------|
|`#`         |Título 1            |
|`##`        |Título 2            |
|`###`       |Título 3            |
|`>`         |Desplegable         |
|`*` o `-`   |Lista con viñetas   |
|`1.`        |Lista numerada      |
|`[]`        |Casilla             |
|` ``` `     |Bloque de código    |
|`---`       |Divisor             |
|`#>`        |Título desplegable 1|
|`##>`       |Título desplegable 2|
|`###>`      |Título desplegable 3|

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks Markdown.gif" alt=""/><figcaption></figcaption></figure></div>

## Cómo dar estilo a los bloques

#### Un solo bloque

Pasa el puntero sobre un bloque para destacarlo. Aparecen las opciones del bloque:

* **Control del bloque** (tres puntos a la izquierda), para moverlo, eliminarlo o transformarlo.
* **Botón +** (a la izquierda), para insertar un bloque nuevo.
* **Barra flotante** (en algunos bloques), para dar formato al texto.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks Options.jpg" alt=""/><figcaption></figcaption></figure></div>

#### Varios bloques

Haz clic en un bloque, mantén pulsada la tecla Mayús y haz clic en otro para seleccionar todos los bloques que hay entre ambos. También puedes hacer clic y arrastrar con el ratón para seleccionar todos los bloques que quieras. Ahora podrás, por ejemplo:

* **arrastrarlos** todos juntos a otro lugar,
* **eliminarlos** todos a la vez,
* **aplicar formato** (negrita, cursiva, color) a todo el texto seleccionado,
* **convertirlos** todos a un tipo de bloque distinto (p. ej., convertir cinco párrafos en una lista con viñetas).

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks Select.gif" alt=""/><figcaption></figcaption></figure></div>

#### Formato de texto

Dentro de un bloque de texto puedes aplicar formatos a palabras o caracteres por separado. Selecciona el texto y aparecerá una barra de herramientas flotante con estas opciones:

* **Negrita:** `Cmd/Ctrl + B` o `**texto**`
* **Cursiva**: `Cmd/Ctrl + I` o `*texto*`
* **Tachado**: `Cmd/Ctrl + Mayús + S` o `~~texto~~`
* **Código en línea**: `Cmd/Ctrl + Mayús + L` o comillas invertidas `` `código` ``
* **Subrayado**: `Cmd/Ctrl + U`
* **Enlace**: `Cmd/Ctrl + K`, y pega una URL o busca un objeto.
* **Color de fondo**: selecciona el texto y elige un color de en barra flotante.
* **Color de texto**: igual que el resaltado, en la barra flotante.
* **Citar en conversación**: copia el texto en un comentario de [discussions.md](../../collaborate/discussions.md "mention").

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks Inline Styling (2).jpg" alt=""/><figcaption></figcaption></figure></div>

#### Controles de los bloques

Cada bloque tiene un control en su lado izquierdo que abre el menú de opciones del bloque:

* **Convertir en objeto**: convierte un bloque en otro tipo de bloque, como frase → título o lista numerada → lista con viñetas.
* **Color**: cambia el color del texto.
* **Fondo**: cambia el color de fondo.
* **Mover a**: traslada el bloque a otro objeto.
* **Copiar / Cortar / Pegar / Duplicar / Eliminar**
* **Citar en conversación**: inicia un hilo de debate sobre este bloque concreto.

Este menú también se abre al hacer clic derecho en cualquier bloque.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Block Action Menu.jpg" alt=""/><figcaption></figcaption></figure></div>

El control del bloque no sirve solo para el menú, sino también para arrastrar y mover bloques. Haz clic, mantén pulsado y arrastra el bloque:

* **arriba o abajo** para cambiar su posición en el objeto,
* **a la izquierda o a la derecha** de otro bloque para crear una columna,
* **fuera de una lista anidada** para sacarlo de esta,
* **sobre un enlace a otro objeto** para añadir el bloque como contenido a ese objeto.

#### Sangría y anidamiento

Casi todos los tipos de bloque se pueden anidar: párrafos, imágenes, elementos de lista, desplegables y títulos pueden tener elementos secundarios.

* `Tab` aumenta la sangría (avanza).
* `Mayús + Tab` reduce la sangría (retrocede).

#### Columnas

Las columnas funcionan con todos los tipos de bloque. Puedes colocar texto junto a imágenes, incrustaciones junto a listas y cualquier otra combinación. Esto es lo más parecido a un diseño de autoedición, muy útil para páginas de proyectos y paneles de control. Para crear columnas, coloca un bloque al lado de otro:

1. Haz clic en el control de seis puntos del borde izquierdo de un bloque.
2. Arrastra el bloque hacia el lado derecho de otro bloque, hasta que veas un indicador vertical para colocarlo.
3. Suelta el bloque. Ahora, los dos bloques están uno al lado del otro.

Repite con otro bloque para seguir añadiendo columnas. Para volver a convertir dos columnas en una sola columna, arrastra uno de los bloques por encima o por debajo del otro.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Blocks Columns.gif" alt=""/><figcaption></figcaption></figure></div>

## Notas

{% hint style="info" %} **Títulos desplegables + índice = mejor navegación en páginas muy largas.** Si usas ambas cosas, puedes contraer las secciones que no estés editando y usar el índice para pasar de una a otra. Consulta [Títulos desplegables](toggled-headings.md). {% endhint %}