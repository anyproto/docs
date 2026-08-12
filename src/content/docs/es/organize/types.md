---
title: "Tipos"
---

Si un objeto fuera un bizcocho, el tipo sería su molde. Los tipos son esquemas que definen el objeto. Notas, tareas, libros, personas, imágenes..., todo esto son tipos. Imagínatelos como moldes que te ayudan a dar una forma regular y predecible a todos tus objetos.

* Las **tareas** suelen tener fecha de vencimiento, prioridad y estado.
* Los **libros** suelen tener género, autor y fecha de publicación.
* Las **personas** suelen tener teléfono, correo electrónico y relación.

## Qué significa esto

1. **Encuentras lo que necesitas**: cuando tienes cientos de objetos, poder buscar por tipo es muy útil. Por ejemplo, «enséñame todas mis ideas» o «enséñame todas mis recetas».
2. **Aplicas tus normas**: los objetos de la misma categoría tendrán una estructura común. Todas tus películas tendrán una fecha de estreno; todas tus reuniones tendrán una transcripción.
3. **Defines tus relaciones**: con tipos para todos los objetos, puedes vincularlos claramente entre sí. Tus libros estarán vinculados a autores; tus tareas estarán vinculadas a proyectos.

## Cómo funciona

Cada objeto pertenece a un tipo, que le aplicas al crearlo y que puedes cambiar en cualquier momento. Anytype incluye tipos integrados, pero puedes crear tus propios tipos para adaptarlos a tus necesidades. Los tipos tienen:

* [properties.md](properties.md "mention") para definirlos, como dirección, fecha de creación y etiquetas.
* [views.md](views.md "mention") para organizarlos, como un calendario con todos los eventos importantes.
* [templates.md](templates.md "mention") para normalizarlos, como un álbum de fotos insertado en todas las vacaciones.

## Cómo crear un tipo

#### Barra lateral

Tanto el botón Crear como la barra lateral del canal muestran los tipos de tu espacio. Haz clic en los botones «Crear tipo» para añadir un tipo nuevo a tu espacio.

Ten en cuenta que la barra lateral solo mostrará los tipos que tengan al menos un objeto. Si el tipo que buscas no está en la barra lateral, añade un objeto de ese tipo y se mostrará automáticamente.

![types where sidebar](/assets/types-where-sidebar.jpg)

#### Ajustes del canal

Puedes ver todos tus tipos en tu [channel-settings.md](../settings/channel-settings.md "mention"), en la sección **Modelo de contenido**. Haz clic en el botón «Nuevo» para añadir un tipo nuevo a tu espacio.

Además, en los ajustes del canal tienes la opción **Tipo de objeto por defecto** para elegir el tipo que se aplicará a los objetos creados mediante el botón Crear.

![type where sidebar](/assets/type-where-sidebar.gif)

## Cómo editar un tipo

Hay tres formas principales de acceder a los ajustes de un tipo:

1. Abre el tipo desde la [barra lateral](../basics/sidebar/) y haz clic en **Editar tipo** en la parte superior derecha.
2. Cuando tengas abierto un [objeto](../create/objects/), haz clic en el botón de tres puntos de la esquina superior derecha y selecciona la opción **Ajustes de tipo**.
3. Ve a los [ajustes del canal](/es/settings/channel-settings/), haz clic en **Tipos de objeto** y selecciona el tipo que quieras modificar.

![types edit type](/assets/types-edit-type.gif)

En este panel puedes hacer varias cosas:

* cambiar el nombre y el icono del tipo,
* cambiar el ancho del contenido,
* añadir y eliminar propiedades y plantillas,
* hacer cambios en la cabecera del objeto,
* modificar el [diseño del objeto](/es/create/objects/formats/#formato-de-pagina).

### Cabecera del objeto

Los objetos pueden mostrar sus propiedades en la cabecera del objeto, que es la sección situada bajo el título y antes de los bloques de contenido. Para elegir las propiedades que se muestran en la cabecera, arrástralas y suéltalas en la sección «Cabecera».

Si no ves en la lista la propiedad que quieres, puedes añadirla usando el botón «+».

![types edit header](/assets/types-edit-header.gif)

#### Colocación en la cabecera

Puedes elegir la forma en que aparecen las propiedades en la cabecera. En la sección «Diseño» encontrarás estas dos opciones en «Vista de propiedades»:

1. Línea: con un aspecto más minimalista.
2. Lista: para mostrar información más estructurada.

## Cómo cambiar de tipo

El tipo de un objeto se puede cambiar en cualquier momento. Puedes hacerlo de varias formas:

* Abre el tipo, haz clic derecho en el objeto y elige **Cambiar tipo** en el menú.
* Si la cabecera del objeto incluye la propiedad «Tipo de objeto», selecciónala y elige **Cambiar tipo** en el menú.

Cuando el objeto cambia de tipo, conserva las propiedades originales. De esta forma, puedes cambiar de tipo una y otra vez sin perder ninguna de las propiedades de tus objetos.

![types change types](/assets/types-change-types.jpg)

#### Cambio de tipo en lote

Para cambiar el tipo de varios objetos a la vez, es mejor usar [views.md](views.md "mention"). Encontrarás más detalles [aquí](/es/organize/views/#edicion-de-objetos-en-lote).

## Cómo eliminar un tipo

Puedes eliminar un tipo desde la barra lateral, desde los ajustes del canal o desde los ajustes del editor (los tres puntos de la parte superior derecha). El tipo se trasladará a la papelera, desde donde podrás restaurarlo o eliminarlo definitivamente.

Si aún hay objetos que forman parte de ese tipo, se abrirá una ventana para que decidas si quieres eliminar o conservar esos objetos.

![docs types delete](/assets/docs-types-delete.jpg)

## Cómo duplicar un tipo en otro canal

Los tipos son particulares del canal en el que se crean. Si quieres que cierto tipo esté también en otros espacios, consulta [Importar y exportar](../data/import-and-export/README.md "mention"). Por el momento, no puedes tener tipos comunes y sincronizados entre espacios, ya que están separados por diferentes claves de cifrado.

## Notas

:::note
**No te compliques**. Crear demasiados tipos suele dar lugar a sistemas complejos y más difíciles de manejar. Empieza con los tipos integrados y ve añadiendo más cuando realmente los necesites.
:::

:::note
**Usa las propiedades**. Para sacar todo el partido a los tipos, añádeles propiedades relevantes. Así podrás ordenar y filtrar tus objetos en vistas útiles, como un tipo «Proyecto» con una vista kanban que solo muestre tus tareas más prioritarias.
:::
