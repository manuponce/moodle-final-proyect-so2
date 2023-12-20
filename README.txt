Para mejorar el aspecto visual en el README de GitHub, puedes utilizar distintos métodos para formatear el texto y las imágenes. Aquí te muestro cómo podrías organizar el texto y las imágenes para que se vea más ordenado y legible:

```markdown
### INSTALANDO MOODLE Y SUS DEPENDENCIAS

#### Descarga de Moodle
```bash
~$ wget https://download.moodle.org/download.php/direct/stable400/moodle-latest-400.tgz
```
![Descarga de Moodle](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.020.png)

#### Instalación de Apache
```bash
~$ sudo apt install -y apache2
```
![Instalación de Apache](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.021.png)

#### Descompresión de Moodle
```bash
~$ sudo tar xf moodle-latest-400.tgz -C /var/www/html/
```
![Descompresión de Moodle - Paso 1](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.022.png)
![Descompresión de Moodle - Paso 2](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.023.png)

#### Creación del directorio de datos para Moodle
```bash
~$ sudo mkdir /var/www/moodledata
~$ sudo chown -R www-data: /var/www/html/moodle/ /var/www/moodledata/
```
![Creación de directorio de datos para Moodle](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.024.png)

#### Instalación de extensiones de PHP para Moodle
```bash
~$ sudo apt install -y php-{curl,gd,intl,mbstring,soap,xml,xmlrpc,zip}
```
![Instalación de extensiones de PHP para Moodle](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.025.png)

#### Configuración de PHP
```bash
~$ sudo nano /etc/php/8.0/apache2/php.ini
```
![Configuración de PHP](Aspose.Words.e7ac596c-2d04-4ee4-b8d2-8d04ee08328c.026.png)

#### Recarga del servicio web Apache
```bash
~$ sudo systemctl reload apache2
```
...

(Continúa con el resto de los pasos)

### INSTALACIÓN DE MOODLE - PASOS FINALES
...

```

En el ejemplo proporcionado, he utilizado encabezados de diferentes niveles (`###` y `####`) para organizar el contenido y los pasos de instalación. También he ajustado la ubicación y los títulos de las imágenes para que coincidan con los pasos correspondientes.

Recuerda reemplazar los títulos y la información de los comandos según corresponda. Además, asegúrate de que las imágenes estén en el directorio correcto y con los nombres adecuados para que puedan mostrarse correctamente en GitHub.
