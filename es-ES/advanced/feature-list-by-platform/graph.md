---
description: Visualiza las conexiones entre tus objetos.
---

# Gráfico

El **gráfico** es un mapa visual en tiempo real de todos los objetos que contiene tu canal y de las conexiones entre ellos. Cada objeto es un vértice, o nodo; cada enlace y cada referencia de propiedad es una arista. Cuando abres el gráfico, ves la estructura de tu canal: lo que está en el centro, lo que está aislado, lo que aglutina proyectos a su alrededor.

## Cómo abrir el gráfico

El icono del gráfico, un pequeño símbolo de un nodo, aparece en la parte superior de todos los objetos. Haz clic en él para cambiar a la vista de gráfico.

<figure><img src="../../../.gitbook/assets/graph.png" alt=""><figcaption></figcaption></figure>

También puedes pulsar el atajo que encontrarás en tus ajustes de atajos para abrir el gráfico desde cualquier objeto.

## Cómo interpretar el gráfico

Cada **nodo** es un objeto. Pasa el puntero por un nodo para ver su título y su tipo.

Cada **arista** (línea que conecta dos nodos) representa una relación, ya sea un enlace en el editor, una propiedad de un objeto que apunta a otro objeto, o un enlace entrante desde otro objeto.

La **dirección de la arista** (si están activadas las flechas) muestra qué objeto hace referencia a qué otro:

* A → B indica que el objeto A tiene un enlace o referencia al objeto B.
* Una conexión bidireccional (A ↔ B) indica que ambos tienen enlaces entre sí.

## Ajustes de presentación

Haz clic en el icono de engranaje o el menú de ajustes, en la parte superior derecha del gráfico, para abrir las opciones de presentación:

#### Aspecto

* **Títulos**: muestra el nombre del objeto bajo a cada nodo (desactívalo para despejar la vista).
* **Flechas**: muestra la dirección de las aristas.
* **Iconos**: muestra el icono del objeto en cada nodo.

#### Conexiones

* **Enlaces**: muestra los enlaces insertados en el editor hacia otros objetos.
* **Propiedades**: muestra las relaciones mediante propiedades de los objetos.
* **Objetos desconectados**: muestra los objetos que no tienen conexiones (huérfanos).

Activar o desactivar una opción hace que el gráfico cambie al instante. Puedes personalizar la vista (por ejemplo, mostrar solo conexiones con propiedades y ocultar enlaces del editor) para concentrarte en cada clase de relación por separado.

#### Filtrar por tipo

El menú **Filtrar por tipo** permite mostrar solo algunos tipos de objetos en el gráfico:

1. Haz clic en «Filtrar por tipo».
2. Activa o desactiva los tipos que quieras.

Esta es la forma más rápida de estudiar una capa; por ejemplo, puedes mostrar solo tareas y proyectos para ver un desglose de tu trabajo.

## Buscar en el gráfico

La búsqueda de la parte superior del gráfico sirve para encontrar un objeto concreto:

* Escribe cualquier parte del título de un objeto y se resaltarán los nodos que coincidan.
* Pulsa Entrar para ir a la primera coincidencia.
* Usa las teclas de flecha para pasar de una coincidencia a otra.

Los nodos coincidentes se resaltan y el resto del gráfico se atenúa para que los encuentres de un vistazo.
