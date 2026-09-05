---
description: Haz que los asistentes de IA trabajen con tus datos de Anytype.
---

# Técnica (skill) de Anytype para agentes

La **técnica de Anytype para agentes** es un kit de herramientas de código abierto que proporciona a los asistentes de IA una forma segura de leer, buscar y modificar objetos en tus canales de Anytype. Si la arrastras a Claude Code, Cursor, Gemini CLI, GitHub Copilot o cualquier otra herramienta agéntica, el agente podrá ejecutar scripts sobre tus datos de Anytype de forma sistematizada para gestionar modificaciones en lote, transformaciones y tareas repetitivas que preferirías no hacer a mano.

El repositorio está en GitHub: [github.com/anyproto/anytype-agents-skill](https://github.com/anyproto/anytype-agents-skill).

***

Anytype ya expone una [API local](local-api.md) que permite la integración directa. Esta técnica está una capa por encima: empaqueta la API en funciones prefabricadas para que el agente de IA pueda usarla sin que tengas que instruirle sobre el protocolo.

Si alguna vez has pensado «ojalá bastara con decir lo que quiero hacer con mis notas para que se hiciera», aquí tienes un instrumento. Describes el encargo en lenguaje corriente, el agente usa la técnica para traducirlo a las operaciones correctas de Anytype y el trabajo queda hecho.

Casos de uso habituales:

* **Actualización de propiedades en lote**: «Asigna a todas las tareas de la colección "Primer trimestre" el estado "En curso"».
* **Transformaciones de datos** — «Encuentra todas las notas etiquetadas como "reunión" del trimestre pasado y crea una colección que las resuma».
* **Migración y limpieza**: «Renombra los objetos que contengan "PENDIENTE" en el título para eliminar esa palabra».
* **Informes**: «Haz una lista de todos los objetos que he modificado este mes, agrupados por tipo».
* **Operaciones entre canales**: «Copia la definición de este tipo de mi canal personal a mi canal de equipo».

## Cómo funciona

La técnica ofrece un **entorno de ejecución de JavaScript ligero y aislado**. Cuando el agente decide hacer algo con tus datos de Anytype, escribe un breve script de JavaScript empleando los métodos de alto nivel de la técnica y, a continuación, lo ejecuta en el sandbox. El script usa tu API local de Anytype para leer y escribir.

Se exponen unos 30 métodos de alto nivel, que abarcan lo siguiente:

* **Lectura de objetos**: obtener el objeto por ID, enumerar objetos por tipo, buscar en canales.
* **Creación de objetos**: añadir un objeto nuevo con tipo, propiedades y contenido.
* **Modificación de objetos**: establecer valores de propiedades, cambiar el tipo, editar bloques de contenido.
* **Búsqueda**: buscar texto, filtrar por propiedad, limitar a un canal.
* **Operaciones con tipos y propiedades**: enumerar los tipos disponibles, crear tipos nuevos, gestionar propiedades.
* **Colecciones y consultas**: añadir y eliminar objetos en una colección, consultar con filtros.

El entorno de ejecución está **aislado**: el script solo tiene acceso a los métodos de la técnica de Anytype, no a tu sistema de archivos ni a la red. Esto significa que puedes ejecutar los scripts generados por IA sin miedo a que hagan algo destructivo fuera del propio Anytype.

(Por supuesto, dentro de Anytype, el script puede cambiar cualquier cosa que permita la API. (Consulta la sección **Seguridad** más abajo.)

## Configuración

#### Requisitos

* Anytype instalado y en ejecución en el mismo dispositivo;
* una [clave de API local](local-api.md) generada en **Ajustes del arca > Claves de API**;
* un agente de IA que admita el uso de herramientas (Claude Code, Cursor, Gemini CLI, GitHub Copilot, etc.).

#### Instalar la técnica

Los pasos de instalación dependen del agente que uses. En general:

1. Clona o descarga la técnica desde [github.com/anyproto/anytype-agents-skill](https://github.com/anyproto/anytype-agents-skill).
2. Configura tu agente para que cargue la técnica (cada agente tiene su propia forma de registrar herramientas, consulta su documentación).
3. Dale tu clave de la API de Anytype cuando te la solicite.

El repositorio de la técnica incluye guías de configuración para los agentes de las herramientas más habituales.

#### Comprobar que funciona

Pídele al agente algo sencillo, como:

> Enumera todos los tipos de objetos de mi canal personal.

Si la técnica se ha conectado, el agente ejecutará un método como `listTypes()` en tu API local y te informará. En caso contrario, verás un error o el agente recurrirá a responder generalidades.

## Ejemplos de encargos

#### Actualización en lote

> Cambia el estado de todas las tareas de la colección «Sprint 14» a «Hecho».

El agente escribe un breve script que hace lo siguiente:

1. busca la colección por su nombre,
2. enumera todos los objetos que contiene,
3. filtra los que son del tipo «Tarea»,
4. modifica la propiedad «Estado» de cada uno.

En muchos de los agentes, verás el script antes de que se ejecute y podrás aprobarlo o rechazarlo.

#### Búsqueda e informes

> ¿Cuántas notas he creado este mes y qué etiquetas usan?

El agente hace esto:

1. consulta los objetos del tipo «Nota»,
2. los filtra por fecha de creación,
3. recopila los valores de su propiedad «Etiqueta»,
4. presenta un informe.

No cambia ningún dato.

#### Transformación y migración

> Por cada objeto «Libro» de mi canal «Lectura», crea un objeto «Reseña» y vincúlalo al libro correspondiente.

El agente hace esto:

1. enumera los libros,
2. crea un objeto «Reseña» para cada libro con una relación que los une,
3. informa de lo que ha hecho.

## Seguridad

#### Qué puede hacer esta técnica

Tiene las mismas capacidades que la API local: crear, modificar y eliminar objetos; modificar tipos y propiedades, y cambiar el contenido de los bloques.

#### Qué no puede hacer esta técnica

* acceder a archivos de tu ordenador externos a Anytype;
* realizar solicitudes de red fuera de la API local;
* ver o modificar otros canales a los el agente no tenga acceso (más concretamente, el agente solo puede actuar en los canales a los que dé acceso la clave de API que le has proporcionado);
* saltarse los permisos del canal, es decir, si tu función en ese canal es la de visitante, la técnica solo podrá leer.

## Notas

{% hint style="warning" %}
**Revisa los scripts antes de ejecutarlos.** La mayoría de los agentes te muestran antes lo que van a ejecutar. Léelo. Es difícil recuperarse de un script «elimina todos los objetos que tengan X» ejecutado por error.
{% endhint %}

{% hint style="warning" %}
**Usa una clave de API aparte para las operaciones del agente.** Si un día quieres revocar el acceso del agente, puedes eliminar la clave en **Ajustes del arca > Claves de API** sin que esto afecte al resto de tus integraciones.
{% endhint %}

{% hint style="info" %}
**Pruébalo primero con algo sencillo.** Antes de ejecutar una operación en lote sobre cientos de objetos, pídele al agente que la ejecute con cinco de ellos y comprueba el resultado.
{% endhint %}

Tienes más información (en inglés) aquí: 

* [Técnica de Anytype para agentes en GitHub](https://github.com/anyproto/anytype-agents-skill): referencia completa de métodos, ejemplos y configuración por agente.
* [API local](local-api.md): interfaz subyacente y gestión de las claves. 
