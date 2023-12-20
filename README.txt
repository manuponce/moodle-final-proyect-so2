***INSTALANDO EL MODDLE Y TODO LO QUE NECESITAMOS***

~$ wget https://download.moodle.org/download.php/direct/stable400/moodle-latest-400.tgz


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



