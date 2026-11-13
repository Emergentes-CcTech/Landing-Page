# IoBuild — Landing Page

Sitio público de IoBuild: plataforma IoT para la administración de condominios. Mide el agua y la energía de las áreas comunes, detecta fugas y calcula la cuota de mantenimiento de cada unidad según su participación (Ley N.° 27157).

La aplicación está en [iobuild.me](https://iobuild.me).

## Páginas

| Archivo | Contenido |
|---|---|
| `index.html` | Propuesta de valor, cómo funciona, beneficios, funcionalidades y planes |
| `about-us.html` | Misión, valores y equipo |
| `faq.html` | Preguntas frecuentes por categoría |

## Planes publicados

| Plan | Departamentos | Precio mensual | Kit en comodato | Activación (primer y último mes) |
|---|---|---|---|---|
| Esencial | hasta 40 | S/ 350 + IGV | 3 equipos | S/ 826.00 |
| Urbano | 41 a 80 | S/ 420 + IGV | 5 equipos | S/ 991.20 |
| Gran Torre | más de 80 | S/ 650 + IGV | 7 equipos | S/ 1,534.00 |

Contrato de 24 meses, instalación incluida y equipo adicional a S/ 30 + IGV al mes. Si cambian los precios en la plataforma, hay que actualizar `index.html`, `faq.html` y `assets/translations.json`.

## Idiomas

El sitio está en español por defecto, con inglés disponible en el selector. Los textos de cada página están en `assets/translations.json`, agrupados por página (`index`, `about`, `faq`) y en `common` para el encabezado y el pie. Cada clave corresponde a un atributo `data-translate` del HTML.

## Ejecutarlo localmente

Las traducciones se cargan con `fetch`, así que hay que servir la carpeta en lugar de abrir el archivo directamente:

```bash
python -m http.server 5500
```

Luego abre <http://localhost:5500>.

## Estructura

```
assets/
  img/             logo, favicon, imagen de misión y fotos del equipo (recortadas en cuadrado)
  translations.json
scripts/script.js  idioma, menú móvil, preguntas frecuentes y desplazamiento suave
styles/            reset.css y styles.css
```
