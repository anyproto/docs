# Almacenamiento

Anytype funciona prioritariamente sin conexión; por lo tanto, todos los datos que creas se guardan primero en tu dispositivo. Después, se sincronizan con el nodo de respaldo y con tus demás dispositivos para obtener redundancia. Usamos una red [IPFS](https://docs.ipfs.tech/concepts/what-is-ipfs/) privada para gestionar el almacenamiento. Se trata de un sistema de archivos entre pares (P2P) que facilita el almacenamiento descentralizado de datos entre dispositivos. Permite crear una conexión P2P de forma local, es decir, que puedes sincronizar los datos directamente entre tus dispositivos si están conectados a una misma red local. Esta conexión funcionará en cualquier modo de red, y es la única forma de sincronizar entre sí tus dispositivos cuando usas el modo solo local.

## Cómo se gestionan los archivos <a href="#media" id="media"></a>

Para ahorrar ancho de banda, los archivos de medios no se descargan directamente durante la sincronización general. En su lugar, cuando se solicita ese archivo, se transmite al dispositivo desde el nodo de respaldo o desde otros dispositivos de la misma red. Por ejemplo, si tienes un vídeo en 4K, se transmitirá a tu dispositivo desde el nodo de respaldo o desde dispositivos P2P. Cuando abres un objeto con una imagen, esta se descarga; cuando pulsas el botón de reproducción de un vídeo o audio, este comienza a descargarse. Después, ese archivo queda almacenado en la caché de la aplicación.

Además, utilizamos la función de deduplicación para reducir el almacenamiento; por ejemplo, si cargas la misma imagen tres veces, solo se almacena una de ellas.

Puedes eliminar todo el contenido multimedia de tu dispositivo móvil mediante la opción de borrar caché en iOS y Android, que eliminará todos los archivos y forzará una sincronización completa de nuevo. Como la descarga de medios funciona a demanda, al eliminar todos los medios de la caché liberarás algo de espacio.

También puedes gestionar todos tus archivos en la aplicación de escritorio desde `Ajustes del canal > Gestionar canal > Gestionar archivos`.

{% hint style="info" %}
Los archivos se almacenan en el directorio `flatfs` como fragmentos cifrados, por lo que no es posible acceder a ellos desde fuera de Anytype.
{% endhint %}

## Ubicación de almacenamiento

La **ubicación de almacenamiento** es la carpeta de tu sistema de archivos en la que Anytype guarda los datos de tu arca: los objetos, los bloques cifrados y los archivos que hayas subido, además de los índices que sirven para facilitar la búsqueda.

Por defecto, Anytype elige una ubicación estándar según tu sistema operativo; puedes elegir cualquier otra carpeta que prefieras; por ejemplo, para mover datos a una unidad más grande, a una partición cifrada o a otro sistema de archivos.

#### Configurar la ubicación durante la instalación

Cuando creas tu primera arca, la pantalla de instalación te ofrece la opción de **elegir la ubicación de almacenamiento**. Haz clic en el icono de engranaje de la parte inferior de la pantalla de bienvenida, ve a la carpeta que quieras y Anytype creará tu arca en ella.

Si omites este paso, Anytype usará la ubicación por defecto, que podrás cambiar más tarde.

#### Cambiar la ubicación después de la instalación

Para cambiar la ubicación de un arca ya existente tendrás que cerrar la sesión, elegir la nueva ubicación en la pantalla de bienvenida y volver a iniciar la sesión. Entonces, Anytype volverá a descargar los datos de tu arca desde la red a esa nueva ubicación. Sigue estos pasos: 

1. Comprueba que tienes tu clave. Esto es fundamental: sin tu clave de 12 palabras no podrás volver a iniciar sesión. 
2. Cierra la sesión en Anytype. Haz clic en el icono de tu perfil en la parte inferior de la barra lateral del arca > Cerrar sesión.
3. En la pantalla de inicio de sesión, haz clic en el icono de engranaje (⚙) de la esquina. 
4. En Ubicación de datos del arca, elige la nueva carpeta. 
5. Vuelve a iniciar la sesión. 

Anytype volverá a descargar los datos de tu arca desde la red a esa nueva ubicación. El tiempo que tarde depende del tamaño del arca y de la velocidad de tu conexión. Al terminar este proceso, estarás de nuevo en tu arca normal, con los mismos canales, objetos y datos, pero almacenados en otra carpeta.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Storage Location.jpg" alt=""><figcaption></figcaption></figure></div>

#### ¿Qué ocurre con la ubicación anterior?

Los datos de la carpeta antigua no se eliminan automáticamente. Cuando confirmes que tu arca funciona correctamente en la nueva ubicación, puedes hacer lo siguiente:

1. Abre la carpeta antigua.
2. Comprueba que contiene los archivos de datos antiguos de Anytype (verás blobs cifrados, una carpeta `index/`, etc.).
3. Elimina la carpeta manualmente.

Así liberarás ese espacio en el disco.

{% hint style="warning" %}
**No elimines la carpeta antigua hasta que hayas comprobado que la ubicación nueva se ha sincronizado por completo.**
{% endhint %}

## Unidades externas

Haz lo siguiente para almacenar tu arca en una unidad externa:

1. **Monta la unidad** antes de iniciar sesión. Anytype necesita que la unidad esté disponible en la ruta que especifiques.
2. **Elige la carpeta de la unidad** cuando selecciones la ubicación de almacenamiento.
3. **Inicia sesión normalmente.**

Esta es una buena opción si usas unidades externas fijas (un SSD externo de sobremesa o un NAS montado como volumen local). No es tan buena opción cuando se trata de unidades que se conectan y desconectan con frecuencia, por estas razones:

* Si la unidad no está montada cuando se inicie Anytype, la aplicación no podrá encontrar tu arca y mostrará un error de conexión.
* La sincronización se detendrá mientras la unidad no esté disponible.
* Algunas operaciones podrían escribir en la ubicación por defecto si la unidad externa desaparece mientras se ejecutan.

Si quieres usar un arca portátil, procura usar un SSD rápido con USB-C que tengas siempre montado mientras Anytype esté en funcionamiento.

## Volúmenes cifrados

Puedes almacenar tu arca en distintos volúmenes cifrados:

* **macOS FileVault**: funciona de forma transparente; no requiere configuración especial.
* **Windows BitLocker**: funciona de forma transparente.
* **Linux LUKS / dm-crypt**: funciona de forma transparente
* **Contenedores VeraCrypt**: compatibles, pero debes montar el contenedor antes de iniciar Anytype

Los datos de Anytype ya están cifrados en reposo mediante la clave maestra del arca derivada de tu frase de 12 palabras, por lo que el cifrado a nivel de volumen es una capa adicional, no un sustituto. Resulta útil si quieres una defensa en profundidad o si te preocupa que otras aplicaciones del dispositivo lean los nombres de archivo o los metadatos de sincronización.

## Modo solo local

Si eliges el modo de red [solo local](sync-and-backup/local-only.md) (en los ajustes iniciales del arca > Red), tu arca no se sincroniza con ningún servidor remoto. Los datos se guardarán únicamente en la ubicación de almacenamiento que selecciones y en los otros dispositivos que sincronices mediante una conexión local entre pares. Encontrarás más detalles [aquí](sync-and-backup/local-only.md).

{% hint style="danger" %}
**En el modo solo local, tu ubicación de almacenamiento es la única copia de tus datos**. Trata esa carpeta como un original muy preciado: haz copias de respaldo con regularidad y nunca la dejes en un lugar provisional (como un directorio temporal o una unidad sin montar).
{% endhint %}
