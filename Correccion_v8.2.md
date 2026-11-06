# SolarPro 8.2 — Corrección de encabezado del explorador

## Problema observado
Al seleccionar un nodo, la ficha cambiaba correctamente pero el encabezado permanecía en «Selecciona una etapa».

## Corrección
El encabezado `#distDetailTitle` se actualiza en la misma función `select(i)` que actualiza la ficha, los enlaces del mapa, el progreso y los controles. Se elimina el encabezado duplicado dentro de la ficha.

## Pruebas
Chromium: clic en cinco nodos SVG, botones de etapas, siguiente, anterior y reiniciar; todas las cabeceras coinciden con la etapa elegida; cero errores JavaScript. `node --check script.js` correcto.

## Alcance
No se cambian las estadísticas, las fuentes, la cartografía ni los demás módulos. Abrir `index.html` después de descomprimir el ZIP completo.
