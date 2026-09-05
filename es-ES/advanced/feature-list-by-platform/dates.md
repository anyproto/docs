---
description: Las fechas funcionan como objetos, propiedades y referencias en Anytype.
---

# Fechas

En Anytype, **cada fecha es un objeto** por sí misma. Cuando escribes una mención como `@today` (hoy), rellenas la propiedad «Fecha final» o abres una vista de calendario, las fechas no son solo texto o metadatos, sino que existen en tu canal como objetos de fecha que puedes abrir, añadir como enlaces y usar como contenedor de todo lo que ocurre ese día.

Haz clic en una fecha en cualquier lugar (el valor de una propiedad, una mención, un cuadro del calendario) y se abrirá el objeto de fecha. Esto es lo que verás en él:

* todos los objetos que mencionan esa fecha,
* todos los objetos creados en esa fecha,
* todos los objetos con una propiedad de formato «Fecha» que contiene ese día,
* mensajes de debates y chats enviados en esa fecha.

De esta forma, el objeto de fecha actúa como un **índice temporal**, una página que muestra todo lo que tiene relación con un momento determinado.

<figure><img src="../../../.gitbook/assets/date.png" alt=""><figcaption></figcaption></figure>

## Formas en que aparecen las fechas

En Anytype, las fechas aparecen de tres formas:

#### 1. Menciones en el texto

Teclea `@fecha` o `/fecha` para abrir el selector de fecha y elegir una fecha (o hacer clic en **Hoy**).

La mención aparecerá como una fecha en la que puedes hacer clic para abrir el objeto de fecha correspondiente.

#### 2. Propiedades de fecha

Puedes añadir a cualquier tipo una propiedad con formato de fecha, como una fecha final, de inicio, de publicación, de última revisión, de cumpleaños… La propiedad acepta la fecha del día y, opcionalmente, la hora:

* **solo fecha**, ideal para vencimientos, cumpleaños, plazos;
* **fecha y hora**, ideal para reuniones, eventos, registros horarios.

Haz clic en el cuadro de la propiedad de fecha de un objeto para abrir el selector de fecha y elegir una.

#### 3. Propiedades de fecha automática

Todos los objetos tienen ciertas propiedades de fecha integradas que establece Anytype de forma automática:

* **Creation date**: fecha de creación del objeto (invariable).
* **Last modified date**: fecha de los últimos cambios en el objeto.
* **Last opened date**: última fecha en que se abrió el objeto (en ese dispositivo).

Puedes hacerlas visibles u ocultarlas en las vistas, usarlas en los filtros y criterios de orden, y referirte a ellas en fórmulas.

## Fecha como objeto

Haz clic en una fecha (en una propiedad de fecha, una mención o un cuadro del calendario) para abrir el objeto de fecha y verás lo siguiente:

* **Menciones a esa fecha**: todas las menciones con `@` a esa fecha en todo el canal.
* **Objetos con esa fecha como valor de una propiedad**: todos los objetos que tienen alguna propiedad de fecha con ese valor.
* **Objetos creados en esa fecha**: agrupados automáticamente en «Fecha de creación».
* **Objetos modificados en esa fecha**: agrupados automáticamente en «Fecha de última modificación».

Cada sección contiene una lista en la que puedes ver y abrir los objetos. También puedes añadir notas directamente al objeto de fecha, como una entrada de diario, un plan para empezar el día o apuntes de una reunión que quedarán asociadas siempre a ese día.

### Vista de calendario

Cualquier consulta o colección que incluya una propiedad de fecha puede tener una **vista de calendario**. Haz clic en el selector de diseño y elige **Calendario**:

* Los objetos aparecerán en la fecha correspondiente a la propiedad seleccionada.
* Haz clic en un objeto para abrirlo.
* Haz clic en un cuadro vacío del calendario para crear un objeto en esa fecha.
* Arrastra objetos a otra fecha para modificar la propiedad de fecha.

La propiedad que sirve para organizar el calendario se elige en los ajustes de la vista; por ejemplo, un calendario de tareas podría usar **Fecha final**, mientras que un calendario de entradas de diario usaría **Fecha de creación**.

### Formato de fecha según la configuración regional

Las fechas de los filtros y selectores respetan la configuración regional de tu sistema operativo. Si tu sistema usa MM/DD/YYY, eso es lo que verás; si usa DD/MM/AAAA, las verás en ese formato.

Puedes elegir el formato que prefieras en los **ajustes del arca > Aplicación > Idioma y región > Formato de fecha y hora**.

En esa sección puedes configurar estos ajustes:

* Formato de fecha (DD/MM/YYYY, MM/DD/YYYY, YYYY-MM-DD, etc.).
* Formato de hora (12 horas o 24 horas).
* Usar fechas relativas (hoy / mañana) o siempre fechas literales.
* Día en que empieza la semana (domingo o lunes).

## Notas

{% hint style="info" %}
**Usa propiedades de fecha para las líneas de tiempo del proyecto.** Un objeto de proyecto con propiedades de fecha de inicio, fecha prevista y fecha de finalización te permite crear una vista de línea de tiempo que se actualiza según avanza el trabajo.
{% endhint %}
