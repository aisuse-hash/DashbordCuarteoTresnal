# Dashboard Cuarteo — versión para GitHub Pages

Este paquete contiene:

- `index.html`: dashboard principal.
- `HISTORICO_CUARTEO_COMPLETO.json`: histórico que se carga automáticamente al abrir la web.
- `.nojekyll`: evita procesamiento innecesario de GitHub Pages.

## Publicarlo en GitHub Pages

1. Crear un repositorio nuevo en GitHub, por ejemplo `dashboard-cuarteo`.
2. Subir estos tres archivos a la raíz del repositorio.
3. En GitHub abrir **Settings → Pages**.
4. En **Build and deployment**, elegir **Deploy from a branch**.
5. Seleccionar la rama `main` y la carpeta `/ (root)`.
6. Guardar.
7. GitHub mostrará la dirección pública del dashboard.

## Importante

La primera vez que una persona abre el sitio, el dashboard carga automáticamente
`HISTORICO_CUARTEO_COMPLETO.json` y lo guarda en el almacenamiento local de ese navegador.

Los cambios que un visitante haga dentro del dashboard quedan solamente en su navegador:
no modifican el archivo publicado ni cambian los datos de otros usuarios.

Para actualizar el histórico público en el futuro, reemplazá el JSON y cambiá el valor
`PUBLIC_DATA_VERSION` dentro de `index.html`.
