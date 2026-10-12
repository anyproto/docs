# Vista general

Anytype for Business es una aplicación independiente de Anytype para equipos. Incluye las siguientes funciones:

* **Inicio de sesión con tu cuenta de trabajo:** Google, proveedor de identidad de la empresa (OIDC) o un código por correo electrónico.
* **Gestión centralizada de miembros:** los propietarios y administradores añaden y eliminan personas, asignan roles y controlan el acceso a los espacios.
* **Consola de administración:** una aplicación web en [business-api.anytype.io/admin](https://business-api.anytype.io/admin/) para gestionar la organización.

La aplicación funciona en Windows, macOS, Linux, iOS y Android. Se descarga por separado y tiene sus propias cuentas, distintas de las de Anytype personal. Para obtenerla, haz clic en **Download Anytype** en la consola de administración.

{% hint style="info" %}
Aún no hay un botón para iniciar sesión con Microsoft. Puedes conectar Microsoft Entra ID como [proveedor de SSO personalizado](sign-in/custom-sso.md).
{% endhint %}

## Por qué es una aplicación independiente

Anytype personal funciona con conocimiento cero. Tus claves nunca salen de tus dispositivos y nadie más puede leer tu contenido, ni siquiera nosotros.

En Anytype for Business, inicias sesión con tu cuenta de trabajo, no con una clave de recuperación. Para hacerlo posible, un servicio llamado **nodo de autenticación** almacena las claves cifradas de tu equipo y le entrega tu clave a la aplicación cuando inicias la sesión.

* **Nodo alojado en Anytype (nube):** nosotros gestionamos el nodo de autenticación, por lo que técnicamente tenemos la posibilidad de acceder a tu contenido. Nuestra política nos impode hacerlo.
* **Nodo autoalojado (próximamente):** tu empresa ejecuta el nodo de autenticación en sus propios servidores y controla las claves. Escríbenos a [business@anytype.io](mailto:business@anytype.io) para recibir notificaciones sobre esta opción.

La razón por la que son aplicaciones distintas es que sería imposible incluir en una sola aplicación ambos modelos de autenticación sin poner en riesgo la privacidad de los usuarios personales.

## Funciones

| Función | Permisos |
| --- | --- |
| **Propietario** | Todos los de los administradores, además de configurar el SSO, la incorporación automática con Google Workspace, las directivas de la API local y la suscripción. Cada organización tiene un solo propietario. |
| **Administrador** | Invitar a miembros, eliminarlos y hacerlos administradores; crear espacios y gestionar sus miembros; gestionar la facturación (el propietario puede deshabilitarlo). |
| **Miembro** | Usar Anytype, trabajar en sus espacios y acceder a los espacios públicos de la organización. |

Las funciones de los espacios (visitante, editor, administrador) son distintas de las de la organización. Consulta [Espacios](spaces.md).

## Precios

20 € por editor al mes, o un 20 % menos con facturación anual. Un editor es cualquier persona que puede editar al menos en un espacio. Los miembros que solo pueden leer (visitantes) son gratuitos.

Las organizaciones nuevas tienen un periodo de prueba gratuito. Cancela la suscripción antes de 30 días para obtener un reembolso completo. Consulta [Facturación](org-settings.md#billing).
