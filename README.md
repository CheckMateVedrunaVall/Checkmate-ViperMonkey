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

