# TUQO · Portafolio para clientes

Sitio estático (HTML + CSS + JS, sin build) para presentar TUQO a clientes. Es el mismo diseño que el portafolio de admisiones (`ulrich-md/Portfolio`), pero con textos de venta: servicios, proceso, proyectos en vivo y contacto.

## Secciones

| Sección | Qué muestra |
|---|---|
| **Portada** (fólder) | Qué hace TUQO, cliente destacado, cotización gratis y polaroids que abren cada sitio |
| **Proyectos** (pizarra) | Testimonios de Ángeles Mastretta, Grupo Balseca y Nexos, cifras y los 6 sitios en vivo + Ally |
| **Proceso** (call sheet) | Cómo trabajamos, en 5 pasos, y cómo usamos la IA |
| **Servicios** (corcho) | Sitios web, agentes de IA, automatizaciones y software a la medida; por qué TUQO y botón para cotizar |
| **Taller** (escritorio de noche) | Los proyectos como objetos que se pueden mover |
| **Caso** (expediente) | Mastretta & Nexos |
| **Contacto** | Preguntas frecuentes, carta, WhatsApp (238 150 1095) y correo |

## Idiomas

- El texto en español está en `index.html`. El inglés está en `i18n.js`, con las mismas claves (`data-i18n`).
- Al entrar, el sitio elige el idioma en este orden:
  1. `?lang=es` o `?lang=en` en el link.
  2. La última elección del visitante con el botón ES / EN.
  3. Su zona horaria: México, Latinoamérica o España cargan español.
  4. El idioma de su navegador: si es inglés, carga inglés.
  5. Si nada de lo anterior aplica, español.
- Para mandarle a alguien el sitio en un idioma fijo, agrega `?lang=en` o `?lang=es` al final del link.

## Verlo en local

```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

## Deploy en Vercel

1. En vercel.com → **Add New → Project** → importa este repositorio.
2. Framework preset: **Other**. Sin build command; output directory: la raíz (`.`).
3. Deploy. Cada push a `main` vuelve a publicar el sitio.

## Créditos de imágenes

- Fólder manila (portada): [Manila folder](https://commons.wikimedia.org/wiki/File:Manila_folder.jpg) — allispossible.org.uk, **CC BY 2.0** (requiere crédito: ya está en el pie de página). Fondo recortado y color ajustado.
- Texturas (kraft, corcho, madera, papel): [ambientCG](https://ambientcg.com), CC0.
- Pizarra, taza, terrario, teclado, clip y recorte de periódico: stocksnap.io y rawpixel.com, CC0.
- Capturas de `assets/proof/`: proyectos de TUQO. En las de Ally está difuminado el nombre de un tercero.
