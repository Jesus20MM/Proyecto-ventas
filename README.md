# Predicción de Ventas con Series de Tiempo usando Facebook Prophet

## Descripción
En este proyecto guiado, el objetivo es predecir las ventas de varias tiendas a partir de una base de datos compuesta por dos tablas relacionadas: una contiene el historial de ventas y la otra, información adicional sobre las tiendas. Para ello, se emplea el análisis de series de tiempo, con el fin de capturar patrones temporales y generar predicciones en función del tiempo.

Como herramienta principal se utiliza Facebook Prophet, un modelo aditivo diseñado específicamente para trabajar con series temporales. Además del análisis exploratorio de datos y la extracción de información relevante, se realiza ingeniería de características para descomponer la variable temporal en componentes como año, mes y día, lo cual permite un análisis más detallado y una mejor modelación del comportamiento de las ventas a lo largo del tiempo.

## Dataset
Se utilizaron dos tablas relacionadas:
- **Tabla de ventas**: contiene el historial de ventas por tienda y por fecha.
- **Tabla de información de tiendas**: incluye datos adicionales relevantes para cada tienda (por ejemplo, ubicación, tipo de tienda, etc.).


## Metodología
1. **Análisis exploratorio de datos (EDA)**  
   Se exploran las variables temporales y se visualizan las ventas a lo largo del tiempo para detectar tendencias o estacionalidades.  


2. **Limpieza y transformación de datos**  
   Se asegura la consistencia en las fechas, se manejan valores nulos y se normalizan los datos si es necesario.

3. **Ingeniería de características**  
   Se descompone la variable fecha en componentes como:
   - Año
   - Mes
   - Día
   - Día de la semana  
   Esto ayuda a detectar patrones específicos.

4. **Modelado con Facebook Prophet**  
   Se usa Prophet para capturar tendencias y estacionalidades en los datos y generar predicciones a futuro por tienda.  
  

5. **Evaluación del modelo**  
   Se evalúa el ajuste del modelo visualmente y se pueden aplicar métricas de error (como MAE o RMSE) si se desea profundizar.

## Resultados
Se logró predecir el comportamiento de ventas para un número selecto de tiendas, capturando adecuadamente patrones temporales como tendencias generales y estacionalidad. Las predicciones permiten anticipar el comportamiento futuro de ventas y apoyar la toma de decisiones comerciales.



## Lecciones aprendidas
- Cómo trabajar con datos temporales y extraer sus componentes clave.
- Uso práctico de Facebook Prophet para generar predicciones.
- Importancia de descomponer variables temporales para mejorar el modelo.
- Valor del análisis exploratorio para entender la estructura y dinámica de los datos.

## Tecnologías
- Facebook Prophet  
- Pandas  
- Series de tiempo

## Mejoras futuras
- Aplicar Prophet con ajustes por tienda individual para capturar mejor sus particularidades.
- Incorporar variables externas (promociones, clima, etc.) para enriquecer el modelo.
- Comparar el rendimiento con otros modelos de series temporales como ARIMA o modelos basados en machine learning.
- Automatizar el pipeline de predicción para futuras actualizaciones del dataset.
