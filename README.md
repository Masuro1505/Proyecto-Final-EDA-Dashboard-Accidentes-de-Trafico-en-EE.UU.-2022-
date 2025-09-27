# Proyecto-Final-EDA-Dashboard-Accidentes-de-Trafico-en-EE.UU.-2022-
Análisis de accidentes de tráfico en EE. UU. durante 2022. Se realiza un EDA con agrupaciones geográficas, temporales, por género y raza, y se presentan insights clave. Incluye un dashboard en Excel con KPIs y gráficas para visualizar los hallazgos

## Archivos del proyecto
- Carpeta **Data**:
	- Datasets originales
	- Dataframes finales
	- Datasets antes del merge

- Carpeta **Notebooks-EDA**

- Excel con el Dashboard

## Pasos seguidos durante el proyecto
1. **Carga y limpieza de datos:**  
   - Se cargaron los dos datasets originales, se eliminaron duplicados, se transformaron columnas y se agregaron columnas nuevas como `Severity_Label` y `Weather_Condition_Grouped`.

2. **Análisis exploratorio (EDA):**  
   - Agrupaciones por estado, condado, mes, día, día de la semana, hora, género y raza.  
   - Visualización de los datos mediante gráficos de barras y líneas temporales. 
   - Extracción de insights descriptivos y observaciones clave.

3. **Exportación de datasets y preparación para Excel:**  
   - Todos los dataframes intermedios exportados a CSV.  
   - Dataset grande cargado en el modelo de datos de Excel para evitar limitaciones de filas.

4. **Generación de KPIs:**  
   - Accidente totales.  
   - Top 3 estados con más accidentes.  
   - Top 3 condados con más accidentes.  
   - Distribución de accidentes por mes, día del mes, día de la semana y hora.  
   - Accidentes por severidad.

5. **Creación del dashboard en Excel:**  
   - Integración de todos los KPIs y gráficas en un dashboard visual mediante el uso de tablas dinámicas. 

## Conclusiones
Este proyecto me ha sido muy útil para terminar de entender bien el uso apropiado de los datos, además de su manejo y utilidad. Sin duda el EDA fue lo que más tiempo me llevó, pues entendí que era la base para entender y analizar mejor el volumen tan extenso de datos con los que elegí trabajar. A la hora de elegir sobre que datos iba a realizar este proyecto, tenía claro que algo relacionado con la geografía era lo que más me interesaba. A partir de ahí decidí buscar datos relacionados con Estados Unidos pues sabía que información no me iba a faltar, y así fue como me topé con un dataset gigante (de unas 7 millones de filas) acerca de los accidentes de tráfico en Estados Unidos desde el 2016 hasta el 2023. Yo decidí estudiar solo los del año 2022, pues tenía que acotar filas; como segundo dateset escogí uno de carácter demográfico para aportar información extra a mis análisis. Tras limpiar y organizar los datasets originales, los junté a través de un merge y empecé a trabajar con ellos. En los notebooks que adjunto viene un informe detallado de cada uno de los pasos que iba tomando a modo de comentario en markdown. Tras terminar el EDA me dispuse a crear el Dashboard, y plasmar todos los resultados relevantes que había conseguido. Tras esto solo quedó hacer muchas comprobaciones y checkeos para asegurarme de que estaba todo listo para entregarse. En cuanto a las conclusiones más destacables que he sacado del análisis cabe destacar un patrón normal en la cantidad de accidentes en aquellos condados/estados donde la densidad de población es mayor, y para mí sorpresa, si bien es cierto que el día de la semana que más accidentes hay son los viernes, accidentes considerados muy graves suceden más los jueves. Insight y conclusiones como estas hay muchas más en los notebooks. Por último me gustaría mencionar que estoy muy contento con el resultado de mi trabajo.
