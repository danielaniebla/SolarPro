# SolarPro Atlas 7.2 — Red de transmisión, referencia 2024

## Qué cambió
- Mapa geográfico SVG local con cuatro sistemas y trazos topológicos **sobre el propio mapa**.
- Barra superior de filtros: Ver todo, Sistema Interconectado Nacional, Sistema Interconectado Baja California, Sistema Interconectado Baja California Sur y Sistema Interconectado Mulegé.
- Panel lateral dinámico al hacer clic en nodos, líneas o filtros; al pasar el cursor sobre un nodo se muestra su ficha si el filtro está en Ver todo.
- Leyenda con controles de visibilidad: red interna conceptual, interconexión internacional, proyecto Baja California–Sonora y sistemas aislados.
- Proyecto Baja California–Sonora diferenciado en ámbar punteado; **no operativo en 2024**.
- Baja California conectada a red occidental estadounidense con línea azul discontinua.
- Mulegé y Baja California Sur aislados, sin enlaces dibujados.
- Sin carga de archivos ni dependencia de internet.

## Advertencias documentales
Los segmentos sobre el mapa son relaciones topológicas **esquemáticas**. NO constituyen trazados físicos de líneas ni geometrías georreferenciadas. Los trazos continuos del Sistema Interconectado Nacional representan su conectividad conceptual, no líneas de transmisión físicas activas individuales. La interconexión por Sonora está representada como proyecto, no conexión operativa en 2024. No se asignan capacidades instaladas ni generación principal por sistema sin datos cotejados; se indica no disponible/no verificada. Los indicadores nacionales de CFE 2024 no se desagregan por sistema.

## Verificaciones
- `node --check script.js`: aprobado.
- Prueba de Chromium (HTML/CSS/JS cargados en memoria): sin errores JavaScript.
- Cinco filtros: seleccionables, actualizan panel y resaltado de líneas.
- Seis trazos: 4 internos, 1 internacional y 1 de proyecto.
- Los dos sistemas aislados no resaltan enlaces.
- Leyenda: desactivación del proyecto verificada.
- Clic directo sobre nodo SVG de Baja California: verificado.
- Captura visual: SolarPro_v7.2_verificacion.png (archivo de prueba aparte).
- Prueba final en navegador local del usuario: pendiente.

## Fuentes de referencia
CFE Informe Anual 2024 para indicadores nacionales y PRODESEN 2023–2037 para estructura de sistemas; revisar el año específico de los anexos antes de atribuir capacidad o generación individual.

## Uso
Descomprime el ZIP completo, abre `index.html` y entra en «2 · Transmisión». El mapa funciona sin red ni archivos aportados por el usuario.


## Versión 7.3 — Controles unificados
Se corrigió la ausencia de la interfaz de filtros y panel lateral en el HTML de la entrega anterior. Se integra una sola barra de acercar, alejar y restablecer dentro del mapa; se retiran los controles inferiores duplicados. Se verificó en Chromium la interacción de los cinco filtros, los cuatro sistemas, las seis relaciones esquemáticas, la leyenda, el clic sobre nodos y las tres acciones de zoom.
