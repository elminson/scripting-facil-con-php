<div class="text-center" markdown="0">

# Características de PHP
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

</div>


<div class="justify">
Orientado al desarrollo de aplicaciones web dinámicas con acceso a información almacenada en una base de datos.

- Es considerado un lenguaje fácil de aprender, ya que en su desarrollo se simplificaron distintas especificaciones, como es el caso de la definición de las variables primitivas, ejemplo que se hace evidente en el uso de php arreglos(array).

- El código fuente escrito en PHP es invisible al navegador web y al cliente, ya que es el servidor el que se encarga de ejecutar el código y enviar su resultado HTML al navegador.

- Capacidad de conexión con la mayoría de los motores de base de datos que se utilizan en la actualidad, destaca su conectividad con MySQL y PostgreSQL.

- Capacidad de expandir su potencial utilizando módulos (llamados extensiones).

- Posee una amplia documentación en su sitio web oficial, entre la cual se destaca que todas las funciones del sistema están explicadas y ejemplificadas en un único archivo de ayuda.

- Es libre, por lo que se presenta como una alternativa de fácil acceso para todos.

- Permite aplicar técnicas de programación orientada a objetos.

- No requiere definición de tipos de variables aunque sus variables se pueden evaluar también por el tipo que estén manejando en tiempo de ejecución.

- Tiene manejo de excepciones (desde PHP5).

- Si bien PHP no obliga a quien lo usa a seguir una determinada metodología a la hora de programar, aun haciéndolo, el programador puede aplicar en su trabajo cualquier técnica de programación o de desarrollo que le permita escribir código ordenado, estructurado y manejable. Un ejemplo de esto son los desarrollos que en PHP se han hecho del patrón de diseño Modelo Vista Controlador (MVC), que permiten separar el tratamiento y acceso a los datos, la lógica de control y la interfaz de usuario en tres componentes independientes.

- Debido a su flexibilidad, ha tenido una gran acogida como lenguaje base para las aplicaciones WEB de manejo de contenido, y es su uso principal.

</div>

### Separación de instrucciones
<div class="justify">
Como en <em>C</em> o en <em>Perl</em>, <em>PHP</em> requiere que las instrucciones terminen en punto y coma al final de cada sentencia. La etiqueta de cierre de un bloque de código de PHP automáticamente implica un punto y coma; no es necesario usar un punto y coma para cerrar la última línea de un bloque de PHP. La etiqueta de cierre del bloque incluirá la nueva línea final inmediata si está presente.
Cada script de PHP se compone de instrucciones, tales como funciones, asignaciones de variables, salida de datos, directivas, etc. Excepto en algunos casos, cada uno de estas instrucciones deben terminar (tal como en C, Perl y JS) con un punto y coma.
Estas tres lineas de codigo PHP son validas.
</div>
<br>

```php
<?php
    echo 'Esto es una prueba';
?>

<?php echo 'Esto es una prueba' ?>

<?php echo 'Hemos omitido la última etiqueta de cierre'; 
```