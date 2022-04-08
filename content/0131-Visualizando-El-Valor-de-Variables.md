<div class="text-center" markdown="0">

# Visualizando el valor de Variables
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

#### echo y print
<div class="justify">
El lenguaje PHP nos permite varias formas de imprimir (visualizar) el valor de una variable.

`echo` y `print` son construcciones del lenguaje, no funciones. Esto significa que no requieren paréntesis alrededor del argumento como lo hace una función (aunque uno siempre puede agregar paréntesis alrededor de casi cualquier expresión de PHP y, por lo tanto, `echo ("prueba");` tampoco hará ningún daño). 
Producen la representación de cadena de una variable, constante o expresión. No se pueden usar para imprimir matrices u objetos.

Asigne la cadena Joel a la variable `$nombre`
```php
$nombre = "Joel";
```

Muestra el valor de `$name` usando `echo` & `print`

```php
echo $name; #> Joel
print $name; #> Joel 
```

Los paréntesis no son necesarios, pero se pueden utilizar
```php
echo($name); #> Joel
print($name); #> Joel
```

Usando múltiples parámetros (solo eco)
```php
 echo $name, "Smith"; #> JoelSmith
 echo($name, " ", "Smith"); #> Joel Smith
```

`print`, a diferencia de `echo`, es una expresión (devuelve 1) y, por lo tanto, se puede usar en más lugares: 
```php
print("oye") && print(" ") && print("tu"); #> tu11
```

Lo anterior es equivalente a:
```php
print ("hola" && (print (" " && print "tu"))); #> tu11
```

### Salida de una vista estructurada de matrices y objetos

`print_r()`: generar matrices y objetos para depurar `print_r` generará un formato legible por humanos de una matriz u objeto.
Puede tener una variable que sea una matriz u objeto. Intentar generarlo con un eco generará el error: 
Aviso: conversión de matriz a cadena. En su lugar, puede usar la función print_r para volcar un formato legible por humanos de esta variable.
Puede pasar `true` como segundo parámetro para devolver el contenido como una cadena.
```php
$myobject = new stdClass(); 
$myobject->myvalue = 'Hello World'; 
$myarray = [ "Hello", "World" ]; 
$mystring = "Hello World";
$myint = 42;

// Usando print_r podemos ver los datos que contiene la matriz.
print_r($myobject);
print_r($myarray);
print_r($mystring);
print_r($myint);
//Esto genera lo siguiente:
```
```bash
stdClass Object
(
    [myvalue] => Hello World
)
Array
(
[0] => Hello
[1] => World )
Hello World
42
```
`var_dump()`: genera información de depuración legible por humanos sobre el contenido de los argumentos, incluido su tipo y valor
La salida es más detallada en comparación con print_r porque también genera el tipo de variable junto con su valor y otra información como ID de objeto, tamaños de matriz, longitudes de cadena, marcadores de referencia, etc.
Puede usar var_dump para generar una versión más detallada para la depuración.

```php
var_dump($myobject, $myarray, $mystring, $myint);
```
La salida es más detallada:
```bash
object(stdClass)#12 (1) { ["myvalue"]=>
  string(11) "Hello World"
}
array(2) {
  [0]=>
  string(5) "Hello"
  [1]=>
  string(5) "World"
}
string(11) "Hello World"
int(42) 
```

#### Concatenación de cadenas con `eco`
Puede usar la concatenación para unir cadenas "de extremo a extremo" mientras las genera (con eco o impresión, por ejemplo). Puede concatenar variables usando un . (punto).
```php
// String variable
$name = 'Joel';
// Concatenate multiple strings (3 in this example) into one and echo it once done. // 1. ↓ 2. ↓ 3. ↓ - Three Individual string items
echo '<p>Hello ' . $name . ', Nice to see you.</p>';
// ↑ ↑ - Concatenation Operators
#> "<p>Hello Joel, Nice to see you.</p>"
```
#### Genere una matriz multidimensional con índice y valor e imprima en una tabla
```php
$array = [  0 => [
                    [id] => 13
                    [category_id] => 7
                    [name] => Leaving Of Liverpool
                    [description] => Leaving Of Liverpool
                    [price] => 1.00
                    [virtual] => 1
                    [active] => 1
                    [sort_order] => 13
                    [created] => 2007-06-24 14:08:03
                    [modified] => 2007-06-24 14:08:03
                    [image] => NONE
                   ],
            1 => [
                    [id] => 16
                    [category_id] => 7
                    [name] => Yellow Submarine
                    [description] => Yellow Submarine
                    [price] => 1.00
                    [virtual] => 1
                    [active] => 1
                    [sort_order] => 16
                    [created] => 2007-06-24 14:10:02
                    [modified] => 2007-06-24 14:10:02
                    [image] => NONE
                   ]
     ];
 ```
```html
<table>
<?php
foreach ($products as $key => $value) {
    foreach ($value as $k => $v) {
        echo "<tr>";
        echo "<td>$k</td>"; // Get index. echo "<td>$v</td>"; // Get value. echo "</tr>";
    } 
}
?>
</table>
```

</div>
</div>

