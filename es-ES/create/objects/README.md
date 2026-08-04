# Objetos

En Anytype, todo lo que creas es un objeto. Páginas, tareas, proyectos, personas, imágenes, recetas… Todo son objetos. Si has usado otras herramientas, puede suelas pensar en términos de archivos y carpetas en una jerarquía de árbol. Pero así no es como funciona Anytype.

* **Las carpetas preguntan: «¿Dónde va esto?»** Tienes que decidir si tu nota corresponde a la carpeta Reuniones, Clientes o Proyectos; si quieres tenerla en más de una, tienes que duplicarla.
* **Los objetos preguntan: «¿Con qué se relaciona esto?».** Tu nota existe por sí misma y puedes conectarla a tus Reuniones, Clientes y Proyectos al mismo tiempo, sin duplicarla.

En Anytype, creas un objeto y le vas añadiendo relaciones con el tiempo. Así se construye un sistema flexible de conocimiento interconectado en el que no importa dónde están las cosas, sino con qué están relacionadas.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Object System.jpg" alt=""/><figcaption></figcaption></figure></div>

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

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Objects How.jpg" alt=""/><figcaption></figcaption></figure></div>

## Cómo crear objetos

#### Menú Crear

En la parte superior de la barra lateral, junto al nombre del canal, está el botón principal que se utiliza para añadir contenido a tu espacio. El botón tiene dos partes:

* **Botón Crear**: al hacer clic en el botón «Crear», crearás inmediatamente un nuevo objeto. Puedes elegir el [tipo](../../organize/types.md) que usa este botón para los objetos en los [ajustes del canal](../../settings/channel-settings.md); por defecto es «Página».
* **Desplegable Crear**: al hacer clic en la flecha desplegable junto al botón «Crear», aparece un menú con estas opciones:
  * Tipos de objeto para crear uno directamente.
  * Crear a partir del portapapeles
  * Cargar desde el dispositivo

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Objects Create.jpg" alt=""/><figcaption></figcaption></figure></div>

#### Sección Tipos

Puedes crear un objeto directamente desde la sección «Tipos» de la barra lateral: pasa el puntero sobre el [tipo](../../organize/types.md) y haz clic en el botón «+». Aquí también encontrarás Consultas y Colecciones. Ten en cuenta lo siguiente:

* Si esta sección no está visible, consulta [Gestionar secciones](../../basics/sidebar/sections.md#gestionar-secciones) para mostrarla.
* En esta sección solo se muestran los tipos que tienen al menos un objeto. Si la categoría que buscas no aparece en la sección «Tipos», [usa el menú Crear](./README.md#menú-crear) para crear primero un objeto de ese tipo y así aparecerá en esta sección.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Objects Create Section.jpg" alt=""/><figcaption></figcaption></figure></div>

#### Menú de comandos

Mientras trabajas en el editor, puedes escribir `/` para abrir el menú de comandos. Si ya sabes el tipo que quieres usar, puedes escribirlo directamente. Si no tienes claro el tipo que quieres usar, puedes desplazarte hasta la sección «Tipos» para elegir uno.

Los objetos creados de esta forma dejan un bloque de enlace en la página y generan un [enlace entrante](../links.md) hacia el objeto recién creado.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Object Create Command.gif" alt=""/><figcaption></figcaption></figure></div>

#### Atajo de teclado

Para crear rápidamente un objeto, puedes usar este atajo: `Cmd/Ctrl + N`. El resultado será el mismo que al hacer clic en el signo «+» de la barra lateral. Además, puedes usar `Cmd/Ctrl + Opt/Alt + N` para abrir el mismo menú que al hacer clic en la flecha Crear de la barra lateral.

#### Convertir en objeto

Si estás trabajando en un objeto y quieres transformar un bloque determinado en otro objeto, puedes emplear el menú de acciones:

1. Pasa el puntero por el extremo izquierdo del bloque en cuestión y haz clic en los 3 puntos.
2. Haz clic en **Convertir en objeto** y selecciona el [tipo](../../organize/types.md) que desees.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/hjhgjkgf.gif" alt=""/><figcaption></figcaption></figure></div>

## Cómo localizar tus objetos

#### Barra lateral

Puedes encontrar todos tus objetos en la [barra lateral](../../basics/sidebar/ "mention"), agrupados por sus respectivos [types.md](../../organize/types.md "mention"). Si esta sección no está visible, consulta [Gestionar secciones](../../basics/sidebar/sections.md#gestionar-secciones) para mostrarla.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Objects Find Sidebar.gif" alt=""/><figcaption></figcaption></figure></div>

#### Búsqueda

Usa uno de estos métodos para hacer una búsqueda:

* Ve a la barra lateral y haz clic en el botón de búsqueda.
* Usa el atajo de teclado `Cmd / Ctrl + K`.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Objects Search.jpg" alt=""/><figcaption></figcaption></figure></div>

#### Gráfico

Para ver todos tus objetos y las conexiones entre ellos, puedes recurrir al [graph.md](../../advanced/feature-list-by-platform/graph.md "mention") como tu principal fuente de información. Cuando tengas abierto un objeto, haz clic en el icono «Gráfico» que aparece junto a los botones de avance y retroceso.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Objects Find Graph.jpg" alt=""/><figcaption></figcaption></figure></div>

#### Papelera

Cuando elimines objetos de tus [channels.md](../../basics/channels.md "mention"), aparecerán en la [papelera](../../organize/deletion.md) hasta que los elimines definitivamente.

Puedes acceder a la papelera desde la barra lateral. Si esta sección no está visible, consulta [Gestionar secciones](../../basics/sidebar/sections.md#gestionar-secciones) para mostrarla.

## Cómo editar objetos en lote

Los objetos tienen tipos y propiedades que se visualizan mejor en [views.md](../../organize/views.md "mention"). Para editar varios objetos al mismo tiempo, lo mejor es usar la función Vistas. Tienes [más detalles aquí](../../organize/views.md#edición-de-objetos-en-lote).

## Cómo elegir el tipo de objeto por defecto

Sigue estos pasos para elegir el tipo que se usará por defecto al crear un objeto:

1. Haz clic en el desplegable Crear de la barra lateral.
2. Pasa el puntero por encima del tipo que prefieras.
3. Haz clic en el botón de tres puntos.
4. Selecciona la opción **Establecer por defecto**.

También puedes configurarlo en los [ajustes del canal](../../settings/channel-settings.md).

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Create Default.jpg" alt=""/><figcaption></figcaption></figure></div>

## Notas

{% hint style="info" %} **Usa las vistas para organizar tus objetos.** Como no existe una jerarquía de carpetas para los objetos, la mejor forma de mantener la organización es usar las [vistas](../../organize/views.md). {% endhint %}
