# Translating Virtual Printer

[English](#english) · [Español](#español)

---

## English

Thank you for helping! Virtual Printer uses standard **gettext `.po` files**: plain text files that free tools can edit. You don't need to know how to program.

| File | What it is |
|---|---|
| `locales/virtual_printer.pot` | Template with every text of the app, in English |
| `locales/es.po`, `locales/fr.po`… | One translation per language |

### Translate with Poedit (recommended)

1. Install [Poedit](https://poedit.net/) (free).
2. **New language:** download [`virtual_printer.pot`](locales/virtual_printer.pot), open it in Poedit, click **Create new translation** and pick your language. Save it as `xx.po` (`fr.po`, `pt_BR.po`, `de.po`…).
   **Existing language:** open its `.po` file (for example [`es.po`](locales/es.po)) to complete or fix it.
3. Translate the texts. Poedit shows the original, notes for translators and where each text is used.

### Rules that keep the app working

- **Keep `{name}`-style placeholders** exactly as they are (you can move them): `Sent to {printer}` → `Envoyé à {printer}`. Poedit warns if one is missing.
- **Keep HTML tags** such as `<b>…</b>` and `<br>`.
- **`&` in menus** marks the keyboard shortcut letter (`&File` → Alt+F). Put it before a letter that suits your language and that is not repeated in the same menu.
- Keep `…` at the end of actions that open a dialog.
- "Receipt" means a POS/till ticket (thermal printer), not a proof of payment.
- Some texts have **singular and plural** forms: fill in every form Poedit shows.

### Test your translation (no need to build anything)

1. Copy your `xx.po` to `%USERPROFILE%\.virtual_printer\locales\` (create the `locales` folder if needed).
2. Restart Virtual Printer and choose your language in **Options › Language**.

The file in that folder takes priority over the one included in the app, so you can keep editing and restarting. If a translation breaks a `{placeholder}`, the app shows the English text for that line and writes a warning to `virtual_printer.log`.

### Send it

- **GitHub:** open a pull request in this repository adding or updating `locales/xx.po`.
- **No GitHub account?** [Open an issue](https://github.com/castoragra/virtual-printer-web/issues) and attach the `.po` file.

Your name will be credited in the file header (`Last-Translator`) and in the release notes.

By sending a translation you agree that it may be included and distributed, free of charge, with Virtual Printer and its website.

---

## Español

¡Gracias por ayudar! Virtual Printer usa **archivos `.po` de gettext**, el estándar: archivos de texto que se editan con herramientas gratuitas. No hace falta saber programar.

| Archivo | Qué es |
|---|---|
| `locales/virtual_printer.pot` | Plantilla con todos los textos de la app, en inglés |
| `locales/es.po`, `locales/fr.po`… | Una traducción por idioma |

### Traducir con Poedit (recomendado)

1. Instala [Poedit](https://poedit.net/) (gratuito).
2. **Idioma nuevo:** descarga [`virtual_printer.pot`](locales/virtual_printer.pot), ábrelo en Poedit, pulsa **Crear nueva traducción** y elige el idioma. Guárdalo como `xx.po` (`fr.po`, `pt_BR.po`, `ca.po`…).
   **Idioma existente:** abre su `.po` (por ejemplo [`es.po`](locales/es.po)) para completarlo o corregirlo.
3. Traduce los textos. Poedit muestra el original, las notas para traductores y dónde se usa cada texto.

### Reglas para no romper la app

- **Conserva las variables tipo `{name}`** tal cual (puedes moverlas de sitio): `Sent to {printer}` → `Enviado a {printer}`. Poedit avisa si falta alguna.
- **Conserva las etiquetas HTML** como `<b>…</b>` y `<br>`.
- **El `&` de los menús** marca la letra del atajo de teclado (`&File` → Alt+A en `&Archivo`). Ponlo delante de una letra adecuada que no se repita en el mismo menú.
- Mantén `…` al final de las acciones que abren un diálogo.
- "Receipt" es el ticket de un TPV (impresora térmica), no un justificante de pago.
- Algunos textos tienen **singular y plural**: rellena todas las formas que muestre Poedit.

### Probar la traducción (sin compilar nada)

1. Copia tu `xx.po` en `%USERPROFILE%\.virtual_printer\locales\` (crea la carpeta `locales` si no existe).
2. Reinicia Virtual Printer y elige tu idioma en **Opciones › Idioma**.

El archivo de esa carpeta tiene prioridad sobre el incluido en la app, así que puedes seguir editando y reiniciando. Si una traducción rompe una `{variable}`, la app muestra ese texto en inglés y lo anota en `virtual_printer.log`.

### Enviarla

- **GitHub:** abre un *pull request* en este repositorio que añada o actualice `locales/xx.po`.
- **¿Sin cuenta de GitHub?** [Abre una incidencia](https://github.com/castoragra/virtual-printer-web/issues) y adjunta el `.po`.

Tu nombre aparecerá en la cabecera del archivo (`Last-Translator`) y en las notas de la versión.

Al enviar una traducción aceptas que se incluya y distribuya, de forma gratuita, con Virtual Printer y su sitio web.
