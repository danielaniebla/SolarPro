# SolarPro 8.4 · Divisiones oficiales de CFE Distribución

## Investigación documental
CFE, Programa de Ampliación y Modernización de las Redes Generales de Distribución 2024–2038, sección III, figura III.1, página 7, identifica 16 divisiones y 150 zonas. El mapa del documento es una figura, no un GeoJSON/shapefile georreferenciado que pueda trasladarse con precisión a la aplicación. No se trazan límites falsos.

Fuente: https://beta.cfe.mx/distribucion/cumplimiento/Documents/PAM%20RGD%202024-2038%20VF.pdf

## Funciones
- Catálogo interactivo de las 16 divisiones con su nombre y orden oficial.
- Buscador, selección, panel de detalles y restablecimiento.
- Acceso a figura oficial de CFE (requiere internet); el catálogo opera sin conexión.
- Se conserva el mapa contextual, el recorrido de cinco nodos y el simulador monofásico.
- Se reparó un error previo de IDs: el HTML del simulador utilizaba `sim...` mientras el JavaScript esperaba `distSim...`; ahora los resultados y las barras se calculan.

## Pruebas
- Chromium: 16 divisiones, búsqueda de Valle de México (3 resultados), selección de divisiones 1/2/14/16, restablecimiento, clic en nodo eléctrico y actualización de simulador; cero errores de página.
- Node: `node --check script.js` correcto.
- ZIP: integridad comprobada.

## Límites
No hay polígonos regionales oficiales incorporados; los totales nacionales no se atribuyen a cada división. La cartografía original de CFE puede consultarse mediante enlace, no como una capa vectorial. El simulador usa valores didácticos, no mediciones de CFE.
