# SolarPro 8.7 — Opción C: preparación de mapa geográfico interactivo

La figura III.1 original sigue siendo un requisito pendiente: no se pudo descargar una copia oficial. Se añade visor de imagen local para que el usuario pueda incorporarla sin conexión, y soporte para una capa GeoJSON con polígonos verificables de las divisiones. No se incluyen polígonos estimados ni se asignan coordenadas ficticias. La aplicación valida estructura GeoJSON, nombres y rango de coordenadas, pero **no puede verificar automáticamente procedencia o exactitud**; es necesario cotejar con fuente oficial antes de publicar.

Para cargar polígonos: archivo GeoJSON FeatureCollection con propiedades `division`, `nombre` o `name`, y geometrías Polygon/MultiPolygon en coordenadas geográficas WGS84 (longitud, latitud). Para mostrar la figura original: cargar imagen PNG/JPG/WEBP extraída del PDF oficial. Los archivos se leen localmente en el navegador y no se envían a un servidor.

Fuente de nombres: CFE PAM RGD 2024–2038, figura III.1, p.7. Mapa base contextual preexistente en SolarPro.
