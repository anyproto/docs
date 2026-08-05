---
description: Contrae y expande secciones en los objetos largos.
---

# Títulos desplegables

Un **título desplegable** es un título que se puede contraer para ocultar todo lo que hay debajo. Haz clic en la flecha para plegar la sección; vuelve a hacer clic para desplegarla. El título sigue siendo visible; solo se contrae el contenido que tiene debajo.

Los tres niveles de título pueden ser desplegables: título 1 (H1), título 2 (H2) y título 3 (H3).

## Cómo funciona

Un título desplegable captura todo lo que tiene debajo como elementos secundarios hasta el siguiente título del mismo nivel o de un nivel superior. Cuando contraes el título, todos esos bloques secundarios se ocultan.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Toggled Headings.gif" alt=""/><figcaption></figcaption></figure></div>

## Cómo crear un título desplegable

#### Desde el menú /

1. Escribe `/` en el editor.
2. Busca **Título 1 desplegable, Título 2 desplegable** o **Título 3 desplegable.**
3. Selecciona el título del nivel que quieras.
4. Escribe el texto del título.

#### Atajos de Markdown

Escribe esto al principio de una línea:

* `#>` + espacio → Título 1 desplegable
* `##>` + espacio → Título 2 desplegable
* `###>` + espacio → Título 3 desplegable

#### Cómo convertir un desplegable normal en título

Si ya has creado un bloque desplegable normal (`>` + espacio), puedes convertirlo en un título desplegable:

1. Haz clic al principio del bloque desplegable.
2. Escribe `#`, `##` o `###` seguido de un espacio.
3. El desplegable se convierte en un título desplegable del nivel correspondiente.

#### Cómo convertir un título normal en desplegable

Para convertir un título normal en título desplegable, tienes dos opciones:

1. Haz clic en el control del bloque y selecciona **Estilo > Título desplegable**.
2. También puedes escribir `> + espacio` al principio del título.

## Cómo trabajar con títulos desplegables

#### Para expandirlos o contraerlos

Haz clic en la flecha (▶ / ▼) a la izquierda del título para expandir o contraer esa sección.

#### Para expandir o contraer varios desplegables a la vez

1. Selecciona todos los bloques desplegables que quieras abrir o cerrar.
2. Haz clic en la flecha desplegable de uno de ellos.

Esto funciona también con desplegables normales.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Toggle Headings Multiple.gif" alt=""/><figcaption></figcaption></figure></div>

#### Para añadir o eliminar bloques secundarios

Para añadir contenido bajo un bloque desplegable, haz clic al final del título y pulsa Entrar: se creará un bloque anidado.

Para sacar un bloque del desplegable, reduce su sangría con Mayús + Tab o arrástralo y suéltalo por encima del título.

#### Para volver a convertirlo en título normal

Haz clic en el control del bloque y selecciona **Estilo > Título 1** (o 2, o 3). El título ya no será desplegable y los bloques de debajo seguir-an en su sitio.

## Comportamiento en distintas vistas

* **En el editor**: los desplegables funcionan según la descripción anterior.
* **En la vista Flujo**: expandido o contraído como en el objeto.
* **En la exportación a PDF**: el contenido de las secciones contraídas no exporta. Expándelas todas antes de exportar si quieres ver su contenido en el PDF.
* **En la exportación a Markdown**: el estado de los desplegables no se conserva (Markdown no tiene sintaxis nativa para desplegables); todo el contenido se exporta con títulos normales.

## Notas

{% hint style="info" %} **Usa los títulos desplegables como divisores de secciones.** Un título 1 desplegable llamado «Archivo» o «Notas antiguas» puede servir para quitar de en medio el contenido sin eliminarlo. {% endhint %}

{% hint style="info" %} **Convierte un título normal en desplegable para organizar el documento rápidamente.** Si ya tienes una página estructurada con títulos, puedes convertirlos en desplegables para crear secciones contraíbles sin tener que reestructurarla. {% endhint %}
