# Auriculares: fichas técnicas de 302 modelos

Especificaciones de los auriculares que se venden en España, recopiladas y revisadas por
[Ondo](https://ondogear.com), el buscador de auriculares. Formato, conexión, códecs, batería, peso, impedancia y
compatibilidad con PC, móvil, PS5, Xbox y Switch, en CSV y JSON.

*English summary below.*

## Qué hay

| Archivo | Contenido |
|---|---|
| [`data/auriculares.csv`](data/auriculares.csv) | Una fila por modelo. Las listas van separadas por `\|` |
| [`data/auriculares.json`](data/auriculares.json) | Los mismos datos, con listas y valores `null` |
| [`VERSION`](VERSION) | Fecha de la última exportación y número de modelos |

302 modelos de 60 marcas: 176 de diadema, 74 true wireless, 32 intraurales de cable, 12 de oído libre y 8 supraaurales.

## Cómo se recogen

- La fuente principal es la web oficial de cada marca (columna `official_url`).
- Un dato que la marca no publica o que no se puede confirmar queda vacío. No se estima ni se rellena.
- `platforms` solo incluye lo que la marca confirma. Que unos auriculares de cable funcionen en el mando de una
  consola no basta para que aparezca la consola.
- `battery_hours` es la mejor cifra que da la marca; si da dos, la que es sin cancelación de ruido.
- Solo modelos a la venta en España en 2026. Un modelo con varios colores es una sola fila.

Los detalles están en la [metodología de Ondo](https://ondogear.com/metodologia/). Si ves un error, abre una
*issue* con el enlace a la fuente.

## Columnas

| Columna | Valores |
|---|---|
| `id` | Identificador único, marca-modelo en minúsculas |
| `brand`, `model` | Marca y modelo |
| `form` | `over-ear` (diadema), `on-ear` (supraaurales), `earbuds` (true wireless), `in-ear` (intraurales de cable), `open-ear` (oído libre o conducción ósea) |
| `back` | `closed`, `open`, `semi-open`; vacío en intraurales y true wireless |
| `connection` | `bluetooth`, `dongle` (adaptador de 2,4 GHz), `wired` |
| `plugs` | Conectores de cable con audio: `3.5mm`, `6.35mm`, `usb-c`, `usb-a`, `lightning` |
| `platforms` | Confirmadas por la marca: `pc`, `mobile`, `ps5`, `xbox`, `switch` |
| `uses` | `gaming`, `music`, `studio`, `casual` |
| `anc` | Cancelación activa de ruido (`true` / `false`) |
| `mic` | `boom-detachable`, `boom-fixed`, `built-in`, `inline`, `none` |
| `multipoint` | Conexión Bluetooth a dos dispositivos a la vez; vacío si no tienen Bluetooth |
| `battery_hours` | Horas según la marca |
| `weight_g` | Gramos, según la marca |
| `driver`, `driver_type` | Descripción del transductor y tipo: `dynamic`, `planar`, `ba`, `hybrid` |
| `impedance_ohm` | Impedancia nominal en ohmios |
| `codecs` | Códecs Bluetooth: `SBC`, `AAC`, `LDAC`, `aptX`, `aptX Adaptive`, `LC3`… |
| `surround` | Sonido envolvente o espacial (`true` / `false`) |
| `water` | Protección IP (`IPX4`, `IP54`…) |
| `release_year` | Año de lanzamiento |
| `official_url` | Página del producto en la web de la marca |
| `ondo_url` | Ficha del modelo en Ondo |

No incluye precios: cambian cada día y dependen de la tienda. Para ver el precio orientativo de cada modelo, abre
su `ondo_url`.

## Licencia y cómo citarlo

[CC BY 4.0](LICENSE): puedes usar, copiar y modificar los datos, también con fines comerciales, siempre que cites la
fuente con un enlace. Por ejemplo:

> Datos: [Ondo](https://ondogear.com), CC BY 4.0.

---

## English summary

Specifications of 302 headphone models sold in Spain (form factor, connection, Bluetooth codecs, battery, weight,
impedance, manufacturer-confirmed compatibility with PC, mobile, PS5, Xbox and Switch), collected from manufacturer
websites by [Ondo](https://ondogear.com). Unknown values are left empty, never estimated. Column names are in
English; text values such as `driver` are in Spanish. Licensed under [CC BY 4.0](LICENSE): attribute as
“Data: Ondo (ondogear.com), CC BY 4.0” with a link.
