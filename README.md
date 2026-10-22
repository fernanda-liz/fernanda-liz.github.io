# fernanda-liz.github.io

Sitio personal de Fernanda Liz Cabezas G. — Magíster en Ciencias del Diseño, UAI.

**→ https://fernanda-liz.github.io/**

Acá se publica lo que va quedando utilizable: plantillas reutilizables, artefactos de
investigación y materiales de trabajo. Todo abierto y documentado.

## Qué hay

| Ruta | Qué es |
|---|---|
| `/` | Portafolio de una página, bilingüe (EN/ES): perfil, experiencia, formación, investigación y trabajo publicado |
| `/materiales/` | Índice de todo lo publicado (plantillas y presentaciones) |
| `/plantillas/presentaciones/` | Plantilla de presentaciones: 33 layouts, exportable a PDF |
| `/presentaciones/prototipado-mediana-resolucion-resina/` | Entrega final del Taller de Prototipos: prototipo de mediana resolución sensorial en resina con lapislázuli (9 diapositivas) |

## Estructura

```
.
├── index.html              ← portafolio (un solo archivo; textos EN/ES en el mismo HTML)
├── assets/img/             ← imágenes del portafolio
├── materiales/             ← índice de lo publicado
└── plantillas/
    └── presentaciones/     ← una carpeta autocontenida por cosa publicada
        ├── index.html
        ├── INSTRUCCIONES.md
        └── …
```

Cada cosa publicada vive en su propia carpeta y es autocontenida: se puede abrir directo por su
URL sin depender del portafolio. Para agregar algo nuevo, se crea su carpeta y se suma una tarjeta
en `materiales/index.html`.

El portafolio se configura en el objeto `CONFIG` al final de `index.html`: `linkedin` (enlace al
perfil, muestra el botón) y `photos` (fotografías de la sección analógica; si está vacío, la
sección no aparece). Cada texto va en dos idiomas con `<span class="en">` y `<span class="es">`.

## Ver localmente

```bash
python3 -m http.server 4200
# abrir http://localhost:4200/
```

Para trabajar sobre la plantilla de presentaciones conviene su propio servidor, que no cachea:

```bash
cd plantillas/presentaciones && python3 servidor.py
# abrir http://localhost:4180/
```

## Marca

Los colores son los mismos en todo el sitio (lapislázuli): navy `#0a0e1c`, dorado `#d9b25a`,
azul `#6478c2`. Viven en `:root` de cada archivo.

## Licencias

El código propio es de uso libre. La plantilla de presentaciones incluye componentes de terceros
bajo licencia MIT — ver
[`plantillas/presentaciones/LICENSE-signal-template`](./plantillas/presentaciones/LICENSE-signal-template)
y la sección de créditos de su README.
