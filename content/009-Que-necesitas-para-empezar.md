<div class="text-center" markdown="0">

# Lo que necesitas para empezar
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

</div>

<div class="justify">
<p>
Hoy en día tenemos muchas opciones para poder ejecutar código PHP. PHP es multiplataforma, por lo tanto te permite operar en varios sistemas operativos. Funciona excelente en LINUX, UNIX, MacOS y Windows. También funciona sin esfuerzos con Apache/MySQL.
</p>
<p>
PHP es conocido como un lenguaje basado en servidores. Esto es porque el PHP no se ejecuta en tu computadora, sino en la computadora que visita la página (servidor).
</p>
</div>

<div class="justify">

### Diferentes formas de ejecutar archivos PHP

<p>
Hay dos maneras de ejecutar archivos PHP. La manera preferida de ejecutar archivos PHP es dentro de un servidor web como Apache, Nginx o ISS; esto te permite ejecutar scripts de PHP desde tu navegador. ¡Así es como funcionan todos los sitios web en PHP! La otra manera es ejecutar scripts de PHP en la línea de comandos, y esto no requiere que establezcas un servidor web.
</p>
<p>
Desde luego, si quieres publicar tus páginas de PHP en línea, tendrás que elegir la opción de establecer un servidor web. Por otro lado, ejecutar scripts de PHP desde la línea de comandos es útil para realizar tareas de rutina.
</p>
<p>
Estas generalmente están configuradas para ejecutarse en segundo plano como trabajos y se ejecutan mediante el comando php sin un servidor web. De hecho, hoy en día muchos scripts o aplicaciones en PHP vienen con comandos integrados que se usan para realizar diversas operaciones, como instalar software, exportar e importar entidades de bases de datos, limpiar la memoria caché y más. Quizá hayas oído hablar de Composer; es un administrador de dependencias para PHP y es una de las herramientas más populares desarrolladas para PHP destinado a la línea de comandos.
</p>

### Ejecuta un archivo PHP en un servidor web

<p>
Si quieres ejecutar scripts de PHP desde un servidor web, necesitas con- figurarlo con uno de los servidores web que son compatibles con él. Para Windows, el servidor web IIS es uno de los más populares de entre los demás. Por otro lado, Apache y Nginx son servidores web ampliamente utilizados para el resto de los sistemas operativos.
</p>
<p>
La buena noticia es que la mayoría de los proveedores de alojamiento tendrán un servidor web con PHP ya configurado para ti cuando inicies sesión en tu nuevo servidor.
</p>

### Ejecuta un archivo PHP en el navegador para el desarrollo con XAMPP

<p>
Si quieres ejecutar un archivo PHP en el navegador en tu propia computadora, necesitarás establecer una pila de desarrollo PHP. Necesitarás al menos PHP, MySQL y un servidor como Apache o Nginx. MySQL se usa para configurar bases de datos con las que tus aplicaciones de PHP puedan trabajar. Desde luego, puedes elegir trabajar con otros motores de bases de datos, pero MySQL es uno de los motores de bases de datos más populares usados junto con PHP.
</p>
<p>
En vez de descargar todo este software por separado y configurarlo para que funcione en conjunto, te recomiendo que solamente descargues e instales un programa como XAMPP. Este incluirá todo el software necesario y te preparará para ejecutar PHP en muy poco tiempo. Y sí, es compatible con Windows, Linux y MacOS.
</p>
<p>
XAMPP contiene todo lo que es necesario para compilar tus páginas web localmente. Es cómodo y te permite comenzar a desarrollar con PHP de inmediato.
</p>
<p>
Una vez que hayas instalado el software XAMPP localmente y que se ejecute con éxito, deberías poder ver la página predeterminada de XAMPP en https://localhost en tu navegador.
</p>

### Ejecuta tu archivo PHP en XAMPP
<p>
Lo primero que necesitarás saber después de instalar XAMPP es la ubicación en donde colocarás tus archivos PHP. Cuando instalas el software XAMPP, este crea el directorio htdocs, que es la raíz de los documentos de tu dominio de servidor web predeterminado: localhost. Entonces, si vas a http://localhost/ejemplo.php, el servidor intentará encontrar el archivo ejemplo.php dentro del directorio htdocs.
</p>
<p>
La ubicación del directorio htdocs varía dependiendo del sistema operativo que estés usando. Para Windows, este debería encontrarse en C:\xampp\ht- docs. De otro modo, este debería encontrarse en /opt/lampp/htdocs para los usuarios de Linux. Una vez que hayas encontrado la ubicación del directorio htdocs, ¡puedes comenzar a crear archivos PHP de inmediato y ejecutarlos en tu navegador!
</p>
<p>
phpinfo() es una función muy útil que te brinda información sobre tu servidor y la configuración de PHP. Generemos un archivo phpinfo.php dentro del directorio htdocs con el siguiente contenido:
</p>

```php
<?php
// Show all information, defaults to INFO_ALL
phpinfo();
?>
```
<p>
Ahora sigue adelante y ejecútalo en tu navegador en http://localhost/phpinfo.php, y deberás ver una salida como esta:
</p>

[<img class="big" src="assets/phpinfo.php.png" width="550"/>](assets/phpinfo.php.png)

</div>
<div class="text-center">
Ya ahora sabes lo necesario para empezar! (si te encuentras con algun problema puedes buescar en internet el problema)
</div>