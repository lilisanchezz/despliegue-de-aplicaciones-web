
1. Instale en una máquina virtual un sistema operativo con base Linux (se recomienda
Debian o Ubuntu) e instale apache2.
.
2. Explique con sus palabras que es una petición GET, POST, PUT y DELETE,
remarcando sus diferencias.
.
3. Cambie del puerto 80 al puerto 4444 el servidor apache2. Muestra desde el navegador
su funcionamiento adjuntando una captura de pantalla. 


<img width="370" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/67bf7942-eba2-4d1b-b5e0-68f0dc213c55">

<img width="545" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/a5f47e25-8095-486a-931b-a170122e13a5">

5.
¿Dónde se encuentran los ficheros de configuración de Apache2?

• Ubicación principal.
Se encuentra en esta URL: /etc/apache2/apache2.conf

• Explora el archivo apache2.conf. Identifica las secciones principales y describe
su propósito.
<img width="404" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/c5a98791-5a1a-4320-9531-3c2184496716">
<img width="407" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/43c65150-9bb0-4e61-a095-8989d62888cc">

Entre les seccions principals trobem el ServerRoot:
<img width="346" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/787379c9-9eb7-43d4-a492-e795c4dc95a5">
El mutex:
<img width="425" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/b375a7be-e04c-4c4d-b6cc-4850f878945a">
<img width="210" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/19447537-d446-4681-98da-53216ced51a6">
<img width="374" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/85a56fec-a672-45f9-a054-fe8955252d14">

• sites-available y sites-enabled: Explica la diferencia entre estos dos directorios
y cómo funcionan juntos.
• mods-available y mods-enabled: Explica la diferencia entre estos dos
directorios.