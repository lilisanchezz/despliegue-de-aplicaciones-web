<img width="490" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/e113130b-c629-4dd3-aaa8-45463b32816e">1. Crea dos sitios web que compartirán IP y puerto, pero tendrán nombres DNS distintos
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

<img width="490" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/138813a4-f2f3-4b04-bcec-c2f4bd1a2fc7">  
<img width="476" alt="image" src="https://github.com/lilisanchezz/despliegue-de-aplicaciones-web/assets/144775558/994ebf82-3823-4ad9-b8b7-d03d7870074c">



