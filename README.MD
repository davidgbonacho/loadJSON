
# 3 ways to load JSON
Load a JSON file into HTML using JavaScript, in three different ways: `XMLHttpRequest`, `fetch` (with promises) and `async/await`.

`[SimPIL are a series of ultra-simple examples of how to perform different operations with code. Uncomplicated.]`

## Install
Simply clone the repo and run the code from a web server (Apache, for example). The page must be served over `http(s)://`: browsers block requests to local files opened with `file://`.

## Perform
Request the document `loadJSON.html` and it will load `data.json` and show the name and surname inside the page.

The three ways are included in the same script. Only one is active (`async/await`); the other two are commented out. To try another one, comment out the active block and uncomment the one you want:

- **XMLHttpRequest**: the classic AJAX way. The response text is parsed with `JSON.parse()`.
- **fetch**: the modern way with promises, chaining `.then()` calls. `response.json()` parses the JSON.
- **async/await**: the same `fetch` request, written with `await` so it reads like sequential code (uses template literals too).

In all three, an object is converted into query string parameters with `URLSearchParams` and sent with the request (`data.json?SayMyName=true`). A static JSON file ignores them, but this is how you would send parameters to a real service (e.g. a PHP endpoint).

## Files
- `loadJSON.html`: an ultra-simple HTML document with the three ways to load the JSON
- `data.json`: the JSON file to be loaded
- `img/logo.svg`: only important images are here

> [!NOTE]
[Texto en español aquí](README_ES.MD)

![](img/logo.svg)
---
`título:` 3 ways to load JSON [`SimPIL`] 11/08/26\
`autor:` David G. Bonacho &nbsp;&nbsp;  [www.tizedit.com](https://www.tizedit.com)
