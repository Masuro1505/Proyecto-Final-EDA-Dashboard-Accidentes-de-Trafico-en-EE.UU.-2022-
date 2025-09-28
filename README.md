# Proyecto-Final-EDA-Dashboard-Accidentes-de-Trafico-en-EE.UU.-2022-
Análisis de accidentes de tráfico en EE. UU. durante 2022. Se realiza un EDA con agrupaciones geográficas, temporales, por género y raza, y se presentan insights clave. Incluye un dashboard en Excel con KPIs y gráficas para visualizar los hallazgos

## Archivos del proyecto
**Nota importante:** Los archivos requeridos en el repositorio superan el límite de 100 MB permitido por GitHub. Por este motivo, he creado tres archivos `.txt` con el enlace correspondiente a cada carpeta en Google Drive.  

- **Archivo.txt → `Data_Link.txt`**  
  - **Datasets originales**  
    - US_Accidents_March23 → [Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents/data)  
    - demographic_data → [Kaggle](https://www.kaggle.com/datasets/ahmedmohamed2003/county-level-demographic-population-race-gender) 
  - **Dataset final**  
    - Accidentes_US_2022 (datasets final)  

- **Archivo.txt → `Notebooks-EDA_Link.txt`**  
  - reducción.ipynb  
  - clean_merge.ipynb  
  - EDA.ipynb  

- **Archivo.txt → `Dashboard_Link.txt`**  
  - Dashboard.xlsx

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
  
## Insights principales

- **Estados con más accidentes:** California, Florida y Texas, siguiendo la lógica de su población total y densidad. Texas, aunque más poblado que Florida, tiene menos accidentes debido a su menor densidad    de población.

- **Estados con menos accidentes:** Predominan aquellos con baja densidad poblacional y áreas rurales extensas.

- **Condados con más accidentes:** Los Angeles County (CA), Miami-Dade County (FL) y Orange County (FL), que coinciden con áreas urbanas densas y con mucho tráfico.

- **Condados con más accidentes por 100.000 habitantes:** Loving County (TX), Mineral County (MT) y Gilliam County (OR), reflejando tasas relativas en áreas menos pobladas.

- **Condiciones meteorológicas:** Los accidentes no dependen mayormente de la meteorología; los factores principales son otros, como la densidad de población y el tráfico.

- **Meses con más accidentes:** Abril y diciembre, probablemente por vacaciones, festividades (*Spring Break*, Pascua, Navidad) y cambios climáticos estacionales. Pico secundario en agosto por vacaciones de   verano.

- **Accidentes muy graves:** Diciembre es crítico; julio muestra un pico inesperado. Tulare County (CA) destaca por alta gravedad, posiblemente por el tipo de carreteras y presencia de vehículos pesados.

- **Día del mes:** Días 1 y 15 concentran más accidentes, reflejando movimientos de vacaciones y viajes al inicio de la primera y segunda quincena. Los últimos días del mes son más seguros.

- **Día de la semana:** Viernes con más accidentes generales; jueves con más accidentes fatales, posiblemente por fatiga acumulada. Domingos son los días más seguros.

- **Horas del día:** Picos de accidentes a las 7-8 AM y 3-5 PM coinciden con horarios de trabajo; accidentes fatales son mayores en la tarde (15-17 h), asociándose a cansancio acumulado tras jornada laboral.

- **Por género:** Miami-Dade, Davidson y Orange County encabezan accidentes por cada 100.000 hombres y mujeres; los top 20 son consistentes entre ambos géneros.

- **Por raza:** 
  - Blancos: Miami-Dade (FL), Orange (TX), Prince George’s (MD)
  - Negros: Miami-Dade (FL), San Diego (CA), San Bernardino (CA)
  - Latinos: Wake (NC), Mecklenburg (NC), Pinellas (FL) 

## Conclusiones
Este proyecto me ha sido muy útil para terminar de entender bien el uso apropiado de los datos, además de su manejo y utilidad. Sin duda el EDA fue lo que más tiempo me llevó, pues entendí que era la base para entender y analizar mejor el volumen tan extenso de datos con los que elegí trabajar.

A la hora de elegir sobre que datos iba a realizar este proyecto, tenía claro que algo relacionado con la geografía era lo que más me interesaba. A partir de ahí decidí buscar datos relacionados con Estados Unidos pues sabía que información no me iba a faltar, y así fue como me topé con un dataset gigante (de unas 7 millones de filas) acerca de los accidentes de tráfico en Estados Unidos desde el 2016 hasta el 2023. Yo decidí estudiar solo los del año 2022, pues tenía que acotar filas; como segundo dateset escogí uno de carácter demográfico para aportar información extra a mis análisis.

Tras limpiar y organizar los datasets originales, los junté a través de un merge y empecé a trabajar con ellos. En los notebooks que adjunto viene un informe detallado de cada uno de los pasos que iba tomando a modo de comentario en markdown. Tras terminar el EDA me dispuse a crear el Dashboard, y plasmar todos los resultados relevantes que había conseguido. Tras esto solo quedó hacer muchas comprobaciones y checkeos para asegurarme de que estaba todo listo para entregarse. Por último me gustaría mencionar que estoy muy contento con el esfuerzo realizado y el resultado de mi trabajo.
