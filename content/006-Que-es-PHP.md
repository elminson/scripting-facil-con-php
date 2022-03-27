<div class="text-center" markdown="0">

# Que es PHP?
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

</div>


<div class="justify">
PHP (acrónimo recursivo de PHP: Hypertext Preprocessor*) fue creado por Rasmus Lerdorf y apareció en 1995, es un lenguaje de programación de propósito general de código abierto ampliamente utilizado, es especialmente adecuado para el desarrollo web y se puede incrustar en HTML.
Bien, pero ¿qué significa realmente? Un ejemplo nos puede aclarará las cosas:
</div>
<br>

<strong>Ejemplo #1 Un ejemplo introductorio</strong>

```php
<!DOCTYPE html>
<html lang="es" dir="ltr">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ejemplo básico PHP</title>
</head>

<body>
  <?php
    echo 'Hola mundo'; // Esto es PHP!!
  ?>
</body>

</html>
```

<div class="justify">
<p>En lugar de usar muchos comandos para mostrar HTML (como en C o en Perl), las páginas de PHP contienen HTML con código incrustado que hace
“algo” (en este caso, mostrar “¡Hola, soy un script de PHP!).</p>
<p>El código de PHP está encerrado entre las etiquetas especiales de comienzo y
final <strong><?php</strong> y <strong>?></strong> que permiten entrar y salir del “modo PHP”. </p>
<p>Lo que distingue a PHP de algo del lado del cliente como Javascript es que el código es ejecutado en el servidor, generando HTML y enviándolo al cliente. El cliente recibirá el resultado de ejecutar el script, aunque no se sabrá el código subyacente que era. El servidor web puede ser configurado incluso para que procese todos los ficheros HTML con PHP, por lo que no hay manera de que los usuarios puedan saber qué se tiene debajo de la manga. </p>
<p>Lo mejor de utilizar PHP es su extrema simplicidad para el principiante, pero a su vez ofrece muchas características avanzadas para los programadores profesionales. No sienta miedo de leer la larga lista de características de PHP. En unas pocas horas podrá empezar a escribir sus primeros scripts.</p>
</div>

<strong>Ejemplo #2</strong>

```php
class Coche {

    public $color = 'rojo';
    public $potencia;
    public $marca;

    public function getColor()
    {
        return $this->color;
    }
}

$miCoche = new Coche();
$miCoche->color = 'verde';
$miCoche->potencia = 120;
$miCoche->marca = 'audi';
```
<div class="center">
No te preocupes, aprenderás que significa cada elemento de este programa
</div>