---
description: Una búsqueda en tiempo real de todos los Objetos que comparten un Tipo o Relación común.
---

# Conjuntos

{% content-ref url="../../../use-cases/deep-dive-sets.md" %}
[deep-dive-sets.md](../../../use-cases/deep-dive-sets.md)
{% endcontent-ref %}

### Entendiendo los Conjuntos

Muchas personas comparan los Conjuntos con bases de datos, pero existe una diferencia clave: los Conjuntos no _almacenan_ Objetos como lo hacen las bases de datos regulares.

Los Conjuntos son una forma de visualizar una parte de tu Grafo y los Objetos que has creado, basándote en criterios filtrados y varios filtros secundarios que puedes personalizar. Puedes pensarlos como un filtro o consulta en tiempo real para Objetos que comparten ciertos criterios, específicamente un Tipo o una Relación.

#### Los Conjuntos cumplen dos funciones principales:

1. **Organizar y Acceder a Objetos**\
   \
   A menudo recibimos preguntas como: _¿Cómo puedo encontrar todas las Notas que he creado?_\
   \
   Una forma sencilla es crear un Conjunto basado en el Tipo.\
   Por ejemplo, Nota, que mostrará todas las Notas que has creado en Anytype.\
   \
   Si tienes notas específicas a las que te gustaría acceder frecuentemente, puedes filtrarlas según las Relaciones que hayas agregado a estas notas.\
   \
   Por ejemplo: Fecha de Creación, Etiquetas o Prioridad. (En este sentido, las Relaciones funcionan como atributos).\
   \
   Luego puedes anclar tu Conjunto al menú de Favoritos, donde estará en tu Barra Lateral, funcionando como una carpeta para todos los Objetos que cumplen ciertos criterios.
2.  **Editar Objetos**

    <figure><img src="../../../.gitbook/assets/assets/image (68).png" alt=""><figcaption></figcaption></figure>

    Los Conjuntos también proporcionan una forma de editar Objetos rápidamente en una Vista de lista.\
    \
    Puedes usar la selección múltiple en Conjuntos para eliminar varios Objetos a la vez, o para actualizar en lote las Relaciones o el Tipo de Objeto de los Objetos. Cualquier Relación agregada a un Conjunto en el Menú de Relaciones (arriba a la derecha) será adoptada por todos los nuevos Objetos creados con el botón "+ Nuevo Objeto".

{% embed url="https://drive.google.com/file/d/1emIekdXcrI0DTve9BQfweqTnPxa_BfGt/view?usp=drive_link" %}

### Creando Conjuntos

#### Puedes crear un Conjunto con el + en la esquina inferior izquierda o usando el menú de acceso directo / en el editor.

Luego, deberás elegir si deseas un Conjunto por Tipo, que te permite listar todos tus Objetos de un cierto Tipo, o un Conjunto por Relación, que listará todos los Objetos que contengan la Relación que elijas.&#x20;

También puedes crear un Conjunto por Tipo desde el conmutador de Tipo de Objeto en un nuevo documento.

<figure><img src="../../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

#### A continuación, debes decidir el propósito de tu Conjunto.&#x20;

Por ejemplo, la gestión de proyectos puede requerir el Tipo: Proyecto; para una lista de lecturas, el Tipo: Libro. Desde la Biblioteca, elige un Tipo de Objeto, haz clic en "Crear" y selecciona "Crear un conjunto."

Esto creará un conjunto de todos los Objetos con el Tipo: Libros.&#x20;

Ahora tienes una selección organizada de todos los objetos de libros ingresados en Anytype.

<figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

### Personalizando tu Conjunto

#### Alterna y Agrega Relaciones a Objetos mediante Conjuntos

En lugar de agregar Relaciones una por una a los Objetos, puedes agregarlas en lote a tu Conjunto haciendo clic en los filtros del lado derecho.

Aquí puedes activar/desactivar cualquier Relación que desees ver, agregar otra Relación o una nueva relación, y editar la Vista del Conjunto desde aquí.

![](<../../../.gitbook/assets/image (16).png>)

Puedes agregar cualquier Relación para que se incluya automáticamente en tus **Objetos**, agregándola durante el proceso de creación de tu **Tipo**.

Consulta más sobre cómo [crear-un-nuevo-tipo.md](../types/create-a-new-type.md "mention") aquí. Debajo de la sección de título y plantilla del proceso de nuevo Tipo, encontrarás las opciones de Relación.

![](<../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1).png>)

#### Orden y Filtros

También puedes ordenar o filtrar tu conjunto por cualquier relación que hayas agregado previamente al Conjunto.
