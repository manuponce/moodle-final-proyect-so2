
<a name="_gjdgxs"></a>UNIVERSIDAD PRIVADA

DOMINGO SAVIO












![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.001.png)![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.002.png)




a








**Proyecto Final**
**

Emmanuel Freddy Ponce Quiroga
Leonardo Carrillo
Grethel J. Fernández Orellana**
Luis Andres Zurita Molina

**Turno:** Medio Dia

**Materia: SISTEMAS OPERATIVOS 2

Docente: Ing. Jaime Zambrana Chácon**






![C:\Users\User\Downloads\descarga.png](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.003.png)![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.004.png)![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.005.png)![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.006.png)![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.007.png)![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.008.png)
# **1.   	CARÁTULA**
# **2.   	INDICE**
# **3.   	INTRODUCCION**
# **4.   	OBJETIVO**
# **5.   	MARCO TEORICO**
# **6.   	PROCESO DE FUNCIONAMIENTO**
# <a name="_eyp6tlq8yjhz"></a>**7.   	DIAGRAMA DE FUNCIONAMIENTO**
# <a name="_jq5v04ci8l1d"></a>**8.   	CONCLUSION**
<a name="_b5s1b23bwg85"></a>**9.   	BIIBLIOGRAFIA** 










====================================================
#
#
<a name="_a7b0lwmk0tjy"></a><a name="_u5df30wkdjlt"></a><a name="_o3anh3r74qn7"></a>**INTRODUCCION** 
EL SISTEMA OPERATIVO UNIVERSAL

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.009.png)
Debian es una de las distribuciones 

Linux más conocidas y respetadas. Fue creada por Ian Murdock en 1993, quien se inspiró en el proyecto GNU de la Free Software Foundation y buscaba construir un sistema operativo completamente libre y abierto, basado en el núcleo Linux. El nombre Debian se deriva de la combinación del nombre de Ian y el de su entonces novia, ahora esposa, Debra.**









============================================================================================================================================================================================================================================================================================================================================================
#
#
#
#
<a name="_8zj7bqhxnmot"></a><a name="_nnxmzjfoei75"></a><a name="_gh1kclgrvyb"></a><a name="_i9yhnctsizh"></a><a name="_58j4m59uvmld"></a>

**OBJETIVO**
==========================================================================================================================================
El objetivo principal de Debian es desarrollar un sistema operativo estable, seguro y fácilmente adaptable, manteniendo un compromiso firme con los principios del software libre. Uno de los aspectos fundamentales de Debian es su gestor de paquetes, APT (Advanced Package Tool), que facilita la instalación, actualización y eliminación de software de forma sencilla y eficiente.
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.010.png)



# <a name="_vz1hjswff8lt"></a>**MARCO TEÓRICO**
Google Cloud ![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.011.png)
"Google Cloud Computing es la robusta plataforma en la nube de Google diseñada para proporcionar una amplia gama de servicios y herramientas para empresas y desarrolladores. Ofrece una infraestructura escalable y segura que permite almacenar datos, ejecutar aplicaciones y aprovechar tecnologías innovadoras como el aprendizaje automático y el análisis de datos en tiempo real. Con servicios como almacenamiento de datos, cómputo, bases de datos, aprendizaje automático y herramientas de desarrollo, Google Cloud se destaca por su flexibilidad, potencia y fiabilidad en la gestión y transformación de datos, así como en el despliegue ágil de aplicaciones en la nube para satisfacer las necesidades de distintos tipos de proyectos y empresas."
# <a name="_epeyg3inl1kr"></a>**Configuración de Google Cloud**
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.012.png)
# <a name="_dezgxyblljju"></a>**PROCESO DE FUNCIONAMIENTO**

REGION

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.013.png)

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.014.png)




![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.015.png)

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.016.png)

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.017.png)






***VIRTUAL PRIVATE CLOUD*** 
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.018.png)




![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.019.png)
















***INSTALANDO EL MODDLE Y TODO LO QUE NECESITAMOS***

~$ wget https://download.moodle.org/download.php/direct/stable400/moodle-latest-400.tgz

CESITAMO

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.020.png)






***INSTALAMOS APACHE***
~$ sudo apt install -y apache2

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.021.png)


***Descomprimimos el archivo que acabamos de descargar en su directorio de instalación definitivo:***

~$ sudo tar xf moodle-latest-400.tgz -C /var/www/html/

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.022.png)
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.023.png)



***Moodle necesita también un directorio de datos que crearemos fuera del alcance de la navegación web:***

~$ sudo mkdir /var/www/moodledata

Como Moodle necesita escribir en ambas carpetas a través del servicio web, cambiaremos su propiedad al usuario con el que corre el servicio:

~$ sudo chown -R www-data: /var/www/html/moodle/ /var/www/moodledata/

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.024.png)



***Moodle requiere la presencia en Debian 11 Bullseye de algunas extensiones de este lenguaje que instalaremos desde los repositorios del sistema.***

Si usamos la versión de PHP incluida en Debian 11, instalaremos estos paquetes:

~$ sudo apt install -y php-{curl,gd,intl,mbstring,soap,xml,xmlrpc,zip}

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.025.png)

~$ sudo nano /etc/php/8.0/apache2/php.ini

Buscamos la directiva *max\_input\_vars*:

;max\_input\_vars = 1000

Está desactivada, así que podemos activarla eliminando el carácter ; inicial y modificando su valor por 5000, o la dejamos como está y añadimos en la siguiente línea la nueva definición:
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.026.png)

Finalmente, recargamos la configuración del servicio web para que se puedan utilizar las nuevas extensiones y ajustes:

~$ sudo systemctl reload apache2

Si trabajamos remotamente sobre la máquina Debian 11, podemos realizar la descarga desde consola con alguna herramienta como *wget*:

~$ wget https://dev.mysql.com/get/mysql-apt-config\_0.8.24-1\_all.deb

Una vez descargado este paquete procedemos a instalarlo:

~$ sudo dpkg -i mysql-apt-config\_0.8.24-1\_all.deb

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.027.png)
Conectamos al servicio con el cliente *mysql* y un usuario administrador:

~$ mysql -u root -p

Creamos la base de datos:

\> create database moodle character set utf8mb4 collate utf8mb4\_unicode\_ci;

Creamos el usuario:

\> create user moodle@localhost identified by 'XXXXXXXX';

Concedemos los permisos necesarios al usuario sobre la base de datos:

\> grant all privileges on moodle.\* to moodle@localhost;

Refrescamos la tabla de permisos:

\> flush privileges;

Y cerramos la conexión:

\> exit

***INSTALACIÓN DE MOODLE FINAL
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.028.png)***
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.029.png)
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.030.png)
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.031.png)
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.032.png)







***Usuarios Involucrados***
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.033.png)
Comando utilizado: 

\# tail -n 7 etc/passwd



***Software instalados: Apache
Instalación de apache:***

***sudo apt install apache2***

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.034.png)
Versión instalada de Apache2:

comando para verificar la versión:

apache2 -v


![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.035.png)



















***MySQL Server*** 

***Comando de instalación:***

***sudo apt install mysql-server***

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.036.png)

Versión instalada de MySQL:

comando de verificación: mysql -V

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.037.png)



***Php***

***Comando de instalación:***

***sudo apt install php***

![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.038.png)
![](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.039.png)Versión instalada de Php:

comando de verificación: php -V






**CONCLUSION GENERAL**
<a name="_urdfrlxc3oz6"></a>**

==============================
# <a name="_3y6t3a61b08a"></a>**BIIBLIOGRAFIA** 
