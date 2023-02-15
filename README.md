# Que es ViperMonkey

ViperMonkey es una herramienta desarrollada en python y su función principal es analizar macros VBA.

## Como funciona ViperMonkey

ViperMonkey extrae la macro del documento y lo muestra por pantalla. 

![Macro](/images/macro_payload.png)

Después hay un apartado que muestra el payload encodeado en base64

![Base64](/images/base64_payload.png)

Otra cosa interesant que mostrará es una tabla con los IOC

![IOC1](/images/IOC_table.png)

![IOC2](/images/IOC_table2.png)

Y por último mostrará funciones que ejecuta que pueden ser también indicadores de compromiso

![PossibleIOC](/images/possible_IOC.png)

Sample utilizado: https://app.any.run/tasks/e472f974-4c58-428f-9159-016453f367d3/

https://www.virustotal.com/gui/file/e26b12859ce5d6654399ec144ba5196fa97bc04cf36d6ed3881501a9478b0338

## Setup

### Descargar repositorio

`git clone [Enlace del repositorio]`

### Construir la imagen

Dentro de la carpeta del repositorio poner:

`docker build -t vmonkey .`

### Crear y ejecutar un contenedor

`docker run --name [nombre] -it [nombre de la imagen]`

### Entrar al contenedor

`docker exec -it [nombre del contenedor] /bin/bash`

### Apagar el contenedor 

`docker stop [nombre del contenedor]`

### Descomprimir samples

`unzip [archivo].zip`

### Ejecutar ViperMonkey

`vmonkey [archivo].doc`

#### Ejemplo 

`vmonkey 1word.doc`
