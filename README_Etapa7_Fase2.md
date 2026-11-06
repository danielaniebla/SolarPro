# SolarPro 8.3 · Etapa 7, fase 2

Se conserva la aplicación SolarPro 8.2 y se añade un simulador **didáctico monofásico de carga resistiva**, sin alterar el módulo de transmisión.

## Modelo
V2,ideal = V1/a; I2 = V2,ideal/(R_carga+R_serie); V_carga=I2 R_carga; P_util=I2² R_carga; P_cobre=I2² R_serie; P_perdidas=P_cobre+P_nucleo; eta=P_util/(P_util+P_perdidas).

Las resistencias están referidas al secundario. La pérdida de núcleo se supone constante; la potencia de entrada se aproxima como potencia útil más pérdidas. No se modelan reactancias, saturación ni factores de potencia distintos de 1. Parámetros ilustrativos, NO cifras de CFE.

## Verificación
Con parámetros iniciales 13,200 V, a=110, R_carga=12 Ω, R_serie=0.5 Ω y pérdida fija de 30 W: V2 ideal=120 V; I2=9.6 A; V_carga=115.2 V; P_util=1105.92 W; pérdidas=76.08 W; eficiencia=93.56 %. Comprobado con Chromium. Cambio de carga a 24 Ω y reinicio también probados. Cinco nodos del módulo previo y sincronización del panel conservados. Se corrigió un conflicto de identificadores con un simulador anterior de transmisión, usando el prefijo distSim.

## Limitaciones
El mapa de distribución permanece contextual, sin polígonos oficiales de divisiones ni ubicaciones inventadas. El simulador no pretende describir instalaciones reales.

## Uso
Descomprimir, abrir index.html y entrar en 3 · Distribución. Funciona sin conexión a internet.
