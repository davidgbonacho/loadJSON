
# 3 formas de cargar JSON
Carga un archivo JSON en HTML con JavaScript, de tres formas distintas: `XMLHttpRequest`, `fetch` (con promesas) y `async/await`.

`[SimPIL son una serie de ejemplos ultra-simples de cómo realizar diferentes operaciones con código. Sin complicaciones.]`

## Instalación
Simplemente clona el repositorio y ejecuta el código desde un servidor web (Apache, por ejemplo). La página debe servirse por `http(s)://`: los navegadores bloquean las peticiones a archivos locales abiertos con `file://`.

## Ejecución
Solicita el documento `loadJSON.html` y éste cargará `data.json` y mostrará el nombre y el apellido dentro de la página.

Las tres formas están incluidas en el mismo script. Sólo una está activa (`async/await`); las otras dos están comentadas. Para probar otra, comenta el bloque activo y descomenta el que quieras:

- **XMLHttpRequest**: la forma clásica de AJAX. El texto de la respuesta se convierte con `JSON.parse()`.
- **fetch**: la forma moderna con promesas, encadenando llamadas `.then()`. `response.json()` convierte el JSON.
- **async/await**: la misma petición `fetch`, escrita con `await` para que se lea como código secuencial (usa también template literals).

En las tres, un objeto se convierte en parámetros de query string con `URLSearchParams` y se envía con la petición (`data.json?SayMyName=true`). Un archivo JSON estático los ignora, pero así es como se enviarían parámetros a un servicio real (por ejemplo, un endpoint PHP).

## Archivos
- `loadJSON.html`: un documento HTML ultra-simple con las tres formas de cargar el JSON
- `data.json`: el archivo JSON que se carga
- `img/logo.svg`: sólo las imágenes importantes están aquí

> [!NOTE]
[Text in English here](README.MD)

![](img/logo.svg)
---
`título:` 3 formas de cargar JSON [`SimPIL`] 08/11/26\
`autor:` David G. Bonacho &nbsp;&nbsp;  [www.tizedit.com](https://www.tizedit.com)
