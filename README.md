# 📊Reacción del Mercado a la Gestión de Capital

Análisis de Volumen ante Eventos de Recompra de Acciones

## 📌Descripción

Este proyecto analiza cómo reacciona el mercado ante eventos de recompra de acciones (Recompra_Acciones), enfocándose específicamente en el comportamiento del volumen negociado el día del anuncio.

Las recompras suelen interpretarse como una señal positiva por parte del management. Un aumento significativo del volumen puede confirmar que el mercado está reaccionando activamente a esta decisión de asignación de capital.

## 📍Objetivo del Análisis

Medir si los eventos de recompra generan un spike de volumen anormal, comparando el volumen del día del evento contra el promedio de los 5 días hábiles previos.

## 🧠Insight clave

¿Qué recompras de acciones generaron un volumen significativamente superior al promedio reciente, indicando una fuerte reacción del mercado?

## ⚙️Metodología

- Selección de eventos
Se filtran únicamente eventos corporativos del tipo Recompra_Acciones.

- Cálculo del volumen base
Se calcula el volumen promedio de los 5 días anteriores al evento para cada ticker.

- Comparación relativa

Se calcula un ratio de volumen:

Volumen del día del evento / Volumen promedio de los 5 días previos


## 🧩Ordenamiento

Los resultados se ordenan de mayor a menor ratio para destacar las reacciones más extremas.

Estructura de Datos Utilizada:
- eventos_corporativos
- ticker_id
- fecha
- tipo_evento
- valor (monto de la recompra)
- precios_diarios
- ticker_id
- fecha
- volume

## ☑️Resultado Esperado

El output identifica:
- Tickers con recompras que activaron fuertemente el volumen

Casos donde el mercado:
- Validó la recompra como señal positiva
- Ignoró el evento (ratio cercano a 1)
- Mostró posible trading institucional (ratios muy elevados)

## 💼Valor de Negocio

- Detecta señales tempranas de interés institucional
- Ayuda a validar la efectividad comunicacional de una recompra
- Puede utilizarse como filtro para:
- Estrategias event-driven
- Análisis de eficiencia de mercado
- Señales de confirmación de tendencia

## 🚀Posibles Extensiones

- Analizar el impacto en precio post-evento
- Comparar volumen vs tamaño de la recompra (valor)
- Medir persistencia del volumen en días posteriores
- Segmentar resultados por sector o mercado de cotización

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.
