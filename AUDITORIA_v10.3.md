# SolarPro 10.3 · Auditoría de cuestionarios y diseño adaptable

## Método
Chromium en modo headless mediante Playwright; HTML cargado en un DOM aislado con `page.set_content`, scripts locales inyectados y CSS local. Los recursos de red se bloquearon. Esto **no equivale** a abrir el ZIP como sitio publicado.

## Evidencia reproducida
- Resoluciones 390 × 850, 768 × 850 y 1366 × 850 píxeles.
- Clasificador: seleccionar «Fósil» en la primera tarjeta produce retroalimentación correcta, habilita «Siguiente tarjeta», avanza de tarjeta 1 a 2 y «Reiniciar actividad» regresa a la tarjeta 1.
- Reflexión: elegir una respuesta habilita «Siguiente pregunta»; «Reiniciar preguntas» regresa a pregunta 1 de 5.
- Sin excepciones de JavaScript en las interacciones examinadas.
- Sin desbordamiento horizontal del documento principal en esas tres resoluciones (`document.documentElement.scrollWidth - innerWidth = 0`).

## Limitaciones
- No se completaron los 18 reactivos ni las 5 preguntas, por lo que no se ha validado el resumen final de cada actividad.
- No se verificaron todas las vistas en todos los tamaños, ni navegación mediante teclado/lector de pantalla.
- No se cambió el código funcional al no reproducirse fallos en esta etapa; se documentó la prueba.
