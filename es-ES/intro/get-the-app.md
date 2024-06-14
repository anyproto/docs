# Obtén la aplicación

Puedes descargar la versión más reciente de Anytype para tu dispositivo desde [download.anytype.io](https://download.anytype.io).

{% hint style="info" %}
Anytype es una aplicación independiente que funciona en dispositivos de escritorio o móviles. No existe una versión de la aplicación que necesite el navegador. Las aplicaciones de navegador tienen muchos puntos de vulnerabilidad que pondrían en riesgo nuestro compromiso con la seguridad y el cifrado de los datos.
{% endhint %}

### Requisitos mínimos

* En las versiones de escritorio usamos Electron, que depende de las directrices de soporte de los proveedores. Por ejemplo, ya no admitimos Windows 7 ni Windows 8.1 porque Microsoft ya no les da soporte.
* En Android (si se instala desde Google Play), el mínimo es Android 8.0 y un dispositivo de 64 bits con 4 GB de RAM.
* En iOS es iOS 16.

### Ubicación de instalación

Anytype se instala en las siguientes ubicaciones:

* En Windows 10 o superior, suele ser\
  `C:\Users\<usuario>\Appdata\Local\Programs\anytype2\Anytype.exe`\
  **usuario** es el nombre de tu usuario, es decir, tu directorio de trabajo.&#x20;
* En MacOS es ` HHD > Users >`` `` `_`usuario`_` `` ``> Library > Application Support > anytype `
* En Linux, el directorio de trabajo está en `~/.config/anytype`
* En Android es la ubicación por defecto, normalmente \_device/data/app\_​.\
  También guardamos algunas cachés en _device/data/data/io.anytype.app_\
  El directorio de Anytype se guarda en una carpeta de datos de aplicación protegida a la que no puede acceder el usuario del dispositivo Android.
* En iOS es la ruta de instalación normal, determinada por iOS.

### Ubicación de almacenamiento personalizada

En el momento de crear un arca se puede seleccionar la ubicación de almacenamiento en la unidad de disco. Si ya has creado tu arca, también puedes cambiar la ubicación y después recuperar los datos desde la red. Para hacerlo, cierra la sesión y luego pulsa el icono de los ajustes (rueda dentada) en la pantalla de inicio de sesión.

<figure><img src="../../.gitbook/assets/Custome Storage Location.gif" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="danger" %}
Ten precaución cuando uses el modo solo local, ya que los datos solo se podrán transferir a otro dispositivo por medio de una conexión directa entre dispositivos (P2P).
{% endhint %}

#### Unidades externas y proveedores de nube&#x20;

Para almacenar tus datos en una unidad externa, solo tienes que montar la unidad y seguir los pasos de [Ubicación de almacenamiento personalizada](get-the-app.md#custom-storage-location "mention").

No te recomendamos que uses proveedores de nube como Google Drive o iCloud porque podrías experimentar problemas y conflictos de sincronización.
