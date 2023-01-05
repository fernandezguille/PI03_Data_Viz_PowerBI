<h1 align=center> PROYECTO INDIVIDUAL 03 </h1>
<h2 align=center> Visualización de datos, en Datasets de telecomunicaciones e internet </h2>

<br>

¡Hola! Mi nombre es *Guillermo Fernández* y éste mi tercer proyecto individual, que forma parte de la formación práctica del bootcamp de Data Science de la academia Henry. 

<hr>

## Objetivo
Realizar un análisis completo que permita reconocer el comportamiento del sector de telecomunicaciones a nivel nacional (en Argentina), considerando principalmente el acceso a internet. Con el fin de monitorear la eficacia de los objetivos de la empresa, se le pide visualizar en un dashboard el siguiente KPI y establecer 3 KPIs adicionales producto de su análisis:
* Variación porcentual trimestral del servicio de internet, cada 100 hogares por provincia.

[Consigna completa del PI](https://github.com/soyHenry/PI03-Analytics)

### Contexto
La industria de las telecomunicaciones ha jugado un papel vital en nuestra sociedad, facilitando la información a escala internacional y permitiendo la comunicación continua incluso en medio de una pandemia mundial. La transferencia de datos y comunicación se realiza en su mayoría a través de internet, líneas telefónicas fijas, telefonía móvil, casi en cualquier lugar del mundo.


<p align="center"> <img alt="Telecomunicaciones" src="https://djpautomacao.com/wp-content/uploads/2020/09/5g-na-industria-1140x596.png" width=500px> </p>

### Tecnologías utilizadas
* [Python](https://docs.python.org/3/)
    * [Pandas](https://pandas.pydata.org/)
* [PowerBI](https://powerbi.microsoft.com/es-es/)

<hr>

## Plan de trabajo:
1. Extraer los datos desde la API _(plus)_
2. EDA (Exploratory data analysis)
3. ETL (Extraction, Transform, Load)
4. Unir datasets, y exportar CSV a PowerBI
5. Establecer KPIs
6. Realizar scripts de Python en PowerBI _(plus)_
7. Realizar el Dashboard
8. Redactar un reporte escrito _(plus)_

### Archivos del repositorio
- [**Conexiones_a_internet_en_Argentina.csv**:](./Conexiones_a_internet_en_Argentina.csv/) Archivo CSV producto de la fusión de los datasets.  
- [**Dashboard_conectividad_a_internet.pbix**:](./Dashboard_conectividad_a_internet.pbix/) Dashboard que muestra el análisis de la información.  
- [**EDA.ipynb**:](./EDA.ipynb) Notebook de jupyter donde se realiza toda la carga y transformación de datos, así como la justificación de los datos escogidos para la realización del dashboard.

## Extraer los datos desde la API _(plus)_
Mediante el uso de la API del sitio web https://datosabiertos.enacom.gob.ar/ se obtuvo un dataset que incluye toda la información disponible del sitio, para revisar cuáles se utilizarán.

## EDA <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width=40px height=40px/><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original-wordmark.svg" width=40px height=40px/><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width=40px height=40px/>   
Se exploraron los 18 datasets obtenidos anteriormente, para detectar features relevantes. Se seleccionaron aquellos que estaban segregados por provincia, por ser los que mayor información aportaban, y de los cuáles se podrían obtener KPIs significativos.

## ETL
Algunos de los datasets tenían tipos de datos incorrectos, caracteres dentro de campos numéricos, etc. Se revisaron los campos de los datasets y se aplicaron correcciones.

## Unir datasets, y exportar CSV a PowerBI
Con los datasets limpios, se realizó el merge, y se quitaron columnas totalizadoras. Luego, se exportó el DF a un CSV para su consumo en PowerBI, revisando que la configuración regional compute bien los decimales. También se modificó el año para que fuera de tipo Date.

## Establecer KPIs
+ Variación porcentual trimestral de los accesos al servicio de internet cada 100 hogares, por provincia.
+ Variación porcentual trimestral de la cantidad de usuarios de las tecnologías más frecuentes, por provincia.
+ Rangos de velocidad, por provincia, y variación del promedio nacional.
+ Ingresos versus accesos cada 100 hogares, por provincia.

## Realizar scripts de Python en PowerBI _(plus)_
Se utilizaron scripts para realizar la carga del CSV y para elaborar una columna Trimestre con tipo Date.

## Realizar el Dashboard
Se estrableció un Dashboard con un tema oscuro y visualizaciones para facilitar el entendimiento los KPIs.

## Redactar un reporte escrito _(plus)_
El reporte se puede encontrar en el archivo EDA.ipynb, que fue realizado explicando los pasos, estableciendo conclusiones y explicando cómo se llegó a ellas.
<hr>

## Conclusión
Éste fue un proyecto desafiante, ya que el énfasis estaba en analizar e interpretar los datos. Por supuesto que esta interpretación es totalmente subjetiva, y de ahí el valor agregado que pueda aportar el Data Analyst.

Les dejo mi contacto:  
<a href="https://www.linkedin.com/in/fernandezguillermo"><img alt="Linkedin" title="Connect with me" src="https://img.shields.io/badge/Linkedin-0077B5?style=flat&logo=linkedin&logoColor=white"></a>  

¡Muchas gracias por llegar hasta aquí!