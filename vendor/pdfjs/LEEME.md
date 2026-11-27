# pdf.js 6.5.438 (Mozilla, Apache-2.0)

`pdf.min.mjs` y `pdf.worker.min.mjs` se descargaron de cdnjs el 21-11-2026 y son idénticos byte a byte a
`pdfjs-dist@6.5.438/build/` de npm (SHA-256 cotejado en ambos orígenes):

| Archivo | SHA-256 |
|---|---|
| pdf.min.mjs | 3a88402882cfa3e7e72c2c9b5149f52f0f88baf1c5b62aa11a41abdbc2072440 |
| pdf.worker.min.mjs | 1e64c8240e54735ec5913b37acd5134747799cb8c6bb3777c70adbc01232d2aa |

La página los importa desde su propia carpeta (`vendor/pdfjs/`), así que al abrir un PDF no corre ningún script de
terceros. Si la carpeta no está (la página servida sola), usa pdf.js 3.11.174 de cdnjs con SRI. Licencia en `LICENSE`.
Para actualizar: descargar la versión nueva de los dos orígenes, comparar los SHA-256, reemplazar los archivos y cambiar
`PDFJS_LOCAL` en `tools/web/web_template.html`.
