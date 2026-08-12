---
title: "Objetos"
---

En Anytype, todo lo que creas es un objeto. Páginas, tareas, proyectos, personas, imágenes, recetas… Todo son objetos. Si has usado otras herramientas, puede suelas pensar en términos de archivos y carpetas en una jerarquía de árbol. Pero así no es como funciona Anytype.

* **Las carpetas preguntan: «¿Dónde va esto?»** Tienes que decidir si tu nota corresponde a la carpeta Reuniones, Clientes o Proyectos; si quieres tenerla en más de una, tienes que duplicarla.
* **Los objetos preguntan: «¿Con qué se relaciona esto?».** Tu nota existe por sí misma y puedes conectarla a tus Reuniones, Clientes y Proyectos al mismo tiempo, sin duplicarla.

En Anytype, creas un objeto y le vas añadiendo relaciones con el tiempo. Así se construye un sistema flexible de conocimiento interconectado en el que no importa dónde están las cosas, sino con qué están relacionadas.

![docs object system](/assets/docs-object-system.jpg)

## Qué significa esto

Como todo es un objeto, todo puede conectarse con todo lo demás. Una tarea puede vincularse a una persona. Una nota de reunión puede vincularse a un proyecto. Estás construyendo un gráfico de información interconectada, en lugar de ordenar archivos en jerarquías de carpetas.

Este es el resultado:

* **Todo es fácil de encontrar.** Una persona puede estar conectada a una empresa, un proyecto, una reunión, una tarea y mucho más, por lo que puedes acceder a ella desde cualquiera de esos lugares.
* **No hay duplicados.** Vincula la misma imagen a varios documentos en vez de copiarla en cada uno.
* **Empiezas por la creación, no por la organización.** Nunca tienes que decidir si una nota pertenece a «Trabajo» o a «Personal»: puede ser las dos cosas a la vez.
* **Los patrones emergen con el tiempo.** A medida que añades vínculos, van apareciendo por sí solas conexiones que no habías planeado y que pueden revelar información valiosa.

## Cómo funciona

Los objetos tienen:

* [types.md](../../organize/types.md "mention") que los clasifican como notas, tareas, proyectos, reuniones, etc.
* [properties.md](../../organize/properties.md "mention") que almacenan sus datos, como el estado, la fecha, el autor, el correo electrónico, etc.
* [links.md](../links.md "mention") a otros objetos, como una receta conectada a una persona.

Aquí tienes un ejemplo sencillo de este funcionamiento:

1. Creas una **tarea**, que es un objeto de ese tipo.
2. Le añades una **fecha de vencimiento**, que es una propiedad.
3. La conectas a un **proyecto**, lo que es un enlace.

![docs objects how](/assets/docs-objects-how.jpg)

## Cómo crear objetos

#### Menú Crear

En la parte superior de la barra lateral, junto al nombre del canal, está el botón principal que se utiliza para añadir contenido a tu espacio. El botón tiene dos partes:

* **Botón Crear**: al hacer clic en el botón «Crear», crearás inmediatamente un nuevo objeto. Puedes elegir el [tipo](/es/organize/types/) que usa este botón para los objetos en los [ajustes del canal](/es/settings/channel-settings/); por defecto es «Página».
* **Desplegable Crear**: al hacer clic en la flecha desplegable junto al botón «Crear», aparece un menú con estas opciones:
  * Tipos de objeto para crear uno directamente.
  * Crear a partir del portapapeles
  * Cargar desde el dispositivo

![objects create](/assets/objects-create.jpg)

#### Sección Tipos

Puedes crear un objeto directamente desde la sección «Tipos» de la barra lateral: pasa el puntero sobre el [tipo](/es/organize/types/) y haz clic en el botón «+». Aquí también encontrarás Consultas y Colecciones. Ten en cuenta lo siguiente:

