# Tipos de bloque

Hay muchos tipos de bloques, cada uno con su propia utilidad. Añade y prueba todos los que quieras.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Block Types.gif" alt=""/><figcaption></figcaption></figure></div>

### Bloques de texto

<table data-search="false"><thead><tr><th width="244.21484375">Bloque</th><th>Para qué sirve</th></tr></thead><tbody><tr><td><strong>Párrafo</strong></td><td>Texto normal</td></tr><tr><td><strong>Título 1, Título 2, Título 3</strong></td><td>Estructura de secciones, o títulos (H1, H2 y H3)</td></tr><tr><td><strong>Título</strong></td><td>Título del objeto</td></tr><tr><td><strong>Cita</strong></td><td>Texto citado o destacado</td></tr><tr><td><strong>Globo</strong></td><td>Texto en recuadro para advertencias, consejos o notas</td></tr><tr><td><strong>Código</strong></td><td>Código monoespaciado con resaltado de sintaxis</td></tr><tr><td><strong>Desplegable</strong></td><td>Bloque contraíble que oculta el contenido anidado</td></tr><tr><td><strong>Título desplegable</strong></td><td>Un título que también contrae y expande su sección, consulta <a href="toggled-headings.md">Títulos desplegables</a></td></tr></tbody></table>

### Bloques de lista

<table><thead><tr><th width="200.66796875">Bloque</th><th>Para qué sirve</th></tr></thead><tbody><tr><td><strong>Lista con viñetas</strong></td><td>Lista sin orden</td></tr><tr><td><strong>Lista numerada</strong></td><td>Lista numerada automáticamente</td></tr><tr><td><strong>Casilla</strong></td><td>Casillas de verificación para elementos de acción</td></tr></tbody></table>

Pulsa Tab dentro de un elemento de lista para añadirle sangría y crear una sublista anidada. Mayús + Tab le quita la sangría.

### Bloques de medios

<table><thead><tr><th width="165.9921875">Bloque</th><th>Para qué sirve</th></tr></thead><tbody><tr><td><strong>Imagen</strong></td><td>Imagen insertada</td></tr><tr><td><strong>Vídeo</strong></td><td>Reproductor de vídeo incrustado</td></tr><tr><td><strong>Audio</strong></td><td>Reproductor de audio incrustado</td></tr><tr><td><strong>Archivo</strong></td><td>Archivo genérico con enlace de descarga</td></tr><tr><td><strong>PDF</strong></td><td>PDF con vista previa</td></tr></tbody></table>

Arrastra un archivo al editor para insertarlo. Cada archivo se convierte en un [objeto de archivo](../files-and-media.md) que puedes encontrar y e insertar en otros lugares.

{% hint style="info" %} **Consejo:** Usa el atajo `/arch` para añadir como bloque una imagen o archivo que ya esté en tu espacio. No tienes que volver a cargar el mismo archivo desde tu dispositivo; sube el archivo una vez y reutilízalo tantas veces como quieras. {% endhint %}

### Bloques de estructura

<table><thead><tr><th width="205.1328125">Bloque</th><th>Para qué sirve</th></tr></thead><tbody><tr><td><strong>Divisor</strong></td><td>Línea de separación horizontal</td></tr><tr><td><strong>Índice</strong></td><td>Generado automáticamente a partir de tus títulos</td></tr><tr><td><strong>Tabla</strong></td><td>Bloque de datos con estilo de hoja de cálculo</td></tr><tr><td><strong>Columnas</strong></td><td>Se crean arrastrando bloques uno al lado del otro (no hay un «bloque de columna» específico)</td></tr></tbody></table>

#### Tablas

Inserta un bloque de tabla con `/tabla`. La tabla se inserta como una cuadrícula reducida que puedes ampliar arrastrando el borde derecho o el inferior. Puedes cambiar el tamaño de las columnas: arrastra el límite entre dos columnas para ajustar el ancho a tu gusto. Ese ancho se conserva al exportar a PDF.

También puedes seleccionar varias celdas a la vez:

* Haz clic y arrastra por las celdas para seleccionar un rango.
* Aplica formato (negrita, color) a toda la selección.
* Copia varias celdas para pegarlas en otro lugar.
* Elimina el contenido de la selección.

### Bloques de referencia

<table><thead><tr><th width="205.19921875">Bloque</th><th>Para qué sirve</th></tr></thead><tbody><tr><td><strong>Enlace a objeto</strong></td><td>Tarjeta o texto que hace referencia a otro objeto</td></tr><tr><td><strong>Fecha insertada</strong></td><td>Referencia a una fecha</td></tr><tr><td><strong>Mención insertada</strong></td><td>Mención con estilo <code>@</code> a un objeto</td></tr><tr><td><strong>Consulta insertada</strong></td><td>Consulta dinámica incrustada</td></tr><tr><td><strong>Colección insertada</strong></td><td>Colección dinámica incrustada</td></tr><tr><td><strong>Chat insertado</strong></td><td>Hilo de chat incrustado</td></tr></tbody></table>

### Bloques de propiedades

<table><thead><tr><th width="193.50390625">Bloque</th><th>Para qué sirve</th></tr></thead><tbody><tr><td><strong>Propiedad</strong></td><td>Añade una propiedad del objeto como bloque en el contenido</td></tr></tbody></table>

Sirve para mostrar [properties.md](../../organize/properties.md "mention") de forma destacada. El valor de la propiedad se mantiene sincronizado en el bloque: si cambias uno, todos los demás se actualizan. Esto permite crear plantillas y diseños elaborados para todos tus documentos.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/slashmenu-property.png" alt=""/><figcaption></figcaption></figure></div>

### Bloques de código

Los bloques de código incluyen lo siguiente:

* **Resaltado de sintaxis**: elige el lenguaje en el menú desplegable de la esquina superior derecha del bloque.
* **Sangría multilínea**: selecciona varias líneas y pulsa Tab para aplicar sangría a todas, Mayús + Tab para quitarla.
* **Copiar**: al pasar el cursor aparece un botón para copiar el bloque entero en el portapapeles.
* **Ajuste de línea**: las líneas largas se pueden ajustar o recorrer con la barra de desplazamiento

Escribe ` ``` ` (tres acentos graves) seguido de un espacio al principio de una línea para que se convierta en un bloque de código. Tras crearlo, haz clic en el menú desplegable de la izquierda para elegir el resaltado de sintaxis de un lenguaje.

### Bloques incrustados

Consulta [Incrustados](../../advanced/feature-list-by-platform/embeds.md) para ver la lista completa: LaTeX, YouTube, Miro, Mermaid, Figma y otros.
