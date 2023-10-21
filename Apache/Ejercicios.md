
**1. Instale en una máquina virtual un sistema operativo con base Linux (se recomienda
Debian o Ubuntu) e instale apache2.**
.
**2. Explique con sus palabras que es una petición GET, POST, PUT y DELETE,
remarcando sus diferencias.**
GET:Para realizar peticiones al servidor. No se modifican los datos del servidor
POST:Envío formularios HTML pudiendo modificar datos del servidor
PUT: Para crear o reemplazar un determinado recurso del servidor  
DELETE:Permite elimianr un recurso o documento del servidor

**3. Cambie del puerto 80 al puerto 4444 el servidor apache2. Muestra desde el navegador
su funcionamiento adjuntando una captura de pantalla.**

<img width="531" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/0aba2470-8f34-46dd-8eac-cb184049103c">

**Instale un certificado SSL y configure su Apache para servir contenido a través de
HTTPS en el puerto 4444. Muestre desde el navegador cómo se muestra el sitio web
como "seguro" (aunque sea un certificado autofirmado).**
<img width="400" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/db1784e5-3483-4671-ac61-87fa993b081e">
<img width="449" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/df483a6c-0942-4f7b-b10b-ed1944c5415d">


<img width="370" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/67bf7942-eba2-4d1b-b5e0-68f0dc213c55">
<img width="455" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/15f8b99f-e71f-4e4d-9d08-23d8a5b7e396">
<img width="214" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/c10d4fec-22d7-4b05-be1e-c34d38e5bc76">

<img width="485" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/ba773583-b467-430f-b62c-7d80bd6f900c">


**5.¿Dónde se encuentran los ficheros de configuración de Apache2?**  

**• Ubicación principal.**  
Se encuentra en esta URL: /etc/apache2/apache2.conf

**• Explora el archivo apache2.conf. Identifica las secciones principales y describe
su propósito.**  
<img width="404" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/c5a98791-5a1a-4320-9531-3c2184496716">  
<img width="407" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/43c65150-9bb0-4e61-a095-8989d62888cc">  

**Entre les seccions principals trobem el ServerRoot:** 
<img width="346" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/787379c9-9eb7-43d4-a492-e795c4dc95a5">  
El mutex:  
<img width="425" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/b375a7be-e04c-4c4d-b6cc-4850f878945a">  
<img width="210" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/19447537-d446-4681-98da-53216ced51a6">  
<img width="374" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/85a56fec-a672-45f9-a054-fe8955252d14">  

**• sites-available y sites-enabled: Explica la diferencia entre estos dos directorios  
y cómo funcionan juntos.**  

El sites-available indica el directorio que contiene los sitios disponibles en la instalación
actual. En cambio el sites-enabled se refiere al directorio que incluye mediante enlaces simbólicos al directorio
anterior, los sitios que va a utilizar Apache la próxima vez que se inicie   

**• mods-available y mods-enabled: Explica la diferencia entre estos dos
directorios.**  

El mods-available se refiere al directorio que contiene los módulos disponibles en la instalación actual, y el mods-enabled indica el directorio que incluye mediante enlaces simbólicos al directorioanterior, los módulos que se van a cargar en memoria la próxima vez que se inicie
Apache.  
**6. ¿Dónde se encuentran los ficheros de ejecución de Apache2?**
**• Ubicación principal**  

**• Control del servicio: Utiliza el binario de ejecución para iniciar, detener,
recargar y reiniciar el servidor Apache2 explicando la diferencia entre cada uno
de los comandos utilizados.**  
Para iniciar se utiliza el comando sudo systemctl start apache2  
Para detener utilizamos el sudo systemctl stop apache2
Para recargar tenemos el comando sudo systemctl reload apache2  
Y finalmente para reaniciarlo usamos el comando sudo systemctl restart apache2  
**• Comprobación de sintaxis: Usa el binario de Apache para verificar la sintaxis
de tu configuración. Esto es útil para asegurarse de que no haya errores antes
de reiniciar el servidor**  
<img width="433" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/e3f44969-8c34-4285-9bac-52d935d15b7f">  
Me sale este error, he modificado el archivo apache2.conf añadiendo el ServerName pero me sigue saliendo mal.  

**7. ¿Dónde se encuentran los ficheros de monitorización de Apache2?**  

**• Ubicación principal**  
/var/log/apache2/access.log  
/var/log/apache2/error.log


**• error.log y access.log: Explica la diferencia entre estos dos archivos. Abre y
revisa las entradas recientes en cada uno de ellos.**  
El error.log  registra eventos y errores relacionados con el funcionamiento del servidor web  
El archivo access.log registra cada solicitud HTTP que llega al servidor.   

<img width="446" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/712d149b-cc81-4db2-abe9-c7db738fefa0">

<img width="436" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/ccfc517a-c971-4b4e-b996-559723c0691c">  **Rotación de logs: Investiga cómo funciona la rotación de logs en Apache2.¿Por qué es importante?¿Cómo se configura?**

Es un proceso que implica el archivo y el resguardo de los archivos de registro (logs) antiguos del servidor web para evitar que ocupen un espacio en disco excesivo y para facilitar la administración de registros
<img width="434" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/955f9a25-da48-4b4d-9dbd-e23620f89a42">  
**Monitorización en tiempo real: Utiliza herramientas como tail -f para monitorear
en tiempo real los accesos a tu servidor web y posibles errores**  
<img width="467" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/9223157d-47a3-4ac6-be03-71576464081b">
**• Análisis de logs: Instala y usa herramientas como goaccess para analizar y
obtener estadísticas visuales a partir de tus logs de Apache2.**  
<img width="492" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/d357661d-3892-44bc-905e-b3cb27da7e17">  
<img width="516" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/9596ae39-4c71-4fa9-9029-736a85446c29">
**¿Qué es un Firewall? ¿Para qué sirve? ¿Por qué es necesario? Instale y configure un
Firewall en la máquina virtual para que solo permita tráfico HTTP y HTTPS. Bloquee
todo el resto de los puertos y demuestre su funcionamiento**
Un firewall es un dispositivo de seguridad de la red que monitoriza el tráfico entrante y saliente y decide si debe permitir o bloquear un tráfico específico en función de un conjunto de restricciones de seguridad ya definidas. Es necesario para para protegernos de amenazas externas y que haya un control de tráfico.
<img width="451" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/71500b82-7b9e-4153-88aa-d99ba53d38c6">  
<img width="536" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/9c449648-a02a-4873-9bb0-b1c75c43d735">  
<img width="497" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/6e2feb94-5862-44f8-8593-1e39d00b67ff">  
**9. Explica con tus palabras las diferentes partes de una URL**
En un URL encontramos diferentes partes, entre estas estan:
- El protocolo, por ejemplo seria https
- El host, ://www.google.es:
- El puerto, podrian ser diferentes, como por ejemplo el 443
- La ruta que es basicamente la ubicación
- La consulta
**10. Explica el funcionamiento del protocolo HTTP con tus palabras.**
  El protocolo HTTP lo que hace es establecer el intercambio de documentos hipertexto en la web
  **11. ¿Qué es un archivo .htaccess? Proporcione un ejemplo de cómo se puede utilizar
para reescribir URL o restringir el acceso a ciertas partes de su sitio web.**
El archivo htaccess es un archivo oculto que se utiliza para configurar funciones adicionales para sitios web alojados en el servidor web Apache. 







