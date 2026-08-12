---
title: "Propiedades"
---

Las propiedades son los datos que asocias a un objeto: su fecha de vencimiento, estado, prioridad, etiquetas o cualquier otro atributo que te importe. Si habláramos de hojas de cálculo, cada objeto sería una fila, y cada propiedad, una columna.

![properties intro](/assets/properties-intro.jpg)

## Qué significa esto

Las propiedades te permiten organizar el conocimiento mediante sistemas flexibles, ya que puedes utilizarlas para ordenar, filtrar y consultar tus objetos:

* Busca todas las **tareas** cuya **prioridad** sea **alta**.
* Busca todos los **libros** cuyo estado sea **leído**, ordenados por **valoración**.
* Busca todas las **ideas** cuya **fecha de creación** sea el **año pasado**.

## Cómo funciona

Las propiedades cumplen dos funciones. Vamos a usar un objeto del tipo «Tarea» como ejemplo.

**1\. Definen los objetos.** Úsalas para añadir datos útiles y descriptivos, como estos:

* Estado: En curso
* Prioridad: Alta
* Fecha final: El próximo viernes

**2\. Conectan los objetos**. Úsalas para vincular un objeto a otro; por ejemplo:

* Asignado a: → Alex (un objeto del tipo «Persona»)
* Proyecto: → Rediseño del sitio web (un objeto del tipo «Proyecto»)

![properties example](/assets/properties-example.gif)

## Formatos de propiedades <a href="#types-of-relations" id="types-of-relations"></a>

Estos son los formatos disponibles en Anytype para las propiedades:

<table data-search="false"><thead><tr><th width="182.1171875">Formato de propiedad</th><th>Descripción</th></tr></thead><tbody><tr><td><strong>Texto</strong></td><td>Para introducir texto libre.</td></tr><tr><td><strong>Número</strong></td><td>Para números. Pronto habrá distintos formatos de número.</td></tr><tr><td><strong>Fecha</strong></td><td>Fecha, con hora opcional.</td></tr><tr><td><strong>Selección</strong></td><td>Lista predefinida de opciones. Se puede elegir solo una.</td></tr><tr><td><strong>Selección múltiple</strong></td><td>Lista predefinida de opciones. Se pueden elegir varias, sin límite.</td></tr><tr><td><strong>Correo electrónico/Teléfono/URL</strong></td><td>Formatos especiales para direcciones, números de teléfono y URL.</td></tr><tr><td><strong>Casilla</strong></td><td>Casilla de verificación para marcar.</td></tr><tr><td><strong>Archivos y medios</strong></td><td>Para adjuntar archivos de texto, audio, vídeo o imagen.</td></tr><tr><td><strong>Objeto</strong></td><td>Referencia a otro objeto (persona, tarea, documento...).</td></tr></tbody></table>

## Relación entre tipos y propiedades

* Las propiedades de los objetos son independientes de los [tipos](/es/organize/types/). Un tipo se puede entender como un conjunto de propiedades que se aplica a todos los objetos de ese tipo.
* Puedes usar una misma propiedad en varios tipos; por ejemplo, la propiedad «Género» se puede aplicar tanto a libros como a películas.
* Puedes aplicar a un objeto concreto una propiedad que no forme parte de su tipo; por ejemplo, la propiedad «Favorito» puede estar en un objeto «Libro», aunque no se haya incluido en el tipo «Libro».

## Cómo crear y gestionar las propiedades

Puesto que todos los [objetos](../create/objects/) pertenecen a un [tipo](/es/organize/types/), es mejor usar las propiedades dentro del contexto del tipo. Tienes estas posibilidades:

* crear propiedades nuevas,
* añadir propiedades existentes,
* cambiar su orden,
* hacerlas visibles u ocultarlas,
* quitar propiedades del tipo,
* mover propiedades a la papelera.

#### Desde el menú de edición del tipo

