# SolarPro — Dictamen de revisión, etapa 6 (versión 6.5)

## Alcance revisado
- 6.1: conceptos de transmisión, ecuaciones y autoevaluación.
- 6.2: explorador esquemático de SIN, Baja California, Baja California Sur y Mulegé. **No es cartografía georreferenciada de infraestructura**.
- 6.3: simulador trifásico equilibrado con potencia activa recibida, tensión entre líneas, factor de potencia, longitud y resistencia por km.
- 6.4: indicadores históricos de CFE Transmisión 2022–2024 y discrepancia de 1 km en 2023.
- 6.5: revisión integral, pruebas automáticas y trazabilidad visible.

## Validación física
El modelo usa I=P/(√3·V·fp), R=r·L, P_J=3·I²·R, P_envío=P_recibida+P_J y η=P_recibida/P_envío. Unidades: P [MW], V [kV], I [A], R [Ω/fase], L [km], r [Ω/km], pérdidas [MW]. Se omiten reactancia, capacitancia, regulación de tensión y variación del factor de potencia. No es una simulación completa de líneas eléctricas.

## Datos y reservas
Las cifras 2022–2024 se presentan como transcripción de los informes anuales CFE proporcionados por el usuario, no como verificación externa independiente. Hay discrepancia 2023: 110,559 km (informe 2023) frente a 110,558 km (comparativo 2024). No se incorporaron coordenadas, líneas ni subestaciones ficticias.

## Cierre
Cierre técnico provisional sujeto a prueba en el navegador del usuario y aprobación explícita. No iniciar etapa 7 sin autorización.


## Iteración 6.9
Se corrigió la interacción del mapa utilizando controles HTML independientes del SVG. Nombres completos y ficha inmediatamente debajo del mapa. Indicadores de CFE nacionales, sin atribución por sistema. La prueba de clics en navegador sigue pendiente debido a restricciones del entorno de pruebas; cierre funcional condicionado a la comprobación del usuario.


## Iteración 7.0
Mapa SVG con marcadores en viewBox, esquema topológico de conectividad internacional y sistemas aislados. Revisión funcional del usuario pendiente.

## Versión 7.1: trazos dentro del mapa
Se incorporaron trazos esquemáticos al SVG geográfico. Representan conectividad topológica y NO rutas georreferenciadas. Se probaron los cuatro estados de selección en Chromium mediante contenido en memoria, incluyendo un clic directo sobre el marcador SVG. Los sistemas separados no presentan líneas ficticias. Queda pendiente validación de la entrega en el navegador del usuario.


## Actualización 7.2
Mapa de referencia 2024 con proyecto Baja California–Sonora NO operativo, filtros, panel lateral, leyenda y enlaces topológicos superpuestos. No se presenta ninguna línea como geometría física real. Los datos de capacidad instalada y generación principal por sistema quedan sin cifras hasta verificar fuentes desglosadas. Probado en Chromium en memoria; falta validación del usuario en archivo local.
