# Sincronización y respaldo

Anytype se basa en los principios _local-first_ (prioridad local) para combinar la fluidez de las aplicaciones en la nube actuales con la privacidad, la seguridad y la propiedad absoluta del software local.

Todo lo que creas reside en tus dispositivos, cifrado con claves que solo tú controlas. Nuestra infraestructura gestiona de forma automática la sincronización en segundo plano y las copias de respaldo para que conserves la plena propiedad de tus datos sin arriesgar tu soberanía.

## Qué significa esto

En el pasado, el software local ofrecía propiedad y privacidad completas: lo que hacías era asunto tuyo y de nadie más. Pero esto tenía un precio: la colaboración era muy complicada.

Internet ofreció una solución: la tecnología de la nube nos permitía colaborar en tiempo real; pero, por el camino, cedimos nuestra privacidad, seguridad y propiedad a las propias aplicaciones.

Con Anytype, no tienes que elegir uno de los dos modelos. Conservas la propiedad y el control total de tus datos en todo momento, mientras usas internet para sincronizar entre dispositivos y colaborar con otras personas.

Es lo mejor de ambos mundos: propiedad local y colaboración en la nube.

## Cómo funciona

A grandes rasgos, Anytype pone el control en tus manos de tres maneras:

{% stepper %}
{% step %}
### Todo es local

Todo el contenido se almacena en tu dispositivo; incluso las claves de acceso se generan en tu propio hardware. Por esta razón, la aplicación funciona prioritariamente sin conexión a internet y te protege frente a interrupciones del servicio, bloqueos de acceso y dependencia de proveedores.
{% endstep %}

{% step %}
### Sincronización cifrada de extremo a extremo

Antes de que ningún dato salga de tu dispositivo, se cifra para que solo se pueda desbloquear con tu clave. La red de Anytype funciona como un «orquestador ciego» que transmite actualizaciones entre tus dispositivos sin capacidad para ver el contenido o acceder a él. Aunque alguien interceptara tus datos cifrados, ni los atacantes mejor preparados del mundo podrían descifrarlos. Es algo que se puede verificar en el código de Anytype, abierto a la constante inspección pública.
{% endstep %}

{% step %}
### Recuperación integrada

Para evitar que pierdas tus datos, la red de Anytype guarda en remoto una copia de respaldo cifrada. Tu clave privada es la única forma de descifrarla y restaurarla en un dispositivo nuevo; nadie más, ni siquiera Anytype, puede acceder a tus datos cifrados. Tener todo el control en tus manos también significa que tienes toda la responsabilidad sobre las [claves](../../basics/key.md) que te dan acceso a tus datos y te permiten recuperarlos.
{% endstep %}
{% endstepper %}

Anytype es un refugio seguro para tu vida digital. Tienes más información sobre la forma de colaborar en [Colaboración](../../collaborate/collaboration.md).

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs E2EE Sync.gif" alt=""><figcaption></figcaption></figure></div>

## Red de Anytype

Por defecto, todo el mundo se incorpora a la red de Anytype, lo que llamamos «sincronización con base local». Anytype proporciona a todos los usuarios un nodo de respaldo remoto con almacenamiento gratuito, que puede ampliarse con una suscripción.

Los objetos y la estructura no consumen este espacio, de modo que nunca encontrarás restricciones para crear y editar páginas ni perderás el acceso a tus datos. Lo único que ocupa espacio de almacenamiento son los archivos, como las imágenes y las vídeos. Si superas tu límite, verás una advertencia y podrás solicitar más espacio de almacenamiento. Aunque hayas superado el límite, podrás seguir usando la aplicación; la diferencia estará en que los nuevos archivos no se sincronizarán entre tus dispositivos.

Mientras usas la sincronización local en la red de Anytype, puedes trabajar completamente sin conexión y sincronizar a través de tu red local de par a par (P2P). Piensa en la red de Anytype como un sistema de respaldo: puedes trabajar sin conexión, sincronizar de forma local y, cuando vuelvas a conectarte, la red iniciará la sincronización y guardará una copia de respaldo.