* Si esta sección no está visible, consulta [Gestionar secciones](/es/basics/sidebar/sections/#gestionar-secciones) para mostrarla.
* En esta sección solo se muestran los tipos que tienen al menos un objeto. Si la categoría que buscas no aparece en la sección «Tipos», [usa el menú Crear](/es/create/objects/#menú-crear) para crear primero un objeto de ese tipo y así aparecerá en esta sección.

![objects create section](/assets/objects-create-section.jpg)

#### Menú de comandos

Mientras trabajas en el editor, puedes escribir `/` para abrir el menú de comandos. Si ya sabes el tipo que quieres usar, puedes escribirlo directamente. Si no tienes claro el tipo que quieres usar, puedes desplazarte hasta la sección «Tipos» para elegir uno.

Los objetos creados de esta forma dejan un bloque de enlace en la página y generan un [enlace entrante](/es/create/links/) hacia el objeto recién creado.

![object create command](/assets/object-create-command.gif)

#### Atajo de teclado

Para crear rápidamente un objeto, puedes usar este atajo: `Cmd/Ctrl + N`. El resultado será el mismo que al hacer clic en el signo «+» de la barra lateral. Además, puedes usar `Cmd/Ctrl + Opt/Alt + N` para abrir el mismo menú que al hacer clic en la flecha Crear de la barra lateral.

#### Convertir en objeto

Si estás trabajando en un objeto y quieres transformar un bloque determinado en otro objeto, puedes emplear el menú de acciones:

1. Pasa el puntero por el extremo izquierdo del bloque en cuestión y haz clic en los 3 puntos.
2. Haz clic en **Convertir en objeto** y selecciona el [tipo](/es/organize/types/) que desees.

![hjhgjkgf](/assets/hjhgjkgf.gif)

## Cómo localizar tus objetos

#### Barra lateral

Puedes encontrar todos tus objetos en la [barra lateral](../../basics/sidebar/ "mention"), agrupados por sus respectivos [types.md](../../organize/types.md "mention"). Si esta sección no está visible, consulta [Gestionar secciones](/es/basics/sidebar/sections/#gestionar-secciones) para mostrarla.

![objects find sidebar](/assets/objects-find-sidebar.gif)

#### Búsqueda

Usa uno de estos métodos para hacer una búsqueda:

* Ve a la barra lateral y haz clic en el botón de búsqueda.
* Usa el atajo de teclado `Cmd / Ctrl + K`.

![objects search](/assets/objects-search.jpg)

#### Gráfico

Para ver todos tus objetos y las conexiones entre ellos, puedes recurrir al [graph.md](../../advanced/feature-list-by-platform/graph.md "mention") como tu principal fuente de información. Cuando tengas abierto un objeto, haz clic en el icono «Gráfico» que aparece junto a los botones de avance y retroceso.

![objects find graph](/assets/objects-find-graph.jpg)

#### Papelera

Cuando elimines objetos de tus [channels.md](../../basics/channels.md "mention"), aparecerán en la [papelera](/es/organize/deletion/) hasta que los elimines definitivamente.

Puedes acceder a la papelera desde la barra lateral. Si esta sección no está visible, consulta [Gestionar secciones](/es/basics/sidebar/sections/#gestionar-secciones) para mostrarla.

## Cómo editar objetos en lote

Los objetos tienen tipos y propiedades que se visualizan mejor en [views.md](../../organize/views.md "mention"). Para editar varios objetos al mismo tiempo, lo mejor es usar la función Vistas. Tienes [más detalles aquí](/es/organize/views/#edición-de-objetos-en-lote).

## Cómo elegir el tipo de objeto por defecto

Sigue estos pasos para elegir el tipo que se usará por defecto al crear un objeto:

1. Haz clic en el desplegable Crear de la barra lateral.
2. Pasa el puntero por encima del tipo que prefieras.
3. Haz clic en el botón de tres puntos.
4. Selecciona la opción **Establecer por defecto**.

También puedes configurarlo en los [ajustes del canal](/es/settings/channel-settings/).

![docs create default](/assets/docs-create-default.jpg)

## Notas

:::note
**Usa las vistas para organizar tus objetos.** Como no existe una jerarquía de carpetas para los objetos, la mejor forma de mantener la organización es usar las [vistas](/es/organize/views/).
:::
