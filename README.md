# Proyecto: Análisis del Sentimiento en Criptomonedas y su Relación con el Tipo de Cambio

# Descripción general
Este trabajo busca evaluar la relación entre el sentimiento en el mercado de criptomonedas, medido a través del Fear & Greed Index (FGI) aplicado especialmente al Bitcoin, y el tipo de cambio de monedas emergentes, en particular el sol peruano.

El análisis incluye además variables de control relevantes como el DXY (Índice del dólar estadounidense), el VIX (Índice de volatilidad del mercado) y el BTC (Precio histórico del Bitcoin).

# Fuentes de datos

- Fear & Greed Index (FGI): datos obtenidos desde la API de Alternative.me
- Tipo de cambio USD/PEN: series oficiales del Banco Central de Reserva del Perú (BCRP).
- DXY, VIX y BTC: información histórica descargada a través de yfinance desde Yahoo Finance.

Fecha de última actualización de los datos: Se consideraron observaciones hasta el 30 de junio de 2025, que corresponde al último registro disponible en la base de datos de Alternative.me.

# Variables principales

FGI: Índice de "Miedo y Codicia" aplicado al Bitcoin, indicador de sentimiento en el mercado cripto. Está especialmente enfocado en el Bitcoin y combina diferentes indicadores (volatilidad, volumen, momentum, encuestas, etc.) para identificar si el mercado se encuentra en un estado de miedo (pesimismo, ventas masivas) o de codicia (optimismo, compras especulativas).

USD_PEN_Venta: Representa el tipo de cambio nominal de venta del dólar estadounidense en el mercado peruano. Refleja el valor en soles peruanos que los agentes económicos deben pagar por adquirir un dólar. Esta variable es clave para analizar la estabilidad cambiaria del país y el impacto de factores externos sobre la economía local.

# Variables de Control

BTC_USD: Precio diario de Bitcoin en dólares estadounidenses. El Bitcoin es el principal activo del mercado de criptomonedas y su precio refleja tanto movimientos especulativos como cambios en la confianza de los inversionistas.

DXY: Índice que mide el valor del dólar frente a una cesta de monedas extranjeras (principalmente euro, yen japonés, libra esterlina, dólar canadiense, corona sueca y franco suizo). Es un indicador de la fortaleza del dólar en los mercados internacionales.

VIX: Índice de volatilidad del mercado de opciones del S&P500. Valores altos del VIX suelen asociarse a periodos de incertidumbre o crisis financieras globales.

# Ejecución del Notebook

El notebook se organiza en las siguientes secciones:

1. Obtención de datos

- Fear & Greed Index
- Tipo de cambio PEN/USD (BCRP)
- DXY, VIX y BTC

2. Unificación de datos
   
- Consolidación de todas las fuentes en un único DataFrame para facilitar el análisis.

3. Análisis exploratorio
   
- Estadísticas descriptivas, visualización de tendencias y correlaciones.

4. Conclusiones
   
- Discusión sobre los hallazgos y su relevancia en el contexto del mercado cambiario.

# Resultados esperados

- Identificación de correlaciones entre el sentimiento en criptomonedas y el comportamiento del tipo de cambio.

- Evaluación comparativa de la volatilidad entre activos tradicionales (USD/PEN, DXY, VIX) y el mercado cripto (Bitcoin).

