# Auditoría del Módulo 3 · SolarPro 9.2 → 9.3

## Redundancias detectadas
- Catálogo de 16 divisiones (`divList`) y panel de detalle.
- Directorio de 16 divisiones (`sigDirectory`) y segundo panel de detalle.
- Explorador adicional de tarjetas (`cfeFigureEmbed`) que repetía las mismas divisiones.
- Dos representaciones de México: una para el recorrido didáctico y otra para el explorador.

## Corrección de la iteración 1
- Eliminados catálogo y visor de tarjetas duplicados.
- Un único selector regional junto al mapa y un solo panel de indicadores.
- Se conserva el recorrido funcional, sus cinco etapas y el simulador.
- Comparación independiente de dos divisiones mediante cuatro indicadores verificados de 2023.
- Eliminadas elipses que podían confundirse con polígonos territoriales: sustituidas por marcadores numerados explícitamente NO geográficos.

## Pendiente para la iteración 2
- Sustituir marcadores por geometrías territorialmente verificadas a partir de cartografía oficial, antes de afirmar que el mapa muestra delimitaciones de CFE.
- Revisión visual de la figura III.1 y de la procedencia de los polígonos.
- Evaluación UX en móvil y navegación por teclado.

## Integridad de datos
- Se preservan los datos de CFE cierre 2023 y el rótulo «Sin dato público regional» para longitud BT y MT+BT.
- Los símbolos del mapa no determinan la división correspondiente a un domicilio.