[Mientras editas un tipo](/es/organize/types/#como-editar-un-tipo), usa el botón «+» de la sección «Propiedades» para añadir una propiedad existente o crear una nueva. Para editar una propiedad, haz clic en ella. Para cambiar el orden, haz clic en cada control de la izquierda y arrastra las propiedades.

![properties create type settings](/assets/properties-create-type-settings.jpg)

#### Desde la vista del tipo

Cuando tengas abierto un tipo, puedes hacer clic en el botón «Ajustes de vista» de la parte superior derecha de la cuadrícula, seleccionar **Propiedades** y añadir la propiedad que desees. Para editar una propiedad, haz clic en ella. Para cambiar el orden, haz clic en cada control de la izquierda y arrastra las propiedades.

![types create view](/assets/types-create-view.gif)

#### Desde el editor del objeto

Puedes añadir propiedades a los objetos tal como lo harías con cualquier otro bloque del editor: por medio del botón `+` o del menú `/`.

Es posible añadir propiedades que no tengan relación con el tipo de ese objeto; sin embargo, si es algo que haces con frecuencia, es mejor añadir la propiedad al tipo de objeto para facilitar la organización.

![properties create command](/assets/properties-create-command.jpg)

#### Desde los ajustes del canal

Abre [channel-settings.md](../settings/channel-settings.md "mention"), ve a «Modelo de contenido» y selecciona **Propiedades**. Aquí basta con hacer clic en el botón «Nuevo» para crear una propiedad.

## Cómo usar las propiedades

Lo más recomendable es aplicar las propiedades en el contexto de un tipo. Puedes gestionarlas desde el panel «Editar tipo», tienes más detalles [aquí](/es/organize/types/#como-editar-un-tipo).

### Propiedades en las vistas

Las propiedades despliegan todo su poder en las [vistas](views.md "mention"), que ofrecen formas flexibles y adaptables de interactuar con tu contenido. Tienes más detalles en la sección [Vistas](/es/organize/views/).

![docs properties views](/assets/docs-properties-views.gif)

### Propiedades en la cabecera del objeto

Cuando abres un objeto con formato de página, las propiedades pueden estar visibles en la cabecera, esto es, la sección que hay entre el título y el contenido. Hay dos opciones de presentación:

* **Línea**, con un aspecto más minimalista.
* **Lista**, para mostrar información más estructurada.

La opción se elige en los ajustes del tipo, por lo que la presentación será la misma para todos los objetos de ese tipo.

![properties header layouts](/assets/properties-header-layouts.jpg)

Puedes usar la cabecera del objeto para lo siguiente:

1. **Mostrar las propiedades más importantes**: edita el tipo, ve a la sección Propiedades, arrastra las propiedades que quieras mostrar y ordénalas como prefieras. Las que pongas en las secciones «Panel de propiedades» y «Oculto» no se mostrarán en la cabecera.
2. **Modificar el valor de las propiedades directamente en el editor**: haz clic en una propiedad de la cabecera para editarla.

Las propiedades que no se muestran en la cabecera siguen formando parte del tipo; normalmente, se utilizan en las [vistas](/es/organize/views/).

### Propiedades en los bloques

Si quieres mostrar propiedades en el área de contenido de una página, puedes insertarlas como bloques. Para hacerlo, tienes estos métodos:

* Abre el menú de comandos con `/` o con el botón «+» y desplázate hasta la sección «Propiedades».
* Escribe / seguido del nombre de la propiedad; por ejemplo, `/tags` o `/description` (las propiedades del sistema aparecerán en inglés).

Solo es posible añadir bloques de las propiedades que ya estén incluidas en el tipo o tengan un valor asociado.

El bloque con la propiedad insertada se puede manipular como cualquier otro bloque, lo que resulta especialmente útil a la hora de diseñar [plantillas](/es/organize/templates/) para evitar las limitaciones de diseño de la cabecera del objeto.

![docs properties blocks](/assets/docs-properties-blocks.gif)

### Panel de propiedades

Para ver rápidamente todas las propiedades del objeto que tengas abierto, abre su panel de propiedades con el icono de información de la esquina superior derecha.

![docs properties use panel](/assets/docs-properties-use-panel.jpg)

## Cómo eliminar propiedades

Las propiedades son independientes de los [tipos](/es/organize/types/) y los [objetos](../create/objects/), así que hay varias formas de eliminarlas.

#### Desde un tipo

1. [Abre el tipo](/es/organize/types/#como-editar-un-tipo) que contiene la propiedad que quieres eliminar.
2. Haz clic derecho en la propiedad y selecciona una de estas opciones:
   1. **Quitar del tipo** desvincula la propiedad del tipo, pero la mantiene en el espacio. Los objetos que tengan algún valor asignado a esa propiedad lo conservarán, aunque la hayas eliminado de su tipo.
   2. **Mover a la papelera** desvincula la propiedad de todos los tipos y la elimina del espacio. La propiedad se puede restaurar desde la papelera.

![docs properties remove](/assets/docs-properties-remove.jpg)

#### Desde los ajustes del canal

En esta sección puedes ver los objetos que están conectados a una propiedad, los tipos que la utilizan y otros detalles que sirven para mantener la organización.

1. Ve los [ajustes del canal](/es/settings/channel-settings/) desde la barra lateral.
2. En «Modelo de contenido», selecciona **Propiedades**.
3. Haz clic derecho en la propiedad y selecciona **Mover a la papelera**. Esto desvincula la propiedad de todos los tipos.

![docs properties remove channel settings](/assets/docs-properties-remove-channel-settings.jpg)

## Notas

:::note
**No te compliques; menos es más.** Cuando estés empezando, usa la menor cantidad de propiedades posible. Ve añadiendo propiedades a medida que aumente tu necesidad de organización.
:::

:::note
**Las etiquetas (tags) son la forma más fácil de empezar a usar las propiedades.** Añade etiquetas relevantes a todos tus documentos y crea una [consulta](/es/organize/queries/) que los agrupe por etiqueta.
:::
