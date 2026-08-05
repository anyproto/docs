# Clave

En el momento de crear tu cuenta en Anytype, recibes tu propia clave, que se genera localmente en tu dispositivo. Es la única forma de acceder a tu arca y descifrar tus datos, como una combinación de tu correo y contraseña de inicio de sesión.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Welcome 3.jpg" alt=""/><figcaption></figcaption></figure></div>

## Cómo funciona

Tu clave es una cadena de 12 palabras, lo que también se conoce como frase mnemotécnica, frase semilla o frase de recuperación. Esta combinación única de palabras comunes conforma una clave criptográfica muy segura. En lugar de una cadena de caracteres aleatorios, se utilizan palabras porque resulta más sencillo escribirlas, leerlas y comprobarlas. Es el mismo método que usan los monederos de criptomoneda como Bitcoin.

En la trastienda, estas 12 palabras codifican una clave maestra que cifra y descifra todo el contenido de tu arca. Matemáticamente, hay más combinaciones posibles que átomos en el universo observable, por lo que, en la práctica, es imposible averiguar tu clave.

Esta clave no se puede cambiar; se genera de forma local y está vinculada intrínsecamente a tu cuenta. Por eso es fundamental mantenerla a buen recaudo: ni siquiera Anytype puede ayudarte si tu clave queda expuesta.

## No olvides guardar tu clave

Anytype no guarda ninguna copia de tu clave, así que, si la pierdes, no podemos ayudarte a recuperar tu arca. Te recomendamos encarecidamente que hagas una copia de seguridad, ya que necesitarás esta clave cada vez que inicies sesión en un dispositivo nuevo.

Para encontrar tu clave en los [ajustes de tu arca](../settings/vault-settings.md):

1. Haz clic en la imagen de tu perfil, en la esquina inferior izquierda.
2. Haz clic en **Clave de acceso** en el menú de la izquierda.
3. Haz clic en el icono del ojo para ver tu frase de 12 palabras.

## Qué ocurre si pierdes la clave

La ventaja de usar una clave es que puedes acceder a Anytype y colaborar con otras personas sin necesitar el permiso de nadie, ni siquiera de Anytype. Pero ese mismo diseño deja en tus manos toda la responsabilidad sobre tus datos.

Anytype no puede identificar un arca, conceder acceso a ella o eliminarla. Aunque fuera posible, no tendríamos forma de verificar si estamos hablando con la persona propietaria del arca o con alguien que se hace pasar por ella. La privacidad y el anonimato que te ofrece Anytype son la razón por la que tu clave está bajo tu exclusiva responsabilidad.

Si tu sesión se cierra sin que hayas guardado tu clave en otro sitio, puedes probar lo siguiente:

* Usa otro dispositivo. Si aún tienes la sesión iniciada en otro dispositivo, abre la aplicación allí y copia tu clave desde los ajustes.
* También puedes intentar recuperar tu clave desde el [almacén de claves del sistema operativo](../resources/faq.md#cómo-recupero-mi-clave-desde-el-almacén-de-claves-del-sistema-operativo).

{% hint style="danger" %} **Anytype no puede recuperar tu arca si has perdido el acceso a tu clave por completo.** {% endhint %}

## Preguntas más frecuentes

#### ¿Por qué no usar correo electrónico y contraseña?

Usar una clave es la forma más segura de crear una cuenta sin depender de una autoridad central que controle tu acceso. La clave se genera enteramente en tu dispositivo, no se comparte con nadie y puede crearse incluso sin conexión.

Los sistemas de correo electrónico y contraseña están expuestos de diversas formas. Por lo general, el acceso a la cuenta queda en manos de la empresa desarrolladora de la aplicación: esto es lo que le permite restablecer tu acceso. Una clave elimina esa dependencia: puedes recuperar el acceso a tus datos aunque pierdas el dispositivo, te lo roben o se dañe, ya que la propia clave es la llave maestra de tus datos.

#### ¿Podría alguien adivinar mi clave?

En la práctica, no. Las claves se generan mediante algoritmos matemáticos complejos, y el número de combinaciones posibles es tan vasto que adivinar una o encontrarla por fuerza bruta resulta prácticamente inviable:

* **Combinaciones posibles:** 5 444 517 870 735 015 415 413 993 718 908 291 383 296
* **Coste de descifrarla:** 38 029 518 006 846 883 000 000 000 USD

Hasta el atacante mejor financiado y más equipado encontraría esta tarea insuperable.

#### ¿Qué riesgo existe de que se creen dos arcas con la misma clave?

Prácticamente ninguno. 

Las probabilidades de que dos personas generen la misma frase mnemotécnica de 128 bits son, más o menos, de 1 entre 2^128^ (alrededor de 3,4 × 10^38^), una cifra inmensamente superior a la de granos de arena que hay en la Tierra. Ni siquiera generando miles de millones de claves por segundo durante 100 años nos acercaríamos a una coincidencia.

En resumen, no tienes que preocuparte de que tu clave se genere para otro usuario.

#### ¿Cómo se genera mi clave?

Las frases semilla de Anytype siguen el estándar BIP-39 (Bitcoin Improvement Proposal 39), un protocolo normalizado que garantiza la compatibilidad entre distintos monederos y aplicaciones. BIP-39 incluye una suma de verificación para detectar errores de transcripción, reduciendo así el riesgo de perder el acceso por un simple error tipográfico.

#### ¿Qué pasa si pierdo mi clave?

Tener una clave te proporciona soberanía digital y una protección sólida, con el inconveniente de que mantenerla a salvo es responsabilidad tuya y solo tuya. Anytype no puede ayudarte a recuperar la clave ni la cuenta si la clave se pierde o queda expuesta.

Por cómodo que resulte guardar la clave de forma digital, hacerlo conlleva una vulnerabilidad real. Esto es lo que puedes hacer:

* Anota tu clave en un soporte físico.
* Guárdala en un lugar seguro que solo tú conozcas.
* Evita los dispositivos conectados a Internet y el almacenamiento en la nube. Si necesitas guardarla de forma digital, usa como mínimo un gestor de contraseñas seguro.
