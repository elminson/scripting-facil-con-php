<div class="text-center" markdown="0">

# Comentarios (Documentando el código)
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

### Comentarios de una sola linea
</div>

Los comentarios de una sola linea comienzan con `//` o `#`. Cualquier texto que este a la derecha de estos dos elementos sera ignorado por el interprete de PHP.
La intencion de los cometarios es documentar el codigo y asi dejarle saber a otro ingeniero que hace el codigo o como funciona.

<div class="justify">

```php
// Esto es un comentario y no es interpretado por PHP
# Esto tambien es un cometario 
```

### Otros Ejemplos 
```php 
echo "Hello World!"; // Esto es un comentario, y empieza con "//"
```
### Comentarios en multiples lineas
En algunas ocaciones necesitaremos comentar un block de codigo completo. Para esto empezamos como `/*` y terminamos con `*/`

```php
/* Esto es un comentario de multiples lineas.
Aqui puede ir otro comentario.
Esto tambien es parte del comentario 
*/ 
```

### Docblocks (Bloques de documentacion)

Un Docblock no es más que un bloque de documentación estilo `C` o `C-stlye` para documentar un bloque de código. Comienza con `/**` y tiene un asterisco al principio de cada línea. He aquí un ejemplo:


```php
/**
* Calcula la suma del cuadrado de un arreglo
*
* Ciclo que recorre el arreglo, obtiene el valor lo 
* eleva al cuadrado y se lo suma y retorna el total
*
* @param array $arr Arreglo de valores 
* @return int
* @throws Exception Si el elemento no es un entero
*/
function sumaDeCuadrados($arr)
{

  $total = 0;
  foreach ($arr as $val) {
   if (!is_int($val)) {
    throw new Exception("Elemento no es un entero !");
   }
   $total = $val * $val;
  }

 return $total;
} 
```

El DocBlocks consiste en tres partes todas tres opcionales, la descripción corta, la descripción larga y los tags. La descripción corta, la cual resumen la funcionalidad, la descripción larga la cual explica de manera específica el funcionamiento el cual puede ser tan largo como desee.
<blockquote class='notice'><p>Los tags de los DocBlocks contiene una serie de etiquetas especiales indicados por el símbolo <strong>@</strong></p>
Los tags se utilizan para especificar información adicional, tales como los parámetrosesperados y su tipo.
</blockquote>
No todo el código se puede documentar con DocBlocks, acá están la lista de elemento que deberían ser documentados

- Archivos
- Clases
- Funciones y métodos
- Propiedades de las clases
- Variables Globales
- include()/require()
- define()

Archivos / Files

En los Docblocks se documentan el contenido de un archivo, la mayoría de elementos están documentados mediante la colocación del Docblocks antes del elemento, pero los archivos son una excepción (ya que no puede escribir nada antes de un archivo). A nivel de archivo docblocks se colocan en la primera línea del archivo.

Para este tipo de docblocks es recommendado utilizar las siguientes tags:
`@package`, `@subpackage`, `@license`, y `@author`.  De los tags hablaremos mas adelante.

### Aca un ejemplo de documentación de un file:

```php
/**
* Este Archivo contiene funciones utilizadas dentro del programa
*
* @package    MiProyecto
* @subpackage Comun
* @license    http://opensource.org/licenses/gpl-license.php  GNU Public License
* @author     Emmi V. De Oleo <email@gmail.com>
*/ 
```


### Clases
Un DocBlock de clase es colocado siempre antes de la clase, en esta va la descripción de la clase, 
Generalmente utiliza los tags `@package`, `@subpackage`, and `@author`. Por Ejemplo :

```php
/**
* Un ejemplo de clase
*
* Colocaremos la clase vacia para el ejemplo
*
* @package    MiProyecto
* @subpackage Comun
* @author     Emmi V. < pedropicapiedra@yabadabado.com>
*/
class Example {

} 
```

### Métodos o funciones

Los métodos y las funciones se documentan igual, para los que no saben que es un método, el método es una función, pero esta, 
se encuentra dentro de una clase. Funciones y métodos generalmente contiene los tags `@param` y `@return`,
estos tags nos indicaran el tipo de datos de entrada y el tipo de datos de salida. Ejemplo :

```php
/**
* La división de dos numeros
*
* @param  int $a primero numero ingresado
* @param  int $b Segundo numero entrado
* @return int    Retorna
*/
function division($a,  $b){
 if ($b  > 0) {
  return $a/$b;
 }
 return 0;
} 
```

</div>
