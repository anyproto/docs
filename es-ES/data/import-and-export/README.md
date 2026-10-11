# Importar y exportar

Puedes importar contenido a tus espacios y exportarlo en cualquier momento.

{% hint style="warning" %}
Estas funciones solo están disponibles en la versión de escritorio.
{% endhint %}

## Importar

1. Ve a los [ajustes del canal](../../settings/channel-settings.md).
2. En el menú lateral, haz clic en **Importar**.
3. Elige la opción que corresponda al tipo de contenido que vas a importar.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Import.jpg" alt=""><figcaption></figcaption></figure></div>

## Exportar

### Exportar un objeto

1. Abre el objeto.
2. Haz clic en los tres puntos de la esquina superior derecha.
3. Seleccionar **Exportar**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export Object.jpg" alt=""><figcaption></figcaption></figure></div>

### Exportar varios objetos

1. Abre una vista con los objetos que quieras exportar.
2. Selecciónalos usando el control izquierdo (en el diseño de cuadrícula y lista).
3. Haz clic derecho y selecciona **Exportar**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export Objects.jpg" alt=""><figcaption></figcaption></figure></div>

### Exportar vistas

1. Abre una vista, como un tipo, una consulta o una colección, con los objetos que quieras exportar.
2. Haz clic en los tres puntos de la esquina superior derecha.
3. Seleccionar **Exportar**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export View.jpg" alt=""><figcaption></figcaption></figure></div>

### Exportar canal

1. Ve a los [ajustes del canal](../../settings/channel-settings.md).
2. En el menú lateral, haz clic en **Exportar**.
3. Elige el formato que prefieras: Markdown o Any-Block.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export.jpg" alt=""><figcaption></figcaption></figure></div>

### Ajustes de exportación

Cuando vayas a elegir el formato de exportación, verás varias opciones:

1. **Formato de exportación**: elígelo según el propósito de tu exportación.
   1. Markdown, para usar el contenido en otras aplicaciones.
   2. Any-Block, para usar el contenido en otro espacio de Anytype.
   3. PDF, para obtener un archivo fácil de compartir.
   4. HTML, para usar el contenido en un navegador web.
2. **Formato de archivo**: puedes usar JSON o Protobuf. Protobuf no es un formato legible, pero suele ofrecer los mejores resultados.
3. **Archivo ZIP**: guarda la exportación como una carpeta comprimida.
4. **Incluir objetos enlazados**: incluye en el paquete todos los objetos hacia los que hay enlaces.
5. **Incluir archivos**: incluye imágenes, vídeos y otros archivos que hayas insertado en los objetos.
6. **Incluir objetos archivados**: incluye los objetos archivados en la exportación.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export Options.jpg" alt=""><figcaption></figcaption></figure></div>

## Lo que no incluye la exportación

#### Miembros del espacio

Cada miembro de un espacio está vinculado a una clave de cifrado única que es independiente del propio canal compartido. Por lo tanto, es posible que los datos relacionados con miembros del espacio no se exporten correctamente y aparezcan errores si importas la copia de respaldo a un espacio nuevo. Por ejemplo, propiedades como «Responsable» o «Creado por» quizás no muestren el miembro correcto.

#### Chats y debates

Los mensajes del chat y las discusiones están vinculados a los miembro del espacio, que a su vez están vinculados a claves de cifrado específicas de cada uno. Por lo tanto, no es posible exportar objetos de chat y mensajes porque están inherentemente ligados a ese espacio en sí.
