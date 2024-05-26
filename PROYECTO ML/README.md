[![SVG Banners](https://svg-banners.vercel.app/api?type=luminance&text1=RealEstate-Valencia2024%20🌻&width=800&height=400)](https://github.com/Akshay090/svg-banners)

Debido al gran auge de los pisos turisticos, se quiere comprobar si de verdad son mas rentables frente al alquiler tradicional, con la idea de invertir en el parque inmobiliario de la ciudad de Valencia y sacar la mayor rentabilidad posible a la inversion.


### **Bases de Datos consultadas y utilizadas ( */data* ):**

- Instituto Nacional de Estadística (INE):
    - IPV

- Colegio General del Notariado
    - Nº Transacciones Inmobiliarias

- Agencia Estatal de Administración Tributaria (Ministerio de Hacienda)
    - Renta Bruta Media por persona

- Banco de España
    - IPC
    - Euribor

- Ayuntamiento de Valencia
    - Mapa Distritos Valencia
    - Areas por distrito
    - Recibos IBIs

- Cátedra Observatorio de la Vivienda (UPV)
    - Consulta de analisis 

- Observatorio de Vivienda y Suelo (Ministerio de vivienda y suelo)
    - Consulta de analisis

- Web Scrapping en Idealista
    - Datos €/m2 de venta de inmuebles por distrito

- Web Scrapping en Fotocasa
    - Datos €/m2 de venta de inmuebles por distrito

### **Limpieza de datos y desarrollo del análisis ( */notebooks* ):**

Se decide partir el trabajo en una coleccion de notebooks para que sea mas facil acceder y tratar los datos:

   - 01_Datos_España: notebook donde se realiza la limpieza y el analisis de los parametros mas globales a nivel nacional

   - 02_Datos_Valencia: notebook donde se realiza la limpieza y el analisis de los parametros enfocados en Valencia y sus distritos.

   - 03_Mapas: notebook donde se trabajan, recopilan y extraes los mapas estadisticos relacionados con el EDA.

   - 

### **Consideraciones en el tratamiento de datos:**

- **Datos INE**: para el 100% de datos extraidos del INE se ha tenido que realizar una transofrmacion en los datos de fechas. No coincidiendo de partida, ni la temporalidad ni el formato en el dataset de origen.

- **Datos Idealista**: debido a la complicidad de realizar webscrapping en la web, se han procesado todos los datos a través de ChatGPT 4, facilitando la URL a scrappear y obtenien de salido un archivo CSV con toda la información.

- **Datos Ayuntamiento de Valencia VS Hacienda**: para poder cruzar datos entre ambas bases de ha tenido que normalizar el dato de distrito para que sean coincidentes, nombrandolo de forma distintiva en cada repositorio.

### **Representación de gráficos ( */graficos* ):**

Una vez ya todos los datos limpios se han realizado graficos y mapas exportandose a jpg y html respectivamente para su posterior inclusion en el ppt resumen del EDA.
