# SolarPro 10.2 · Pruebas de interacción (Chromium aislado)

## Procedimiento
Se utilizó Chromium del sistema con Playwright. Por las restricciones de navegación `file://`, el HTML y los scripts locales se cargaron mediante `page.set_content`, conservando el DOM y los manejadores de eventos. Esto **no equivale** a una prueba integral de la aplicación extraída del ZIP.

## Comprobaciones observadas
- Generación: botones de acercar, alejar y restablecer modificaron el `viewBox` de 1100×690 a 825×517.5 y lo restauraron. El buscador con texto inexistente devolvió cero registros.
- Transmisión: acercar cambió el `viewBox` de 1100×690 a 858×538.2; alejar y restablecer devolvieron la vista inicial. La casilla de red interna aceptó cambios.
- Distribución: la selección de divisiones 14, 15 y 16 activó `url(#spMarkerGlow)` en la flecha de ampliación. Seleccionar la división 1 lo desactivó. El comparador conservó dos barras y respondió al cambio de indicador.
- Recorrido: al seleccionar la tercera etapa se mostró el simulador. Cambiar tensión primaria a 15 000 V actualizó su salida; restablecer devolvió 13 200 V.
- No se observaron excepciones JavaScript durante estas interacciones.

## Alcance y pendientes
- No se probó cada uno de los 57 botones, todos los cuestionarios ni la visualización a diferentes tamaños de pantalla.
- No se verificó conectividad externa de SEMARNAT, SENER o WRI.
- No se modificaron cifras ni datos oficiales. El código funcional se mantiene respecto de 10.1: esta entrega añade evidencia de auditoría, no afirma corregir errores que no se reprodujeron.
