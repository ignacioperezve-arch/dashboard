# 📡 Dashboard IoT - Estación Meteorológica UV

Este archivo (`index.html`) implementa un **dashboard en tiempo real** para una estación meteorológica IoT, desarrollado en el contexto del proyecto **Framework IoT · Colectores Activos de Agua de Rocío** de la Universidad de Valparaíso.

## 🚀 ¿Qué hace?

- 🔌 Se conecta mediante **MQTT WebSocket** a un broker público (`161.35.98.146:9001`) autenticado.
- 📡 Se suscribe a múltiples tópicos con variables climáticas:
  - Temperatura (exterior/interior)
  - Humedad (exterior/interior)
  - Velocidad y dirección del viento
  - Presión atmosférica y tendencia
  - Lluvia, índice UV, energía solar, etc.
- 🖥️ Muestra los datos en una interfaz tipo panel dividida en **dos secciones**:
  - **Zona Beysens**: enfocada en el modelo de condensación de rocío (incluye cálculo del punto de rocío).
  - **Estación completa**: vista integral de todas las variables ambientales.
- ✨ Actualiza visualmente cada tarjeta al recibir un nuevo dato (efecto *flash*), con barras de progreso, gráficos (rosa de los vientos animada) e indicadores de estado de conexión.
- 📊 Provee información de última actualización, contador de mensajes recibidos y *badges* técnicos (QoS, RETAIN).

## 📌 Resumen

**Monitoreo en vivo de variables meteorológicas vía MQTT, con foco en investigación de rocío y visualización científica.**
