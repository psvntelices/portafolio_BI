# Portafolio de Power BI

Sitio estático (HTML + CSS, sin dependencias) pensado para publicarse gratis en GitHub Pages.

## Estructura

```
index.html            Página principal: presentación, tarjetas de proyectos, habilidades, contacto
proyectos/ventas.html Plantilla de página de detalle (cópiala por cada dashboard)
assets/style.css      Estilos (colores en :root, arriba del archivo)
assets/img/           Capturas y GIFs de tus dashboards
```

## Cómo agregar un dashboard

1. Copia `proyectos/ventas.html` con otro nombre, por ejemplo `proyectos/inventario.html`.
2. Guarda la captura o el GIF en `assets/img/` y cambia la ruta de la imagen.
3. Rellena problema, proceso, medida DAX e impacto.
4. En `index.html`, copia un bloque `<a class="card">` y apúntalo a la nueva página.

Busca `EDITA:` en los archivos para encontrar lo que falta personalizar.

## Antes de publicar un dashboard: anonimizar

- Trabaja sobre una **copia** del .pbix, nunca el original.
- Reemplaza nombres de clientes, empleados y proveedores por nombres genéricos (Cliente 001, Región Norte).
- Multiplica los montos por un factor fijo (por ejemplo 0,73) para conservar las proporciones sin mostrar cifras reales.
- Revisa títulos, tooltips, filtros y logos: ahí suelen quedar nombres reales.
- Nunca uses "Publicar en la web" con datos reales: el enlace es público.
- Si tienes dudas sobre tu contrato de confidencialidad, muestra solo capturas con datos ficticios.

Para GIFs de la interacción sirven ScreenToGif (Windows) o la grabación de pantalla de tu sistema; mantenlos cortos y livianos (menos de 5 MB).

## Publicar en GitHub Pages

El sitio se publica desde la rama `main`, carpeta raíz (Settings → Pages → Source: "Deploy from a branch").
Cada cambio que subas a `main` se publica solo en uno o dos minutos en:

https://psvntelices.github.io/portafolio_BI/
