---
description: Totales y recuentos en la vista de cuadrícula.
---

# Fórmulas

Las **fórmulas** te permiten resumir y agregar los valores de las propiedades de los objetos en una consulta o colección. Cuando tienes los datos en una vista de cuadrícula, puedes mostrar recuentos, sumas, promedios, mínimos, máximos y otros cálculos al final de cualquier columna.

Así obtienes una fila de totales bajo los datos que puede servirte para ver este tipo de cosas:

* el total de horas estimadas para todas las tareas de un sprint,
* la valoración media de todos los libros de tu lista de lectura,
* el número de tareas en curso de cada responsable,
* una suma de gastos por categoría,
* un recuento de los objetos de cada tipo.

<figure><img src="../../../.gitbook/assets/formulas.png" alt=""><figcaption></figcaption></figure>

## Dónde aparecen las fórmulas

Las fórmulas se encuentran en la **parte inferior de cada columna en la vista de cuadrícula**. Cada columna puede tener su propia fórmula y mostrar un cálculo distinto.

Para abrir el menú de fórmulas:

1. Abre una consulta o colección en **vista de galería**.
2. Haz clic en el nombre de la propiedad en la cabecera de una columna.
3. Selecciona # **Calcular** en la parte inferior del menú.
4. Elige una opción.

El resultado aparece en el pie de columna y se actualiza cuando cambian los datos.

<figure><img src="../../../.gitbook/assets/formulas (1).png" alt=""><figcaption></figcaption></figure>

## Fórmulas disponibles

Las fórmulas disponibles dependen del formato de la propiedad de esa columna. Esta es la lista completa:

#### En todos los formatos de propiedad

| Fórmula                 | Cálculo                                    |
| ----------------------- | ---------------------------------------------- |
| **Ninguno**                | Sin fórmula (por defecto)                   |
| **Recuento**               | Número total de objetos en la columna          |
| **Contar valores únicos** | Número de valores distintos                      |
| **Contar vacíos**         | Número de objetos sin ningún valor en esta columna |
| **Contar no vacíos**     | Igual que Contar valores                           |
| **Porcentaje vacíos**       | % de objetos sin ningún valor                     |
| **Porcentaje no vacíos**   | % de objetos con algún valor                      |

#### En propiedades numéricas (matemáticas)

| Fórmula     | Cálculo       |
| ----------- | ------------------------ |
| **Suma**     | Total de todos los valores      |
| **Promedio** | Media de todos los valores               |
| **Mediana**  | Valor central al ordenar |
| **Mínimo** | Valor más bajo        |
| **Máximo** | Valor más alto         |
| **Intervalo**   | Máximo − Mínimo          |

## Limitaciones

* **Las fórmulas son solo visuales**: aparecen en el pie de la columna, pero no puedes hacer referencia a ellas en otro objeto ni usarlas en filtros.
* **No hay expresiones personalizadas**: tienes que elegir una de la lista de fórmulas disponibles; no hay forma de escribir `columna1 + columna2`.
* **Solo en la vista de cuadrícula**: otros diseños (Lista, Galería, Kanban) no muestran fórmulas.
* **Dependen de la vista**: cada vista guarda su propia selección de fórmulas; en una misma consulta, la vista de cuadrícula y la de lista no comparten las fórmulas.

Para realizar cálculos más complejos, exporta los datos a CSV y procésalos externamente, o usa la [técnica (skill) de Anytype para agentes](../../features/integrations/anytype-agents-skill.md) para ejecutar scripts con tus datos.

## Modelos frecuentes

#### Estimación de horas del sprint

```
Consulta: Tareas
Filtro: Sprint = «Sprint 14»
Propiedad: Horas estimadas (número)
Fórmula: Suma
```

#### Estadísticas de lectura

```
Consulta: Libros
Propiedad 1: Valoración (Número) → Fórmula: Promedio
Propiedad 2: Páginas (Número) → Fórmula: Suma
Propiedad 3: Estado (Selección) → Fórmula: Contar por opción
```

#### Cartera de proyectos

```
Consulta: Proyectos
Agrupar por: Estado
Propiedad: Presupuesto (número) → Fórmula: Suma (por grupo)
```
