<h2>
Configuración de Teléfono IP Huawei eSpace 7910 por medio de RPA (Robotic Process Automation) con TagUI</h2>
<div>
A partir de una herramienta de <b>RPA</b> (Automatización Robótica de Procesos) denominada <b>TagUI</b> (<a href="https://github.com/kelaberetiv/TagUI" target="_blank">https://github.com/kelaberetiv/TagUI</a>) se desarrolla un robot para la configuración automática de los teléfonos marca Huawei, modelo eSpace 7910.<br />
<h3>
Requisitos</h3>
Para la ejecución del robot, se necesita:<br />
<br />
<ul>
<li>Tener instalado <a href="https://github.com/kelaberetiv/TagUI#set-up" target="_blank">TagUI</a></li>
<li>Crear la carpeta <b>C:\telefonohuawei</b></li>
<li>Descargar los siguientes archivos:</li>
<ul>
<li><a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/telefonohuawei" target="_blank">telefonohuawei</a> - código fuente del robot</li>
<li><a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/extensiones.csv" target="_blank">extensiones.csv</a> - listado de extensiones a configurar</li>
<li><a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/srn2.jpg" target="_blank">srn2.jpg</a> - imagen a utilizar como papel tapiz del teléfono</li>
<li><a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/configurados.csv" target="_blank">configurados.csv</a> - listado generado por el robot con los teléfonos y extensiones configuradas</li>
</ul>
</ul>
<h3>
Ejecución</h3>
Desde la consola de comados (cmd) ubicarse dentro de la carpeta y lanzar el siguiente comando:<br />
C:\telefonohuawei&gt;&nbsp;<b>tagui telefonohuawei chrome</b><br />
<h3>
Funcionalidades</h3>
<div>
Una vez iniciado el robot ejecutará las siguientes tareas:</div>
<div>
<ul>
<li>Iniciar una ventana del navegador Chrome</li>
<li>Preguntar el ultimo octeto de la ip del teléfono a configurar. El robot tiene precargados los primeros 3 octetos de la ip 172.24.30.</li>
<li>Preguntar la extensión a configurar. El robot consultará del listado&nbsp;<a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/extensiones.csv" target="_blank">extensiones.csv</a>&nbsp;los otros datos para la configuración.</li>
<li>Iniciar sesión en el teléfono con el usuario admin y la contraseña que viene por defecto</li>
<li>Cambiar el idioma a Español</li>
<li>Cargar la imagen&nbsp;<a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/srn2.jpg" target="_blank">srn2.jpg</a>&nbsp;y configurarla como papel tapiz</li>
<li>Cambiar la contraseña por defecto a *12345678</li>
<li>Configurar la cuenta de la extensión en el teléfono</li>
<li>Desactivar DND</li>
<li>Configurar buzón de voz</li>
<li>Leer los datos de mac y serial del teléfono</li>
<li>Configurar fecha y hora con la zona horaria (Bogota, Lima, Quito)</li>
<li>Crear un nuevo registro en el listado&nbsp;<a href="https://github.com/alfarodaniel/RPA-TagUI-Telefono-IP-Huawei/blob/master/configurados.csv" target="_blank">configurados.csv</a>&nbsp;con los datos de la mac, serial, extensión y oficina del teléfono configurado</li>
</ul>
</div>
En el siguiente video se puede ver la ejecución del robot:<br />
<iframe allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" frameborder="0" height="315" src="https://www.youtube.com/embed/CK-lVlkq5I0" width="560"></iframe></div>
