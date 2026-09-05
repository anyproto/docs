# API local

La versión 0.46.X marca un momento interesante y muy esperado en la evolución de Anytype: **la primera iteración de nuestra API local**, que abre posibilidades muy potentes para un ecosistema de plugins, automatizaciones e integraciones de terceros.

Nuestra API está incluida directamente en la aplicación de escritorio y se ejecuta por completo en el host local. Funciona sin conexión, lo que significa que puedes crear y usar integraciones sin depender de ningún servicio en la nube, incluso durante un vuelo.

{% hint style="danger" %}
**Aviso de seguridad importante:** Cuando proporcionas una clave de API o usas extensiones, concedes acceso limitado a tu arca de Anytype para realizar operaciones como modificar o eliminar objetos. Asegúrate de **usar solo extensiones de confianza**.
{% endhint %}

## Aspectos destacados

* **Autenticación segura:** autentícate una sola vez mediante un desafío de 4 dígitos en la aplicación de escritorio y genera una clave de API. Esta clave actúa como token de portador para autenticar las solicitudes posteriores. Además, las claves API se pueden gestionar y generar directamente desde los ajustes del cliente de escritorio, de modo que es fácil compartirlas con integraciones de terceros.
* **Documentación completa:** la especificación de OpenAPI y la documentación completa están publicadas en nuestro nuevo [portal para desarrolladores](https://developers.anytype.io/).
* **Capacidades potentes de API:** los endpoints ofrecen la funcionalidad principal de Anytype: crear objetos, editar, consultar y mucho más.
* **Ecosistema creciente de desarrolladores:** ya están en marcha los primeros SDK y herramientas impulsadas por la comunidad, como clientes de Python y Go, servidor MCP y extensión de Raycast.

## Obtén una clave de API local

1. Ve a tus [Ajustes del arca](../../settings/vault-settings.md). 
2. En la sección «Gestión de datos», selecciona «Claves de API». 
3. Haz clic en el botón «Crear nuevo». 
4. Da un nombre a la clave. 

Puedes generar tantas claves como necesites y revocar el acceso cuando quieras. 

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Integration API Revoke.jpg" alt=""><figcaption></figcaption></figure></div>