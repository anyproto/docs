# Privacidad y cifrado

La mayor parte del software actual se ejecuta en servidores corporativos en la nube, donde las empresas pueden ver tus datos, sacar provecho de ellos e impedirte el acceso cuando quieran. En esencia, necesitas su permiso para acceder a tu propia vida digital.

Anytype es distinto desde la base: nadie más que tú tiene o tendrá la propiedad de tu mundo digital. La soberanía digital no es una característica de Anytype, sino el principio fundamental de su diseño.

## Privacidad

La arquitectura de Anytype está ideada de forma que la privacidad se aplica matemáticamente mediante código, no mediante promesas en una política. Esto es lo que eso implica en la práctica:

* **Tú controlas el acceso.** Nadie más que tú puede acceder a tus espacios y permitir el acceso a otros; ni siquiera Anytype puede ver tu contenido.
* **No necesitas permisos.** No necesitas la aprobación de nadie para acceder a tus datos; ni siquiera la de Anytype.
* **Puedes irte cuando quieras.** Tus datos se van contigo y Anytype no puede impedírtelo.

#### Cómo funciona

* **Generación de clave local.** Tu [clave](../basics/key.md) criptográfica se genera localmente en tu dispositivo cuando creas el [arca](../basics/vault.md). Nunca se transmite por internet ni se almacena en los servidores de Anytype: solo la tienes tú.
* **No hay un sistema central de recuperación.** Puesto que Anytype no tiene ninguna clave de tu cuenta, no puede restablecer tu contraseña ni facilitarte la recuperación de una cuenta a la que no consigues acceder. Si pierdes la clave, pierdes el acceso a tus datos de forma definitiva.
* **Sincronización ciega.** Todos los datos y el contenido se cifran antes de sincronizarlos entre dispositivos, de modo que Anytype solo actúa como un mensajero ciego que transporta un mensaje sin poder leerlo.

{% hint style="warning" %}
**Comparte tus espacios confidenciales solo con personas de confianza que también usen dispositivos seguros.** Cada miembro que añades a un espacio aumenta su superficie de riesgo.
{% endhint %}

## Cifrado

Anytype cifra tus datos empleando un sistema de claves superpuestas, por lo que ni siquiera son legibles para la infraestructura de sincronización y respaldo. Esto es lo que eso implica en la práctica:

* **Los objetos están cifrados en reposo.** Tanto en tu dispositivo como en los nodos de sincronización, los objetos se almacenan en un formato cifrado que solo se puede decodificar con las claves de cifrado. Tus claves se generan localmente, en tu dispositivo, y nunca se envían a Anytype.
* **Los índices son locales y no están cifrados.** Para buscar en tus documentos de forma eficaz, Anytype crea índices locales a partir de tus objetos cifrados, que descifra sobre la marcha empleando tus claves. Estos índices se almacenan aparte de los datos cifrados y no están cifrados en sí mismos; se supone que tu dispositivo local es seguro.
* **Los índices no se sincronizan nunca.** Tus índices solo residen en el dispositivo que los crea. Si usas dos dispositivos, cada uno almacena su propio índice por separado.

#### Cómo funciona

El cifrado de Anytype es potente, pero, en última instancia, tu privacidad depende de la seguridad de tu dispositivo. Si el dispositivo está expuesto, la protección del cifrado local contra ataques se reduce. Te recomendamos que te tomes muy en serio la seguridad de tus dispositivos con medidas como las siguientes:

1. Usa una contraseña de acceso al dispositivo.
2. Habilita el cifrado de disco.
3. Bloquea el dispositivo cada vez que lo dejes desatendido.
4. No compartas el acceso al dispositivo.

<details>

<summary>Detalles técnicos</summary>

