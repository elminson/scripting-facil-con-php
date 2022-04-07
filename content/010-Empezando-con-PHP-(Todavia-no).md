<div class="text-center" markdown="0" xmlns="http://www.w3.org/1999/html">

# Empezando con PHP <br>(Todavía no)
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

</div>

<div class="justify">
<p>
Para comenzar a entender PHP debes saber algunos conceptos básico de programación. Sin estos conceptos básicos, vas a creer que es difícil aprender PHP, también a este puntos si te interesa aprender PHP deberías saber estos conceptos, de igual manera aquí un pequeño resumen de algunos conceptos. Si ya tienes estos conceptos básicos puedes ir al directamente próximo capitulo.
</p>
<p>
Todos los lenguajes de programación comparten algunos elementos básicos que funcionan y se usan de forma diferente en cada lenguaje, pero que cumplen el mismo objetivo. Esos elementos son:
</p>

- Tipos de datos 
- Variables
- Control de flujo 
- Ciclos
- Estructuras de datos 
- Funciones

### Tipos de datos
<p>
Algunos lenguajes de programación tienen más tipos de datos que otros, pero, en general, todos incluyen al menos los siguientes: caracteres (char), cadenas de caracteres (string), enteros (integer), decimales (decimal, float), y booleanos (true y false). Por ejemplo:
</p>

```php
"Hola Mundo" #Cadenas de caracteres
34 #Enteros
23.45 #Decimales
false #Booleano
```

### Variables
<p>
Las variables nos permiten almacenar información temporalmente. Por ejemplo, podemos almacenar la cadena “Hola Mundo” en una variable.
</p>

```php
$miPrimeraVariable = "Hola Mundo";
```
Mas adelante hablaremos mas de Variables

### Un mecanismo para tomar de decisiones
<p>
Un elemento muy importante en todo lenguaje de programación es cómo tomar una decisión según la información que se tenga en las variables. Por ejemplo:
</p>

```php
<?php

$puntos = 20;

if ($puntos > 15){
    print("Felicidades, tienes mas de 15 puntos!");
} else {
    print("Muy Regurlar, tienes menos de 15 puntos!");
}
```
<p>
A esto se le llama <strong>control de flujo</strong> porque cuando el programa está corriendo, los <strong>if</strong> deciden qué código se ejecuta.
</p>

### Un mecanismo para iterar (ciclos)
<p>
Por ejemplo, cuando queremos imprimir los números de 0 hasta 9.
</p>

```php
<?php

$numeroMaximo = 10;

for ($indice = 0; $inicio < $numeroMaximo; $indice++){
    print($indice);
}

```
### Estructuras de datos (Array)
<p>
Las estructuras de datos existen porque programar únicamente con los tipos básicos (char, integer, boolean, etc) sería muy difícil. A veces necesitamos almacenar colecciones de datos e información más estructurada.
</p>
<p>
Los arreglos son los más conocidos, nos permiten almacenar varios datos en una sola variable.
</p>

```php
<?php

$arreglo = [1, 2, 3, 4, 5];
print($arreglo[2]); // 3
```
<blockquote class='notice'><p>El primer elemento de los arreglos empieza en <strong>0</strong></p>
<p>Esto quiero decir que el valor de:</p>
<p>$arreglo[0] es <strong>1</strong></p>
<p>$arreglo[1] es <strong>2</strong></p>
<p>$arreglo[2] es <strong>3</strong></p>
<p>$arreglo[3] es <strong>4</strong></p>
<p>$arreglo[4] es <strong>5</strong></p>
</blockquote>
<p>
A veces se necesita guardar información más estructurada. Por ejemplo, los datos de una persona.
</p>

```php
<?php

$person = [];
$person["name"] = "Juan Torres";
$person["gender"] = "masculino";
$person["age"] = 25;
print($person["gender"]); //imprimira masculino 
```

### Funciones
<p>
Las funciones, también llamadas procedimientos o métodos, encapsulan algunas instrucciones y se pueden llamar utilizando el nombre de la función.
</p>

```php
<?php

/**
 * Que lenguaje rockea!
 *
 * @param string $lenguaje El lenguage de programacion
 *
 * @return void
 */
function rockear($lenguaje)
{

	print($lenguaje . " rocks!");
	$ejemplo = "asdf";
	echo $Ejemplo;
}

rockear("PHP");
 
```
<br><br><br>
```bash
$php rockear.php 
$PHP Rocks! // Esta sera la salida
```
<p>
Estos son los elementos (super simplificado) que se necesitan para aprender a programar y empezar a crear tus primeros programas en PHP.
</p>

</div>