# Registro ARCO

App para celular para registrar emociones con el método ARCO (Antecedentes, Respuesta, Consecuencias), basada en el Registro ARCO 2.0 de Ps. Nicolás Cabib Olave. Funciona en iPhone, Android y computador, se instala en la pantalla de inicio y funciona sin internet.

Los registros se guardan **solo en el teléfono** donde se usa la app. No se envían a ningún servidor.

## Publicar en GitHub Pages

1. Crea un repositorio público llamado `USUARIO.github.io` (o cualquier nombre).
2. Sube todos los archivos de esta carpeta, incluida la carpeta `icons`.
3. En el repositorio, ve a **Settings → Pages**.
4. En "Build and deployment", elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
5. En uno o dos minutos la app queda publicada. La versión oficial está en https://registro-arco.github.io/

## Instalar en el teléfono

- **iPhone:** abre el link en Safari, toca Compartir y luego "Agregar a inicio".
- **Android:** abre el link en Chrome y toca "Instalar" (o menú ⋮ → "Instalar app").

## Enviar registros al psicólogo

En **Ajustes → Enviar tus registros a tu psicólogo** se genera un PDF con los registros del período elegido, listo para compartir por WhatsApp o correo.

Guía para pacientes: [`guia-registro-arco.pdf`](guia-registro-arco.pdf).

## Respaldos

En **Ajustes → Respaldo** se descarga un archivo con todos los registros. Guárdalo en Drive, iCloud o tu correo. Para pasar los registros a otro teléfono, usa **Ajustes → Importar respaldo**.

## Actualizar la app

Al cambiar `index.html`, sube también `sw.js` con un número nuevo en `VERSION` (por ejemplo `arco-v2`), para que los teléfonos descarguen la versión nueva.

## Archivos

- `index.html`: la app completa.
- `manifest.webmanifest`: nombre, colores e íconos para instalarla.
- `sw.js`: guarda la app para que funcione sin internet.
- `icons/`: íconos de la app.
- `vendor/jspdf.umd.min.js`: librería jsPDF 2.5.2 (licencia MIT) para generar los PDF sin internet.
- `guia-registro-arco.pdf`: guía de una página para pacientes, con código QR.
