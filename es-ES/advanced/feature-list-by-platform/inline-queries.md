---
description: Presenta una vista de objetos filtrada y dinámica dentro de otro objeto.
---

# Vistas insertadas

Las **consultas insertadas** y **colecciones insertadas** son objetos incrustados en otro objeto. En lugar de abrir una consulta en su propia página, presentas los resultados directamente en el editor, junto al texto, las imágenes y otros bloques.

La consulta insertada se actualiza automáticamente cuando se añaden, modifican o eliminan objetos en el canal.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/inline-list (1).png" alt=""><figcaption></figcaption></figure></div>

## Qué significa esto

Las consultas y colecciones insertadas convierten cualquier página en un **panel de información**. Por ejemplo, una página de proyecto puede tener lo siguiente:

* una lista de todas las tareas pendientes de ese proyecto,
* una galería de documentos relacionados,
* un tablero de estado agrupado por progreso,
* la actividad reciente de los miembros del equipo.

Todo esto, siempre al día y en un mismo objeto. No necesitas abrir la página de la consulta  para ver lo que está pasando: la tienes ahí mismo.

## Cómo crear una consulta insertada

#### Método 1: insertar una consulta existente

Si ya has creado una consulta y quieres mostrarla en un objeto:

1. Escribe `/inser` en el editor.
2. Elige **Consulta insertada** en el menú.
3. Busca el nombre de la consulta y selecciónala.
4. La consulta se inserta con la vista por defecto de la original.

#### Método 2: crear una consulta insertada nueva

Si quieres insertar una consulta que solo exista dentro de ese objeto:

1. Escribe `/inser`.
2. Elige **Consulta insertada > Crear nueva consulta**.
3. Elige el criterio de selección: **Tipo de objeto** o **Propiedad**.
4. Configura filtros y criterios de orden como en cualquier otra consulta.
5. Esta consulta insertada se guarda también como objeto independiente, así que podrás encontrarla desde la barra lateral y reutilizarla donde quieras.

Estos métodos sirven también para insertar una colección y tener una lista de objetos seleccionados por ti en una página de proyecto.

## Cómo personalizar la vista de una consulta insertada

Haz clic en el bloque de la consulta insertada para seleccionarlo y usa los controles normales de las consultas:

* **Diseño**: elige entre cuadrícula, lista, galería, kanban, calendario y gráfico.
* **Propiedades**: activa las que quieras mostrar en los campos o columnas.
* **Filtrar**: añade filtros, que se aplicarán solo en esta inserción de la consulta.
* **Ordenar**: decide el orden de los objetos mostrados en esta vista.
* **Agrupar**: en la vista de kanban, elige la propiedad por la que se agruparán los objetos.

Todos estos ajustes afectan solo al bloque insertado, no a la consulta original.

<figure><img src="../../../.gitbook/assets/inline-list.png" alt=""><figcaption></figcaption></figure>

### Valores de filtro dinámicos

Las consultas insertadas hacen buena pareja con los [valores de filtro dinámicos](advanced-filters.md). Estos son dos valores especialmente útiles:

* **Usuario actual** filtra los objetos según quien los esté viendo. Si insertas una consulta con el filtro `Tareas en las que Responsable = Usuario actual` en un panel de información compartido, cada miembro verá sus propias tareas.
* **Este objeto** filtra los objetos según el objeto que contenga la consulta insertada. Si insertas una consulta con el filtro `Tareas en las que Proyecto = Este objeto` en un objeto de tipo «Proyecto», la consulta se centra automáticamente en ese proyecto. Si mueves o copias ese objeto a un proyecto distinto, la consulta insertada se actualiza.

De esta forma, puedes crear una plantilla para el tipo «Proyecto» con una consulta insertada `Tareas de Este objeto` y utilizarla con todos los proyectos sin tener que configurar el filtro en cada uno de ellos.

### Insertar varias consultas en un objeto

Puedes insertar en un objeto tantas consultas cuantas quieras:

```
# Hoy

[Consulta insertada: Tareas en las que Estado = En curso y Responsable = Usuario actual]

# Esta semana

[Consulta insertada: Notas en las que Creado = últimos 7 días]

# En lectura

[Consulta insertada: Libros en los que Estado = Leyendo]
```

Cada bloque de consulta es independiente. Las consultas se presentan en paralelo, se actualizan en tiempo real y te permiten crear un «centro de control» personal.

## Notas

{% hint style="info" %}
**Construye una página como agenda con consultas insertadas.** Selecciona esa página como página de inicio del canal (Ajustes del canal > Preferencias > Página de inicio). Cada vez que abras el canal, tendrás una visión de tu día.
{% endhint %}

{% hint style="info" %}
**Usa «Este objeto» como filtro en las plantillas.** Una plantilla de proyecto con una consulta insertada `Tareas en las que Proyecto = Este objeto` se adaptará dinámicamente a cada proyecto que crees a partir de ella.
{% endhint %}

{% hint style="info" %}
**Mezcla consultas y colecciones insertadas.** Usa una colección insertada para «cosas que coloco aquí a mano» (lista de lecturas seleccionadas, referencias clave) y consultas insertadas para «cosas que cumplen ciertos criterios» (tareas activas, cambios recientes). Es una combinación muy potente.
{% endhint %}
