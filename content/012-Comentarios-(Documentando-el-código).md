<div class="text-center" markdown="0">

# Comentarios (Documentando el código)
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

### Comentarios de una sola linea
</div>

Los comentarios de una sola linea comienzan con `//` o `#`. Cualquier texto que este a la derecha de estos dos elementos sera ignorado por el interprete de PHP.
La intencion de los cometarios es documentar el codigo y asi dejarle saber a otro ingeniero que hace el codigo o como funciona.

<div class="text-justify">

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

Un Docblock no es más que un  bloque de documentación  estilo  C o C-stlye para documentar un bloque de código. Comienza con `/**` y tiene un asterisco al principio de cada línea. He aquí un ejemplo:


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
			throw new Exception("El elemento no es un entero !");
		}
		$total = $val * $val;
	}

	return $total;
} 
```
</div>
