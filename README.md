# ConnectaTel-analysis

Este repositorio contiene el análisis realizado para la empresa de telecomunicaciones ConnectaTel, con operaciones en México y Colombia.

El objetivo del proyecto es analizar cómo los clientes usan los servicios móviles de mensajes y llamadas, identificando patrones de comportamiento, detectando valores atípicos y creando segmentos de clientes que ayuden a mejorar la oferta comercial y la experiencia del usuario.

## 📂 Contenido del repositorio

- `notebooks/connectatel_analysis.ipynb`  
  Notebook principal con carga de datos, limpieza, análisis exploratorio, visualizaciones, detección de outliers, segmentación de clientes e insights ejecutivos.

- `data/plans.csv`  
  Catálogo de planes disponibles, incluyendo precio, minutos incluidos, GB incluidos y costos por consumo extra.

- `data/users_latam.csv`  
  Información de los clientes, incluyendo edad, ciudad, fecha de registro, plan contratado y churn.

- `data/usage.csv`  
  Información de uso real de los servicios, incluyendo llamadas, mensajes, duración y longitud.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pUwwED8626N0dbtCO8Q_0ZvpsAF5WU6w#scrollTo=05e15812)

O también puedes abrirlo manualmente:

1. Abre el archivo `notebooks/connectatel_analysis.ipynb` en GitHub.
2. Copia el enlace del notebook.
3. Entra a Google Colab.
4. Selecciona **File → Open notebook → GitHub**.
5. Pega el enlace del repositorio o busca el nombre del repositorio.

## 📘 Cómo reproducir el análisis

1. Abre el notebook `notebooks/connectatel_analysis.ipynb`.
2. Ejecuta las celdas en orden.
3. El notebook carga los datasets desde la carpeta `data/` del repositorio.
4. Revisa los resultados, gráficos e insights generados.

## 🧠 Objetivo del análisis

El proyecto busca responder preguntas clave de negocio:

- ¿Qué segmentos de clientes muestran mayor o menor uso de llamadas y mensajes?
- ¿Qué usuarios presentan valores atípicos que puedan indicar comportamientos inusuales, fraude o errores de registro?
- ¿Cómo varía el uso según la edad y el tipo de plan contratado?
- ¿Qué patrones pueden ayudar a diseñar mejores planes, optimizar la oferta y mejorar la satisfacción del cliente?

## 🛠️ Herramientas utilizadas

- Python
- pandas
- NumPy
- matplotlib
- seaborn
- Jupyter Notebook
- Google Colab
- GitHub

## 🔎 Etapas del análisis

1. **Carga y exploración de datos**  
   Se cargaron los datasets `plans`, `users_latam` y `usage`, revisando sus primeras filas, estructura, tipos de datos y dimensiones.

2. **Identificación de problemas en la calidad de los datos**  
   Se revisaron valores nulos, valores inválidos, sentinels y fechas fuera de rango.

3. **Limpieza básica de datos**  
   Se corrigieron valores inválidos como edades imposibles, ciudades desconocidas y fechas futuras.

4. **Resumen estadístico por usuario**  
   Se agregaron las métricas de uso por cliente, calculando cantidad de mensajes, cantidad de llamadas y total de minutos de llamada.

5. **Visualización de distribuciones**  
   Se crearon histogramas para analizar la distribución de edad, mensajes, llamadas y minutos de llamada.

6. **Identificación de outliers**  
   Se utilizaron boxplots y el método IQR para detectar usuarios con comportamientos extremos de uso.

7. **Segmentación de clientes**  
   Se crearon segmentos por nivel de uso y por grupo de edad para entender mejor el comportamiento de los clientes.

8. **Insights ejecutivos**  
   Se generaron conclusiones y recomendaciones comerciales para ConnectaTel.

## 📊 Principales hallazgos

- La mayoría de usuarios pertenece al segmento de `Uso medio`.
- El grupo de edad más grande corresponde a usuarios `Adultos`.
- Existen usuarios con consumos altos en llamadas, mensajes y minutos, especialmente en la variable `cant_minutos_llamada`.
- Los outliers de uso no se eliminaron automáticamente, ya que pueden representar clientes intensivos o de alto valor.
- Se identificaron oportunidades para mejorar la oferta de planes según edad, nivel de uso y comportamiento de consumo.

## 💡 Recomendaciones de negocio

- Crear ofertas especiales para usuarios de alto consumo.
- Diseñar campañas de activación para usuarios de bajo uso.
- Revisar planes diferenciados para adultos mayores, con beneficios enfocados en llamadas.
- Analizar oportunidades para atraer usuarios jóvenes con planes más flexibles o beneficios digitales.
- Mantener los outliers de uso para análisis comercial, ya que pueden representar clientes valiosos.

## 📌 Conclusión

El análisis permitió construir una visión clara del comportamiento de los clientes de ConnectaTel. La base de usuarios está compuesta principalmente por clientes adultos y de uso medio, pero también existen segmentos de bajo y alto consumo que pueden ser aprovechados para mejorar la estrategia comercial, optimizar planes y fortalecer la retención de clientes.


