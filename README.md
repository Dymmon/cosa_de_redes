# Web Service SOAP/REST 


### Web Service SOAP
Se debe descargar cualquier version de "apache-tomcat-8.0.X-windows-x64/x86.zip", una vez descargado se debe descomprimir el 
archivo, copie y pege la carpeta resultante en el disco "C:\". Luego debe colocar el archivo "SOAP_Back.war" en la carpeta
"webapps" que está dentro de "apache-tomcat-version". Despues debe ir a las variales de entorno del sistema, una vez dentro 
en "Variales del sistema" debe ver si estan creadas las variable JAVA_HOME y JRE_HOME, de no estar las debera crear dando
click en el boton "nueva" de mas abajo, se dezplejara una pestaña nueva, donde le pedira un "Nombre de la variable" que son
los ya antes mencionados y un "Valor de la variable" en el valor debe poner la direcion de la carpeta de java a utilizar, en
este caso se esta trabajando con java 1.8.0_91, por lo cual la carpeta tendria que ser "C:\Program Files\Java\jre1.8.0_91", 
despues tendre que hacer click en la variable de sistema llamada "Path", una vez dentro de esta tendra que crear dos nuevas
"variables  de entorno" una sera "%CATALINA_HOME%\bin" y la otra sera la carpeta bin del java utilizado que sería
"C:\Program Files\Java\jre1.8.0_91", una vez hecho esto podremos abrir consola de comandos "cmd" y escribir "catalina start"
para iniciar el servidor tomcat, para finalizarlo se tendra que escribir "catalina stop".

## Cliente Web SOAP
Colocar la carpeta "cliente SOAP" en la carpeta inetpub de iss. Abrir administrador de Internet Information Services,
en la sección de "Conexiones" hacer click derecho en "Sitios" y seleccionar la opción "Agregar sitio web". Establecer
un nombre para el sitio y en la sección de "Ruta de acceso física" seleccionar la carpeta "cliente SOAP" antes mencionada.
Escojer un puerto disponible para el usuario y dar click en aceptar.
Posterormente en su navegador al acceder a "localhost:puerto asignado" se debe ver el cliente ejecutandose.
## Web Service Rest
Si no se encuentra la carpeta "Target":
Ubicarse con la terminal en la carpeta Rest y ejecutar el comando "mvn compile"
y luego “mvn clean package spring-boot:repackage” esto generara la carpeta "Target" donde se encuentra el archivo .jar
Ubicarse en la carpeta target y ejecutar el archivo .jar para iniciar el servicio en el localhost:8080.

## Cliente Web REST
-activar el iis desde las características de Windows
-Abrir una consola de comandos y ubicarse en la carpeta netframework 4.0
-ejecutar el comando asp.NET_regiis.exe -ir
-mover la carpeta a intpub 
-abrir el administrador de servicio de internet
-verificar que las aplicaciones por default usen asp.net 4.0
Convertir la carpeta cliente_rest en aplicacion
-examinar la carpeta cliente_rest para obtener la ruta y que esta se abra en el navegador

### Requerimientos
## Para SOAP
  -ISS
  -Tomcat
### Abrir Sitio Web
