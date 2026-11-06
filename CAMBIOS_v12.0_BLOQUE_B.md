# SolarPro 12.0 — Bloque B y cabeceras

- Factor de potencia predeterminado del simulador trifásico: 1.00 (antes 0.95).
- Comparación de pérdidas: incluye y destaca la tensión seleccionada, además de 115, 230 y 400 kV.
- Distribución: selector de transformador monofásico ideal o modelo resistivo con pérdidas; conserva el simulador anterior.
- Modelo ideal: tensión primaria, relación de espiras y potencia aparente; muestra tensión secundaria, corriente primaria, secundaria y conservación de potencia aparente.
- Se distinguen los supuestos del modelo ideal y el modelo con pérdidas.
- Cabeceras de los módulos 0–3 con marco, gradiente y jerarquía visual consistente con «¿Sabías que?».
- No se cambiaron indicadores CFE, mapas, fuentes ni la identidad SolarPro.

## Pruebas numéricas independientes
- Transmisión P=100 MW, V=230 kV, fp=1, R=5 ohm por fase: I=251.021 A; pérdidas=0.94518 MW (aprox).
- Transformador ideal Vp=13200 V, Np/Ns=110, S=10 kVA: Vs=120 V; Ip=0.757576 A; Is=83.333333 A.

## Límites
No es un modelo de flujo de potencia de red ni un transformador trifásico real. Las pruebas de navegador y accesibilidad requieren revisión adicional.
