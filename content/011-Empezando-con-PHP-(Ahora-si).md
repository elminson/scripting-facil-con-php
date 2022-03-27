<div class="text-center" markdown="0">

# Empezando con PHP (Ahora si)
<div>
<img src="assets/vineta.png" class="vineta" />
</div>

</div>

<div class="justify">
<p>
Cada variable consta del símbolo del dólar($), seguido del nombre de la variable. Las variables se utilizan en los scripts de PHP para integrar datos externos en páginas web. En este sentido se puede hablar de valores muy variados que van desde números simples y cadenas de caracteres hasta textos completos o estructuras de documentos HTML.
</p>
<p>
La administración central de los contenidos tiene lugar, en general, con ayuda de sistemas de bases de datos. Los valores para las variables pueden definirse directamente en el script. Este tipo de clasificación se realiza según el esquema siguiente:
</p>

```php
<?php
 $ejemplo = "Valor";
```
<blockquote class='notice'>
<p><strong>Atencion</strong>
Los valores para la variables del tipo entero (integer) y flotante (float) no se escriben en comillas.
</p>
<p>
Ejemplo:

```php
<?php

$entero  = 24;
$flotante = 2.4;
 
```

</p>
</blockquote>
<br>
<p>
PHP te da la libertad de designar variables según tu creas conveniente, pero surgen aquí ciertas limitaciones:

- Cada variable comienza con el símbolo del dólar ($).

- El nombre de las variables es una secuencia de caracteres formada por letras, números y guiones (p.ej., $ejemplo_1).

- Un nombre de variable válido siempre comienza con una letra o con un guion bajo ($ejemplo1 o $_ejemplo), pero nunca con un número (incorrecto: $1ejemplo).

- PHP distingue entre mayúsculas y minúsculas ($ejemplo ≠ $Ejemplo).

- Los nombres de las variables no pueden contener espacios o saltos de línea (incorrecto: $ejemplo 1)

- El usuario no puede hacer uso libre de las secuencias de caracteres reservadas por PHP para otros propósitos (p. ej., $this)
</p>
<p>
Veámoslo en un ejemplo:
</p>

```php
<?php
$author = "John Doe";
echo "<h1>Hello World!</h1>
<p>This dynamic web page was created by $author.</p>";
?> 
```
<div>
<img src="assets/hello.png" />
</div>

<em class="text-center">La palabra reservada <strong>echo</strong> resulta de una utilidad mayor que la propia emisión de texto, la cual puede implementarse también sin PHP y tomando HTML como base. La verdadera plusvalía de <strong>echo</strong> está basada en el hecho de que la instrucción permite generar textos de manera dinámica con ayuda de variables.
</em>
<p>
La etiqueta de apertura de PHP va seguida de la definición de la variable: en el caso de $author se utilizaría el valor John Doe. A la hora de ejecutar el script, la variable $author se sustituye por el valor John Doe cada vez que se haga mención a ella en el entorno del script. El siguiente gráfico muestra cómo se refleja esto en el navegador web.
</p>
</div>