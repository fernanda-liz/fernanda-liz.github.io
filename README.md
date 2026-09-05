# fernanda-liz.github.io

Sitio personal de Fernanda Liz Cabezas G. — Magíster en Ciencias del Diseño, UAI.

**→ https://fernanda-liz.github.io/**

Acá se publica lo que va quedando utilizable: plantillas reutilizables, artefactos de
investigación y materiales de trabajo. Todo abierto y documentado.

## Qué hay

| Ruta | Qué es |
|---|---|
| `/` | Landing: índice de todo lo publicado |
| `/plantillas/presentaciones/` | Plantilla de presentaciones: 33 layouts, exportable a PDF |

## Estructura

```
.
├── index.html              ← landing
└── plantillas/
    └── presentaciones/     ← una carpeta autocontenida por cosa publicada
        ├── index.html
        ├── INSTRUCCIONES.md
        └── …
```

Cada cosa publicada vive en su propia carpeta y es autocontenida: se puede abrir directo por su
URL sin depender de la landing. Para agregar algo nuevo, se crea su carpeta y se suma una tarjeta
en `index.html`.

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
