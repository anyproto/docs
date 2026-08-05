# Tipos de bloque

Hay muchos tipos de bloques, cada uno con su propia utilidad. Añade y prueba todos los que quieras.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Block Types.gif" alt=""/><figcaption></figcaption></figure></div>

### Bloques de texto

|Bloque                          |Para qué sirve                                                                                          |
|--------------------------------|--------------------------------------------------------------------------------------------------------|
|**Párrafo**                     |Texto normal                                                                                            |
|**Título 1, Título 2, Título 3**|Estructura de secciones, o títulos (H1, H2 y H3)                                                        |
|**Título**                      |Título del objeto                                                                                       |
|**Cita**                        |Texto citado o destacado                                                                                |
|**Globo**                       |Texto en recuadro para advertencias, consejos o notas                                                   |
|**Código**                      |Código monoespaciado con resaltado de sintaxis                                                          |
|**Desplegable**                 |Bloque contraíble que oculta el contenido anidado                                                       |
|**Título desplegable**          |Un título que también contrae y expande su sección, consulta [Títulos desplegables](toggled-headings.md)|

### Bloques de lista

|Bloque               |Para qué sirve                                   |
|---------------------|-------------------------------------------------|
|**Lista con viñetas**|Lista sin orden                                  |
|**Lista numerada**   |Lista numerada automáticamente                   |
|**Casilla**          |Casillas de verificación para elementos de acción|

Pulsa Tab dentro de un elemento de lista para añadirle sangría y crear una sublista anidada. Mayús + Tab le quita la sangría.

### Bloques de medios

|Bloque     |Para qué sirve                         |
|-----------|---------------------------------------|
|**Imagen** |Imagen insertada                       |
|**Vídeo**  |Reproductor de vídeo incrustado        |
|**Audio**  |Reproductor de audio incrustado        |
|**Archivo**|Archivo genérico con enlace de descarga|
|**PDF**    |PDF con vista previa                   |

Arrastra un archivo al editor para insertarlo. Cada archivo se convierte en un [objeto de archivo](../files-and-media.md) que puedes encontrar y e insertar en otros lugares.

{% hint style="info" %} **Consejo:** Usa el atajo `/arch` para añadir como bloque una imagen o archivo que ya esté en tu espacio. No tienes que volver a cargar el mismo archivo desde tu dispositivo; sube el archivo una vez y reutilízalo tantas veces como quieras. {% endhint %}

### Bloques de estructura

|Bloque      |Para qué sirve                                                                              |
|------------|--------------------------------------------------------------------------------------------|
|**Divisor** |Línea de separación horizontal                                                              |
|**Índice**  |Generado automáticamente a partir de tus títulos                                            |
|**Tabla**   |Bloque de datos con estilo de hoja de cálculo                                               |
|**Columnas**|Se crean arrastrando bloques uno al lado del otro (no hay un «bloque de columna» específico)|

#### Tablas

Inserta un bloque de tabla con `/tabla`. La tabla se inserta como una cuadrícula reducida que puedes ampliar arrastrando el borde derecho o el inferior. Puedes cambiar el tamaño de las columnas: arrastra el límite entre dos columnas para ajustar el ancho a tu gusto. Ese ancho se conserva al exportar a PDF.

También puedes seleccionar varias celdas a la vez:

* Haz clic y arrastra por las celdas para seleccionar un rango.
* Aplica formato (negrita, color) a toda la selección.
* Copia varias celdas para pegarlas en otro lugar.
* Elimina el contenido de la selección.

### Bloques de referencia

|Bloque                 |Para qué sirve                                                                                                   |
|-----------------------|-----------------------------------------------------------------------------------------------------------------|
|**Enlace a objeto**    |Tarjeta o texto que hace referencia a otro objeto                                                                |
|**Fecha insertada**    |Referencia a una fecha                                                                                           |
|**Mención insertada**  |Mención con estilo `@` a un objeto                                                                               |
|**Consulta insertada** |Consulta dinámica incrustada, ver [Consultas insertadas](../../advanced/feature-list-by-platform/inline-queries.md)|
|**Colección insertada**|Colección dinámica incrustada                                                                                    |
|**Chat insertado**     |Hilo de chat incrustado                                                                                          |

### Bloques de propiedades

|Bloque       |Para qué sirve                                            |
|-------------|----------------------------------------------------------|
|**Propiedad**|Añade una propiedad del objeto como bloque en el contenido|

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