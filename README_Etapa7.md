# SolarPro 8.1 · Corrección del gráfico de distribución

## Diagnóstico
La versión 8.0 solo mostraba un mapa territorial de fondo sin nodos ni flujo eléctrico en el gráfico principal. Los botones funcionaban, pero no había visualización interactiva del proceso en esa zona.

## Corrección
- El gráfico SVG ahora muestra cinco nodos eléctricos y cuatro enlaces funcionales encima del mapa contextual.
- Cada nodo es seleccionable con clic, Enter o Espacio y sincroniza el panel y los botones inferiores.
- Los enlaces cambian de azul a verde lima conforme avanza el recorrido.
- Reiniciar devuelve la selección a la primera etapa.
- Los nodos son conceptuales: NO se presentan como instalaciones reales ni georreferenciadas.
- No se alteró la etapa de transmisión ni se duplicaron sus controles de zoom.

## Auditoría de contenido
- Informe Anual CFE 2024: 49.1 millones de usuarios; 16 divisiones; 150 zonas; 901 mil km de Redes Generales de Distribución. Datos nacionales, sin desglose geográfico.
- Proceso subestación → alimentador → transformador → red secundaria → usuario: secuencia didáctica, no unifilar específico de CFE.
- Fórmulas de transformador ideal monofásico y diferencia entre kW y kWh: conceptos físicos; se distinguen de datos oficiales.
- Se evita asignar voltajes, rutas y capacidades individuales sin evidencia.

## Pruebas realizadas
- `node --check script.js`: correcto.
- Chromium: SVG visible; cinco nodos, cuatro enlaces (ocho elementos gráficos); clic en cada nodo y actualización correcta del panel; reinicio; cero errores JavaScript.
- Captura verificada: SolarPro_v8.1_grafico_verificado.png, fuera del ZIP.

## Uso
Descomprimir, abrir index.html, ir a 3 · Distribución. No requiere internet.
