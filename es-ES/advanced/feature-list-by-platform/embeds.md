---
description: Añade directamente contenido externo dinámico a tus objetos.
---

# Elementos incrustados

Un elemento **incrustado** es un bloque del editor que muestra contenido actualizado de un servicio externo: un vídeo de YouTube, un tablero de Miro, una ubicación de Google Maps, un diagrama de Mermaid. En lugar de añadir un simple enlace al contenido original, puedes incrustarlo en el objeto para verlo y, en muchos casos, interactuar con él sin salir de Anytype.

## Qué significa esto

El contenido incrustado te permite tener junto todo tu trabajo. Por ejemplo, una página de proyecto puede tener lo siguiente:

* la lluvia de ideas de Miro junto a las notas de la reunión,
* un tutorial de YouTube que explica la técnica,
* la ruta de Google Maps hasta el lugar,
* un diagrama de Mermaid con la arquitectura del sistema.

Y todo, sin tener que saltar entre pestañas y aplicaciones. Cuando regresas a esa página unas semanas después, todo lo que necesitas sigue estando allí y el contenido incrustado está actualizado con los cambios posteriores.

## Cómo añadir un incrustado

Esta es la forma más rápida:

1. En el editor, escribe `/` para abrir el menú y escribe el nombre del elemento que quieras incrustar ([aquí hay una lista completa](embeds.md#incrustaciones-admitidas)) o desplázate hasta la sección «Incrustados». 
2. Elige el que quieras y pega la URL correspondiente.

También puedes pegar una URL directamente en el editor. El menú «Pegar como» ofrece cuatro opciones:

* **URL**: se inserta como enlace de texto para visitarlo al hacer clic.
* **Marcador**: se crea una tarjeta de marcador con vista previa de metadatos.
* **Incrustado**: se incrusta el contenido dinámico (solo con los servicios admitidos).
* **Texto simple**: se pega la URL como texto normal.

Si la URL es de un servicio incrustable admitido, la opción por defecto es **Incrustado**. Si se trata de un servicio desconocido, solo verás las opciones **URL**, **Marcador** y **Texto simple**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (12) (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

## Incrustaciones admitidas

#### Vídeo y audio

* **YouTube**: pega cualquier URL de YouTube, incluso enlaces con marca de tiempo.
* **Vimeo**: pega la URL de un vídeo.
* **Bandcamp**: pega la URL de un álbum o una pista.
* **SoundCloud**: pega la URL de una pista o una lista de reproducción.
* **Apple Music**: pega el enlace de una canción, un álbum o una lista de reproducción.

#### Diagramas y elementos visuales

* **Mermaid**: escribe con sintaxis de Mermaid y se renderizará directamente como diagrama de flujo, diagrama de secuencia u otro diagrama de Mermaid.
* **Miro**: pega la URL de un tablero de Miro (quien tenga un enlace público de Miro puede verlo; los tableros privados requieren acceso de visualización).
* **Excalidraw**: inserta un editor de Excalidraw como bloque y edítalo ahí mismo (desactivado temporalmente por problemas de rendimiento).
* **Figma**: pega la URL de un marco o un archivo de Figma.
* **draw.io**: pega la URL de un diagrama publicado.

#### Mapas y ubicaciones

* **Google Maps**: pega una URL o unas coordenadas de Maps.
* **OpenStreetMap**: pega la URL de una ubicación.

#### Código y contenido

* **LaTeX**: puedes ver los detalles [aquí](../../create/editor/inline-latex.md "mention").
* **GitHub Gist**: pega la URL de un gist.
* **CodePen**: pega la URL de un pen.
* **CodeSandbox**: pega la URL de un sandbox.

#### Redes sociales

* **Twitter / X**
* **Reddit**
* **Facebook**
* **Instagram**

## Archivos incrustados

Además de servicios externos, también puedes incrustar archivos que tengas en Anytype:

* **Imagen**: arrastra una imagen, pégala desde el portapapeles o escribe `/imagen`.
* **Vídeo**: arrastra uno o escribe `/vídeo`.
* **Audio**: arrastra uno o escribe `/audio`.
* **PDF**: arrastra uno o escribe `/pdf`.

Estos elementos incrustados están vinculados al [objeto de archivo](../../create/files-and-media.md): el archivo se convierte en un objeto en tu canal, donde puedes buscarlo, etiquetarlo y crear enlaces hacia él.

#### Estilo por defecto de bloques de archivo

Puedes elegir entre dos modos de presentación para los bloques de archivo:

* **Incrustado**: el archivo se representa en el objeto (imagen visible, reproductor de vídeo, reproductor de audio).
* **Enlace**: un breve enlace con el nombre del archivo, que se abre al hacer clic.

La opción por defecto se establece en **Ajustes del arca > Preferencias > Contenido y vistas > Estilo por defecto de bloques de archivo**, pero puedes cambiarla en cada bloque: pasa el puntero por el bloque de archivo, haz clic en el menú de tres puntos y elige el estilo que prefieras.

### Cambiar el tamaño y la posición de un bloque incrustado

Casi todos los bloques incrustados, como vídeos, mapas y contenido visual, cuentan con un control de tamaño. Arrastra el control para aumentar o reducir su tamaño. El cambio se aplica solo a ese bloque.

Si quieres colocar un bloque incrustado en una columna junto al texto, arrástralo al lado de otro bloque. Tienes más detalles sobre el diseño de columnas en [Bloques](../../create/editor/).

### Sintaxis de Mermaid (referencia rápida)

Mermaid es un lenguaje de diagramas basado en texto. Escribe `/mermaid` para insertar un bloque de Mermaid y luego escribe algo como esto:

```
graph TD
  A[Inicio] --> B{Decision}
  B -->|Sí| C[Hacer esto]
  B -->|No| D[Hacer lo otro]
```

Anytype representa esto como un diagrama de flujo en tiempo real. Mermaid admite diagramas de flujo, diagramas de secuencia, diagramas de Gantt, diagramas de clases y más; consulta la [documentación de Mermaid](https://mermaid.js.org) para ver la sintaxis completa.

## Notas

{% hint style="info" %}
**Incrusta para consultar, enlaza para citar.** Un artículo de la Wikipedia funciona mejor como enlace (no es muy incrustable), mientras que un tablero de Miro queda mejor incrustado (para poder verlo). Elige el mejor formato para el uso que le darás.
{% endhint %}

{% hint style="info" %}
**Usa Mermaid para crear diagramas editables.** Los diagramas de Mermaid se crean con texto: si los modificas en tu objeto, el cambio permanece. Sin embargo, una captura de pantalla de un diagrama ya no sirve cuando cambias algo.
{% endhint %}

{% hint style="warning" %}
**Las incrustaciones dependen de servicios externos.** Si YouTube modifica su API de incrustación o alguien borra un tablero de Miro, la incrustación deja de funcionar en tu objeto. El contenido importante debería guardarse también como marcador o descargarse como copia de respaldo.
{% endhint %}