* Anytype guarda un historial de cambios de todos los objetos que creas.
* Cada cambio realizado en el objeto tiene dos capas de cifrado con distintas claves.
* La primera capa sirve para relacionar los cambios con el objeto, es decir, «todos estos datos cifrados pertenecen al objeto con el identificador \<abc>».
* La segunda capa es la que cifra los datos en sí. Usamos AES con cifrado de flujo en modo CFB.
* Los cambios que realizas en un objeto se envían regularmente a nuestro nodo de respaldo empleando solo la clave de la primera capa. Tienes más información sobre la sincronización [aquí](https://tech.anytype.io/any-sync/overview).
* Los nodos de respaldo de Anytype tienen acceso a la clave de primera capa, por lo que pueden agrupar los cambios del objeto y enviarlos en un paquete cuando quieras restaurar tus datos.
* Los nodos de respaldo de Anytype no tienen acceso a la segunda capa, por lo que no pueden leer los cambios de los datos.

Encontrarás más detalles técnicos [aquí](https://tech.anytype.io/any-sync/overview?id=encryption).

</details>

{% hint style="warning" %}
**Mantén seguros tus dispositivos.** Cuando usas Anytype, la seguridad de tus dispositivos y de tus hábitos de uso es la primera línea de defensa y la más importante.
{% endhint %}

## Telemetría

Aunque tu contenido siempre es privado y está cifrado, Anytype recopila datos de uso del producto anonimizados y limitados para entender cómo se usa la app y orientar el desarrollo. Estos datos de telemetría son independientes por completo de tu contenido real.

Esto es lo que eso implica en la práctica:

* **El contenido nunca forma parte de la telemetría.** Nunca son visibles para la telemetría ni los títulos ni los contenidos de objetos, mensajes de chat y archivos. Tus espacios siguen siendo igual de privados para ti y para quienes los comparten contigo.
* **Los datos de uso son anónimos y se visualizan de forma agregada.** Podemos ver señales de alto nivel, pero no detalles concretos. Por ejemplo, podemos ver cuántos usuarios han creado tipos personalizados, pero no lo que contienen esos tipos ni la forma en que se usan.
* **Los datos están compartimentados.** Los análisis del producto y las herramientas de correo electrónico se mantienen por separado, sin que haya ningún vínculo de datos identificables entre ambos. Las direcciones de correo electrónico recopiladas en el sitio web o durante el proceso de incorporación no están vinculadas a tu arca ni a la telemetría de ninguna forma.
* **Los datos se abstraen.** Ponemos especial cuidado en conseguir que la telemetría sea lo más abstracta posible; por ejemplo, se crean ID de canal sintéticos en lugar de usar los ID reales. Esto es un impedimento más para cualquier posibilidad de interpretar lo que ocurre en un espacio.
* **No se vende nada.** Los datos de uso nunca se venden a terceros; solo se utilizan para orientar las decisiones internas sobre el producto.

## Correos electrónicos de usuario

Las cuentas de Anytype no requieren permisos y se crean por medio de una frase semilla, sin necesidad de usar un correo electrónico. Cuando recopilamos correos electrónicos en solicitudes de soporte técnico, boletines y registros en la web, tomamos medidas para aislarlos de sus arcas y de nuestras herramientas.

* **Compartimentación estricta**: las herramientas que empleamos para el correo electrónico están separadas de las herramientas de análisis del producto y no comparten datos.
* **Sin entrecruzamiento**: aunque nuestros análisis muestren que 1000 usuarios han abandonado Anytype, como nuestros sistemas no están interconectados, no podemos enviarles mensajes de reenganche.

Adoptamos todas las precauciones posibles para evitar la pérdida del anonimato, pero es aconsejable que los usuarios tomen sus propias medidas.

* Alias de email: usa servicios como SimpleLogin o DuckDuckGo cuando te pongas en contacto con nuestro soporte técnico.
* VPN: enmascara tu dirección IP durante las sincronizaciones al nodo.
* Autoalojamiento: mantén tu propia infraestructura si quieres tener los datos completamente aparte de los nodos de Anytype.

Para solicitudes relacionadas con el RGPD, es decir, la eliminación de datos de otros servicios, puedes escribirnos a [gdpr@anytype.io](mailto:anylab@anytype.io).
