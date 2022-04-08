<div class="text-center" markdown="0">

# Variables
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

### ¿Qué es una Variable en PHP?
<div class="justify">
Las variables se utilizan para almacenar datos, como cadenas de texto, números, etc. Los valores de las variables pueden cambiar en el transcurso de un script. 
Aquí hay algunas cosas importantes que debe saber sobre las variables:

En PHP, no es necesario declarar una variable antes de agregarle un valor. PHP convierte automáticamente la variable al tipo de datos correcto, según su valor.
Después de declarar una variable, se puede reutilizar en todo el código.
El operador de asignación (=) utilizado para asignar valor a una variable.
En PHP, la variable se puede declarar como:
```php
#Variable estilo snake
$var_name = 'valor';

#Variable estilo Camelcase
$varName = 'valor';

echo $varName; # retorna: valor

function add($a, $b) { 
    return $a + $b;
}

$suma = add(1, 2); // ahora la variable $suma tiene el valor 3
```
</div>
</div>

