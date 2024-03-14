# Exploratory Data Analysis
## TOP 1000 canales de Twitch

El objetivo de este proyecto es realizar un EDA acerca de los datos de los primeros 1000 canales de Twitch según dentro de https://twitchtracker.com/. 

## Estructura del proyecto:
* Extracción de la información (Web Scraping)
* Limpieza de datos (Web Scrubbing)
* Planteamiento de hipótesis.
* Análisis y generación de gráficos.
* Conclusiones.

### Extracción de la información.
Los datos para el análisis del proyecto han sido extraídos a través de web scraping de la web citada anteriormente. Se han obtenido 2 dataframes, el primero extrayendo la información con Beautiful Soup del ranking general dentro de las primeras 20 páginas, complementándolo con la información que se encuentra en el perfil de cada canal dentro de la misma plataforma.

Disponiendo de esta información, se han podido extraer posteriormente los datos de los últimos 40 streams disponibles de cada uno de los canales, para lo cual ha sido necesario manejar tanto Beautiful Soup como Selenium.

Podemos encontrar todo el código utilizado en "streamers.ipynb", "Streamers2.ipynb", "Streamers3.ipynb" y "streams.py"

### Limpieza de datos (Web Scrubbing).
Dentro del segundo dataframe ha sido necesario realizar una limpieza ya que las fechas y valores numéricos habían sido extraidos como texto. Disponible en: "Limpieza de datos.ipynb".

### Planteamiento de hipótesis.
Una vez revisado que se disponía de toda la información prevista correctamente se han planteado 2 hipótesis:
* El idioma del contenido influye para tener más/menos éxito en la plataforma.
* El tipo de contenido influye en el progreso en la plataforma.

### Análisis y generación de gráficos.

Para poder extraer unas conclusiones, se han elaborado múltiples relaciones gráficamente de que simplificarán este proceso, entre las que podemos destacar los heatmaps por idioma o boxplots y violinplots relacionando el idioma con las diferentes variables numéricas. Todo el proceso está disponible en el fichero "EDA.ipynb".

### Conclusiones.

Finalmente se declara que no parece existir una influencia clara del tipo de contenido sobre los múltiples factores de las retransmisiones, por otro lado el idioma influye notablemente en las primeras 50-100 posiciones.

