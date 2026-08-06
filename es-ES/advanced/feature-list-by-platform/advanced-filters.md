---
description: Crea consultas precisas con lógica AND/OR y condiciones agrupadas.
---

# Filtros avanzados

**Filtros avanzados** te permite combinar varias condiciones de filtro con lógica Y/O y agruparlas en reglas anidadas, para que puedas expresar consultas complejas como:

> Muéstrame todas las tareas donde (la prioridad es Alta **OR** la fecha límite es esta semana) **AND** el estado no es Completado

Sin filtros avanzados, todas las condiciones se unen con AND y se aplican de forma lineal. Los filtros avanzados te permiten usar paréntesis: puedes expresar OR, agrupar reglas y crear consultas precisas que reflejen cómo piensas realmente sobre tus datos.

## Qué significa esto

La mayoría de las necesidades de filtrado son sencillas: «tareas asignadas a mí», «libros que he leído». Una sola condición es suficiente para eso.

Pero cuando tus datos tienen cierta complejidad, empiezas a necesitar cosas como:

* «Tareas urgentes **O** vencidas»
* «Notas de este trimestre, **pero no** las etiquetadas como 'archivo'»
* «Libros a los que he dado 4 o 5 estrellas **Y** que aún no he recomendado»

Cada una de esas opciones necesita al menos dos condiciones, y la forma en que se combinan es importante. Los filtros avanzados permiten expresar esto.

## Cómo añadir un filtro avanzado

Los filtros avanzados conviven con los filtros básicos en la barra de filtros de cualquier Colección o consulta.

1. Abre una consulta o Colección en cualquier vista de tipo lista (cuadrícula, lista, galería, tablero).
2. Haz clic en el icono de filtro (o usa el botón **+** que aparece junto a la barra de filtros).
3. Elige **Añadir filtro avanzado** en la parte inferior del menú.
4. Define tus condiciones en la barra dedicada que aparece.

La barra de filtro básico muestra condiciones simples unidas por AND. La barra de filtro avanzado muestra tu lógica completa, incluidos los agrupamientos OR, las reglas anidadas y los indicadores visuales de cómo se combinan las condiciones.

<figure><img src="../../../.gitbook/assets/unknown (1).png" alt=""/><figcaption></figcaption></figure>

## Crear condiciones

Cada condición tiene tres partes:

* **Propiedad**: la propiedad por la que filtrar (estado, prioridad, etiquetas, fecha de vencimiento, etc.)
* **Operador**: cómo comparar (es, no es, está vacío, contiene, es mayor que, etc.)
* **Valor**: con qué comparar (un valor específico, una lista o un [valor dinámico](advanced-filters.md#dynamic-filter-values))

Los operadores disponibles dependen del tipo de propiedad:

|Tipo de propiedad                 |Operadores                                                                                                                                                                                                                 |
|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|**Texto / Título**                |es, no es, contiene, no contiene, está vacío, no está vacío                                                                                                                                                                |
|**Número**                        |=, ≠, >, <, ≥, ≤, está vacío, no está vacío                                                                                                                                                                                |
|**Fecha**                         |es, es antes de, es después de, es el mismo día o después, es el mismo día o antes, está dentro de, está vacío, no está vacío **+** hoy, mañana, ayer, número de días atrás, número de días a partir de ahora, fecha exacta|
|**Selección / Selección múltiple**|contains any, contains all, doesn't contain, is empty, is not empty                                                                                                                                                        |
|**Checkbox**                      |is checked, is not checked                                                                                                                                                                                                 |
|**Object**                        |contains any, contains all, doesn't contain, is empty, is not empty                                                                                                                                                        |

### Combining with AND / OR

By default, multiple conditions are joined by **AND** — every condition must be true for an Object to match. Switch to **OR** between two conditions and only one of them needs to be true.

To toggle between AND and OR:

1. Click the operator label (AND / OR) between two conditions.
2. The label flips to the other operator.

Visually:

```
Condition A  AND  Condition B  AND  Condition C    → All three must be true
Condition A  OR   Condition B  AND  Condition C    → A is true, OR (B and C are both true)
```

### Grouping conditions

For more complex logic, use **groups** to control precedence — like parentheses in math:

```
(Priority is High  OR  Priority is Urgent)  AND  Status is not Done
```

To create a group:

1. Add the first condition you want to group.
2. Click three-dots next to the values and choose **Turn into group.**
3. Select AND or OR operator.
4. Add next rule.

Grouped conditions are visually indented in the filter bar. You can change the operator inside a group (AND or OR) independently of the operator joining groups.

To delete a rule:

1. Click three-dots next to the values in the group
2. Click **Delete**.

<figure><img src="../../../.gitbook/assets/advanced-filters (1).png" alt=""/><figcaption></figcaption></figure>

### Dynamic filter values

Filters support **dynamic values** that change based on context:

|Dynamic value   |Where it makes sense                |Example                            |
|----------------|------------------------------------|-----------------------------------|
|**Current User**|Object Property pointing to a Person|Tasks where Assignee = Current User|
|**This Object** |Inline Queries on Object Properties |Tasks where Project = This Object  |
|**Today**       |Date Property                       |Notes where Created = Today        |

**Current User** is especially useful for shared Channels — every member sees their own personalized view of a Query without you having to maintain separate Queries per person.

**This Object** works inside [Inline Lists](inline-queries.md) — it scopes the inline Query/Collection to whatever Object is hosting it. 

### Auto-open value picker

When you select a Property in the filter menu, the value picker now opens automatically — saving you an extra click. Just pick the values you want and the filter is added.

### Active filter bar

Once you have filters configured, they appear in a **dedicated bar above your view**. The Advanced Filters show how many rules are applied to the View.

To edit any active filter, click it. To remove it, click the × on the filter chip. To clear everything in one click, use the **Clear** button at the end of the bar.

### Common filter patterns

#### Tasks I'm working on right now

```
Status is In Progress  AND  Assignee is Current User
```

#### Notes from this week

```
Created is this week
```

#### Books I want to recommend

```
Rating ≥ 4  AND  Recommended-To is empty
```

#### Tasks that are blocked or stale

```
Status is Blocked  OR  (Status is In Progress  AND  Modified is before 7 days ago)
```

#### Items needing review

```
(Type is Document  OR  Type is Note)  AND  Reviewed is unchecked  AND  Created is before this week
```

## Tips

{% hint style="info" %} **Group OR conditions.** AND has higher default precedence — `A AND B OR C` may not mean what you think. Wrapping the OR in a group makes the intent explicit and unambiguous. {% endhint %}

{% hint style="info" %} **Save complex filters as separate Views.** If you've built a filter that's hard to recreate, save it as a View on your Query rather than rebuilding it each time. The Views menu makes them switchable in one click. {% endhint %}

{% hint style="info" %} **Use Current User in shared Channel templates.** A "My Tasks" Query in a team Channel works for everyone — each member sees their own tasks. No need to duplicate the Query per person. {% endhint %}