#### ¿Dónde se almacenan las copias de respaldo remotas?

Nuestra infraestructura está alojada en servidores dedicados de centros de datos de la Unión Europea. Estos son los dominios que utilizamos para la red de Anytype:

* Sincronización: `*.anyclub.org`
* Análisis: `*.anytype.io`

## Cómo usar la red de Anytype

Por defecto, estarás en la red de Anytype. Si estabas usando otro modo de sincronización y quieres volver a la red de Anytype, deberás hacerlo manualmente en todos los dispositivos. 

Te recomendamos encarecidamente que uses una identidad distinta para cada red. Si vas a cambiar desde una red autoalojada, exporta todos tus canales e impórtalos a una identidad nueva antes de cambiar el modo de red.

#### Escritorio

1. Cierra la sesión de tu identidad actual.
2. En la pantalla de incorporación, haz clic en el icono de engranaje de la esquina superior derecha.
3. En el campo «Red», elige la opción «Anytype».
4. Haz clic en el botón «Guardar».
5. Crea una identidad nueva o inicia sesión con una existente.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure></div>

#### Móvil

1. Cierra la sesión de tu identidad actual.
2. En la pantalla de incorporación, haz clic en el icono de engranaje de la esquina superior derecha.
3. En el submenú «Redes», haz clic en «Anytype».
4. Crea una identidad nueva o inicia sesión con una existente.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Screenshot_20240411-104810_Anytype2.png" alt="" width="375"><figcaption></figcaption></figure></div>

## Métodos de sincronización alternativos

Anytype también admite dos modos se sincronización alternativos:

* [Autoalojado](self-host.md): usa tu propia infraestructura para alojar y sincronizar tus datos de Anytype.
* [Solo local](local-only.md): tus datos se quedan en el dispositivo y no usan ningún servidor para la sincronización.

Te recomendamos que te quedes en la red de Anytype por defecto y su sincronización con prioridad local, y que solo cambies a uno de estos modos si cuentas con los conocimientos técnicos necesarios para administrarlos.

#### Servicios de terceros y unidades de red

No coloques tu directorio de datos de Anytype en ninguna carpeta sincronizada con una nube de terceros (como Nextcloud, Dropbox, OneDrive o Google Drive) ni en una unidad de red compartida. Esto pondría en grave riesgo tu privacidad y la integridad de tus datos.

1. **Riesgo alto de deterioro de la base de datos**: Anytype usa bases de datos SQLite para almacenar tus espacios en el dispositivo. Las herramientas de sincronización en la nube monitorizan los archivos y los bloquean cuando detectan cambios. Cada vez que una herramienta de sincronización accede a archivos SQLite activos, interfiere con el bloqueo de archivos de la base de datos, sobre todo cuando hay varios dispositivos escribiendo al mismo tiempo. Esto puede provocar un deterioro irreversible de la base de datos, daños en los índices de búsqueda y un fallo definitivo del arca.
2. **Filtración de datos privados**: aunque tu contenido principal está cifrado, el directorio de trabajo de Anytype también contiene índices locales sin cifrar que son imprescindibles para el rendimiento de la aplicación y la función de búsqueda. Si sincronizas esa carpeta con una nube de terceros, se envían estos archivos sin cifrar, exponiendo tus metadatos privados y datos de índice ante el proveedor.

**Cómo almacenar tus datos de forma segura**

* Usa solo el almacenamiento local: asegúrate de que tu directorio de datos de Anytype se encuentre en una unidad normal y no sincronizada de tu dispositivo; es decir, en tu almacenamiento interno estándar.
* Copias de respaldo manuales: si quieres usar un almacenamiento en la nube para las copias de respaldo, exporta tus espacios manualmente o haz una copia de respaldo de una instantánea estática y cerrada del directorio mientras Anytype no esté en ejecución.

{% hint style="danger" %}
**No uses unidades de red ni servicios de terceros para sincronizar**: es muy probable que esto cause daños en los datos. [Tienes más información aquí](#servicios-de–terceros-y-unidades-de-red). 
{% endhint %}
