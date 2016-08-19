# AcuseReciboDte
SDK Factronica
Librería para Integración de Acuse Recibo DTE.

Para realizar la integración con su software propio se deben realizar 3 procesos.

<h3>Procesos:</h3>
1.-Generar Archivo Plano con Formato Acuse Recibo Dte.<br>
2.-Enviar Archivo Plano hacia Servidor de Facturación.<br>
3.-Recuperar Resultados desde Servidor de Facturación.<br>

<h3>Proceso 1: Generar Archivo Plano</h3>
Consiste en generar un archivo de texto plano con el formato requerido.

Url con Formato Acuse Recibo Dte:
<br>https://github.com/FacTronica/AcuseReciboDte/blob/master/FormatoAcuseRecibo.php

<h3>Proceso 2: Enviar Archivo Plano</h3>
El archivo de texto plano se debe enviar al servidor de facturación.
<br>Para realizar este proceso se hace uso de librería opensource CURL.

<br>Enviar archivo desde Consola Windows:
<br>c:\curl\curl.exe --form "archivito=@c:\curl\archivo_plano.txt" http://www.factronica.cl/sdk/index.php

Enviar archivo desde Consola Linux:
<br>curl --form "archivito=@archivo_plano.txt" http://www.factronica.cl/sdk/index.php

<h3>Proceso 3: Recuperar Resultados:</h3>
Consiste en obtener los archivos con resultados.
