# Fuentes de Información

## Examen de reposición- Sección práctica

#### Mayo, 2020

### 1. Hadoop

Conéctese a nuestro servidor de Hadoop (148.205.....).  En la carpeta `/home/jincera/MaterialExReposición` encontrará los archivos `OwidDataCovidModif.csv`, `OwidData155.csv` y `EncabezadosOwidCovid.txt`. Son archivos que tienen un subconjunto de la data colectada por el sitio [ourworldindata](http://ourworldindata.org) sobre la pandemia Covid-19.



1. Cree una nueva carpeta en su directorio local llamada **Reposicion**.
2. **Cambie los permisos para que sólo usted pueda accederla** (`chmod 700 Reposicion`)
3. Ingrese a esa carpeta y **copie**  (comando `cp`) los tres archivos en la carpeta que acaba de crear.



El archivo `EncabezadosOwidCovid.txt` muestra el significado de cada columna de los otros dos archivos.  Revíselo (`cat EncabezadosOwidCovid.txt`).



En esta sección trabajaremos con el archivo `OwidDataCovidModif.csv`.

Con código que utilice **el paradigma MapReduce** y que se ejecute **en HDFS** (no puede limitar su respuesta a la ejecución con pipes de Unix), responda a las siguientes preguntas:

*  ¿Cuántos países contiene esta base de datos? *Su código debe responder con un número específico. No puede utilizar comandos como `wc`.*
* ¿Cuántos registros tiene cada país? *Genere un archivo de salida con el resultado de esta pregunta*.  Muestre los tres últimos países (`tail -3 <su archivo de resultados>`).

**Envíe sus resultados a jincera@itam.mx y deje su código en la carpeta `Reposición`. El profesor lo revisará posteriormente**.



### 2. Pig

*¡¡Cuidado con los separadores de los campos!!*

En esta sección trabajará con el archivo `OwidData155.csv`. Contiene únicamente datos de países para los que se han capturado 155 días de registros.

Mediante comandos de PigLatin, responda las siguientes preguntas:  

* ¿Cuántos fallecimientos, cuántos fallecimientos por millón, cuántos nuevos casos por millón y cuántas pruebas por millar tiene cada país?
* ¿Cuáles son los 10 países con la mayor tasa de fallecimientos por país?
* ¿Cuáles son los 10 países con la menor tasa de pruebsa por millar?



*Los resultados no van a ser consistentes con los datos oficiales porque la base de datos no está depurada*.

**Envíe sus resultados y las líneas de su script a jincera@itam.mx**



### 3. Fiware

En nuestro Orion Context Broker  en la nube (**IP: 18.222.167.78**) se han registrado instancias de entidades que simulan personas que utilizan pulseras con  monitoreo de temperatura corporal. Las pulseras envían periódicamente la lectura de tempreatura y las coordenadas geográficas donde se encuentra la persona.  Su tipo es `HealthMonitor`. 

1. Identifique qué atributos tienen estas entidades
2. Identifique todas las entidades que tienen una temperatura mayor a 37 grados.  Presente sus resultados como tuplas key-value
3. Identifique si hay entidades con una temperatura mayor o igual a 38 grados en un radio de  100 metros alrededor de las coordenadas del ITAM Sta. Teresa, que son: `longitud: 19.311802 latitutd:-99.223071` 



**POR FAVOR NO MODIFIQUE LOS ATRIBUTOS PARA NO AFECTAR A SUS COMPAÑEROS**



**Envíe el resultado obtenido y el URL con que hizo la consulta en cada caso a jincera@itam.mx**.  No es necesario que envíe capturas de pantalla.

