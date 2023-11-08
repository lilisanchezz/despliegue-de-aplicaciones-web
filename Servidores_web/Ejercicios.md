1. Crea dos sitios web que compartirán IP y puerto, pero tendrán nombres DNS distintos
para acceder a ellos. El nombre del primer dominio será daw.gimbernat.eug.es y el
segundo tunombreyapellidos.gimbernat.eug.es, donde “tunombreyapellidos” contiene
la inicial de tu nombre, el primer apellido, y la inicial de tu segundo apellido. De esta
manera, si tu nombre es: Francisco Mesas Cervilla, el domino quedaría:
fmesasc.gimbernat.eug.es.
• En el primer caso, daw.gimbernat.eug.es tendrá su directorio base en
/var/www/daw/ conteniendo una página llamada index.html que ponga el
nombre de la clase como título con un archivo css para aplicarle estilos al título.
• En el segundo caso, fmesasc.gimbernat.eug.es tendrá su directorio base en
/var/www/fmesasc/ (el equivalente para vuestros nombres), conteniendo una
página llamada index.html que contenga vuestro currículum aplicándole un
estilo css para que se visualice correctamente.
Para ello, tendrás que crear un archivo de configuración (copiado de 000-default.conf)
para cada uno de los dominios. Recuerda que con a2ensite puedes crear los enlaces
simbólicos necesarios para añadir esta configuración a la ejecución de apache.
<img width="490" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/e113130b-c629-4dd3-aaa8-45463b32816e">  

<img width="490" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/138813a4-f2f3-4b04-bcec-c2f4bd1a2fc7">  
<img width="476" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/994ebf82-3823-4ad9-b8b7-d03d7870074c">

<img width="500" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/3922cb77-560b-4f2e-a2e3-bf71f8b8719a">  
<img width="475" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/acbe0175-a016-468b-8537-3d28eaa8543d">
<img width="541" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/6c94d82e-4c5c-45d2-9091-1e8fa5754e7a">
<img width="436" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/90f31270-bc6d-418c-aafa-29cbd587168a">
<img width="485" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/14910e15-ba86-42c3-b862-ef430b134a5b">




<img width="483" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/99db41ad-2b8e-446c-abc3-7b825d2d6647">
<img width="473" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/8a632321-9cbb-4c29-bcf5-3abfe8e9ac6b">
<img width="539" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/72e0cdde-837f-41a6-b4bf-1df2f7463ff9">
<img width="485" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/cd0da933-30de-4043-bc67-54cc6073a201">










