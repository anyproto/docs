---
description: Crea consultas precisas con operadores lógicos Y/O y grupos de reglas.
---

# Filtros avanzados

Los **filtros avanzados** te permiten combinar varios criterios de filtro con operadores lógicos Y/O y agruparlos en reglas anidadas para realizar consultas complejas como esta:

> Muestra todas las Tareas en las que (Prioridad es Alta **O** Fecha final es esta semana) **Y** Estado no es Hecho

Sin filtros avanzados, las reglas se suman con Y para aplicarlas de forma lineal. Con los filtros avanzados puedes usar paréntesis, expresar O, agrupar reglas y crear consultas precisas que reflejen tu forma de pensar en tus datos.

## Qué significa esto

A menudo, lo que necesitas filtrar es sencillo: «tareas que tengo asignadas» o «libros que he leído». Una sola regla es suficiente para estos casos.

Sin embargo, cuando tu conjunto de datos tiene cierta complejidad, empiezas a necesitar consultas como estas:

* «Tareas urgentes **O** vencidas»
* «Notas de este trimestre, **pero no** las etiquetadas como archivadas»
* «Libros que he valorado con 4 o 5 estrellas **Y** que aún no he recomendado»

Estas consultas necesitan al menos dos reglas, y la forma en que se combinan es importante. Para esto están los filtros avanzados.

## Cómo añadir un filtro avanzado

Los filtros avanzados se encuentran junto con los filtros básicos en la barra de filtro de toda colección o consulta.

1. Abre una consulta o colección en cualquier vista de lista (cuadrícula, lista, galería, kanban).
2. Haz clic en el icono de filtro (o usa el botón **+** que hay junto a la barra de filtros).
3. Selecciona **Añadir filtro avanzado** en la parte inferior del menú.
4. Define tus reglas en la barra que aparece.

La barra de filtro básico muestra reglas simples que se unen con Y. La barra de filtro avanzado muestra toda la secuencia lógica: agrupaciones con O, reglas anidadas e indicadores visuales de las combinaciones de reglas.

<figure><img src="../../../.gitbook/assets/unknown (1).png" alt=""><figcaption></figcaption></figure>

## Cómo construir las reglas

Una regla tiene tres partes:

* **Propiedad**: la propiedad que servirá como filtro (Estado, Prioridad, Etiquetas, Fecha de vencimiento, etc.).
* **Operador**: el modo de comparación (es, no es, está vacío, contiene, es mayor que, etc.).
* **Valor**: el criterio de comparación (un valor determinado, una lista o un [valor dinámico](advanced-filters.md#valores-de-filtro-dinamico)).

Los operadores disponibles dependen del formato de la propiedad:

| Formato de propiedad      | Operadores                                                                                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Texto / Título**          | es, no es, contiene, no contiene, está vacío, no está vacío                                                                                                                         |
| **Número**                | =, ≠, >, <, ≥, ≤, está vacío, no está vacío                                                                                                                                              |
| **Fecha**                  | es, es antes de, es después de, es en o antes de, es en o después de, está entre, está vacío, no está vacío **+** hoy, mañana, ayer, número de días atrás, número de días desde ahora, fecha exacta |
| **Selección / Selección múltiple** | contiene alguno, contiene todo, no contiene, está vacío, no está vacío                                                                                                                   |
| **Casilla**              | está marcada, no está marcada                                                                                                                                                            |
| **Objeto**                | contiene alguno, contiene todo, no contiene, está vacío, no está vacío                                                                                                                   |

### Combinar con Y/O

Por defecto, cuando hay varias reglas se unen con **Y**: se deben cumplir todas para que se seleccione el objeto. Si cambias al operador **O** entre dos reglas, solo tendrá que cumplirse una de ellas.

Para alternar entre Y y O:

1. Haz clic en el operador (Y / O) entre dos reglas.
2. Selecciona el que necesites.

Una guía visual:

```
Regla A  Y  Regla B  Y  Regla C    → Se deben cumplir las tres
Regla A  O  Regla B  Y  Regla C    → Se debe cumplir A, O (se deben cumplir tanto B como C)
```

### Agrupar reglas

Para crear una secuencia lógica más compleja, usa **grupos** para controlar la precedencia como con los paréntesis matemáticos:

```
(Prioridad es Alta  O  Prioridad es Urgente)  Y  Estado no es Hecho
```

Para crear un grupo, haz lo siguiente:

1. Añade la primera regla que quieras agrupar.
2. Haz clic en los tres puntos junto a los valores y elige **Convertir en grupo**.
3. Selecciona el operador Y u O.
4. Añade la siguiente regla.

Las reglas agrupadas se distinguen con una sangría en la barra de filtros. Puedes cambiar el operador interno de un grupo (Y u O) independientemente del operador que une los grupos.

Para eliminar una regla:

1. Haz clic en los tres puntos junto a los valores del grupo.
2. Haz clic en **Eliminar**.

<figure><img src="../../../.gitbook/assets/advanced-filters (1).png" alt=""><figcaption></figcaption></figure>

### Valores de filtro dinámicos

Los filtros admiten **valores dinámicos** que cambian según el contexto:

| Valor dinámico    | Dónde es útil                 | Ejemplo                             |
| ---------------- | ------------------------------------ | ----------------------------------- |
| **Usuario actual** | Propiedad de objeto que apunta a una persona | Tareas en las que Responsable = Usuario actual |
| **Este objeto**  | Consultas insertadas sobre propiedades del objeto  | Tareas en las que Proyecto = Este objeto   |
| **Hoy**        | Propiedad de fecha                        | Notas en las que Creado = Hoy         |

**Usuario actual** es especialmente útil en canales compartidos: cada miembro tiene su vista personal de una consulta sin necesidad de mantener consultas separadas para cada persona.

**Este objeto** funciona dentro de [listas insertadas](inline-queries.md): ajusta la consulta o colección insertada al objeto que la contiene.

### Selector de valores automático

Cuando seleccionas una propiedad en el menú del filtro, el selector de valores se abre automáticamente y te ahorra un clic adicional. Elige los valores que quieras y se añadirá el filtro.

### Barra de filtros activos

Cuando hayas configurado filtros, aparecerán en su **propia barra encima de la vista insertada**. Esta barra muestra cuántas reglas tiene aplicadas la vista.

Para modificar un filtro activo, haz clic en él. Para eliminarlo, haz clic en la × de la ficha del filtro. Para quitar todos los filtros con un clic, usa el botón **Limpiar** del final de la barra.

### Modelos de filtros frecuentes

#### Tareas en las que estoy trabajando ahora

```
Estado es En curso  Y  Responsable es Usuario actual
```

#### Notas de esta semana

```
Fecha de creación es esta semana
```

#### Libros que quiero recomendar

```
Valoración ≥ 4  Y  Recomendado a está vacío
```

#### Tareas bloqueadas o estancadas

```
Estado es Bloqueado  O  (Estado es En curso  Y  Modificado es antes de 7 días atrás)
```

#### Elementos pendientes de revisión

```
(Tipo es Documento  O  Tipo es Nota)  Y  Revisado está sin marcar  Y  Fecha de creación es antes de esta semana
```

## Notas

{% hint style="info" %}
**Agrupa las reglas O.** Por defecto, el operador Y tiene más prioridad; es posible que `A Y B O C` no signifique lo que piensas. Si colocas las reglas que usan O en un grupo, la intención es explícita y no hay ambigüedades.
{% endhint %}

{% hint style="info" %}
**Guarda filtros complejos como vistas aparte.** Si has creado un filtro que te va a costar recrear, guárdalo como una vista de la consulta en lugar de reconstruirlo cada vez. El menú de vistas permite cambiarlas con un solo clic.
{% endhint %}

{% hint style="info" %}
**Utiliza «Usuario actual» en plantillas de canales compartidos.** En un canal de equipo, una sola consulta «Mis tareas» sirve para todo el mundo: cada miembro ve sus propias tareas sin necesidad de duplicar la consulta para cada persona.
{% endhint %}
