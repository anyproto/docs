# Migrar desde Obsidian

#### Paso 1: Exportar desde Obsidian

* Limpia tus notas:
  * Convierte incrustados como `![[Título de nota]]` en enlaces simples `[[Título de nota]]`.
  * Elimina o convierte la sintaxis específica de complementos, como consultas de Dataview, campos de Templater, etc.
* Localiza tu bóveda:
  * Abre el administrador de bóvedas (que aparece al principio o desde `Archivo → Abrir bóveda`).
  * Haz clic derecho en la bóveda que quieres exportar y selecciona «Mostrar en el explorador del sistema».

#### Paso 2: Importar a Anytype

* Abre `Ajustes del canal → Importar → Obsidian` y haz clic en «Importar archivos».
* Selecciona toda la carpeta de tu bóveda o la subcarpeta que quieras importar.
  * Algunas plataformas, como Linux y Windows, no admiten la selección de carpetas.\\
    En ese caso, comprime la carpeta en un archivo .zip e importa ese archivo.
* Anytype procesará tus archivos y creará automáticamente un objeto por cada archivo de Markdown.

{% hint style="info" %}
**Asignación de contenido**

* Los `[[enlaces internos]]` → se convierten en enlaces entre objetos en Anytype, de modo que se mantiene la conexión entre tus notas.
* Las `#etiquetas` → se convierten en valores de la propiedad Tag (etiqueta). Puedes usarlos para filtrar, agrupar o buscar objetos.
* La sección Frontmatter (los metadatos entre `---` en la parte superior) → se convierten en propiedades del objeto.
{% endhint %}
