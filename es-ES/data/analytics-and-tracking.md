# Analítica y seguimiento

Mientras el producto está en su versión preliminar, empleamos servicios de análisis para conocer mejor el rendimiento general de la aplicación, la adopción de determinadas funciones y cómo esto afecta a la retención. [Tienes más información aquí](privacy-and-encryption.md#telemetria).

La analítica consta de dos partes: análisis de bajo nivel en la red y análisis de uso de la aplicación en el cliente. Ambas partes son anónimas y no analizan el contenido con el que trabajas, ya que está cifrado.

## Seguimiento de uso

El servicio principal que empleamos para rastrear eventos en la aplicación es **Amplitude**. Nos permite hacer un seguimiento de métricas como las siguientes:

* cuántos usuarios se incorporaron el mes pasado y cuántos han abandonado Anytype;
* cuántos objetos, bloques, conjuntos y tipos personalizados se crearon (y la media según el número de usuarios activos);
* cuánto tiempo, de media, dedican los usuarios a la aplicación;
* qué dispositivos se usan para acceder a la aplicación.

Estas métricas nos sirven para comprender mejor nuestro producto y ver si nos movemos en la dirección adecuada. Aunque detectamos la frecuencia de los eventos y su nivel de adopción, no podemos ver de ninguna manera el contenido que creas.

Esto nos permite saber, por ejemplo, que los usuarios crean bastantes tipos personalizados, pero no nos dice cuáles son esos tipos ni qué objetos se crean con ellos.

Además de Amplitude, nuestros equipos de ingeniería usan Sentry para conocer la frecuencia de los fallos.

{% hint style="info" %}
Si cambias al modo de red autoalojado o solo local, la red de Anytype no recopila análisis de bajo nivel, aunque seguirán realizándose análisis de uso de la aplicación.
{% endhint %}

{% hint style="info" %}
Podrás desactivar estos análisis [en el futuro](https://github.com/orgs/anyproto/projects/1/views/1?pane=issue\&itemId=29227689).
{% endhint %}

{% hint style="info" %}
Por el momento, la única forma de deshabilitar los análisis es bloquear las conexiones salientes a los hosts relacionados con los análisis, aunque también puedes editar el código fuente correspondiente y recompilar el cliente para tu propio uso.
{% endhint %}

Para solicitudes relacionadas con el RGPD, es decir, la eliminación de datos de otros servicios, puedes escribirnos a [gdpr@anytype.io](mailto:anylab@anytype.io).
