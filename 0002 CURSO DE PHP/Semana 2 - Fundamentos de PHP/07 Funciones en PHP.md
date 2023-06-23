Ejemplos de uso y ejemplos de código para trabajar con funciones en PHP:

1. Declaración de funciones:
   - Las funciones en PHP se declaran utilizando la palabra clave `function`, seguida del nombre de la función y paréntesis `()`. El código de la función se coloca entre llaves `{}`.
   - Las funciones pueden tener parámetros, que son variables que se pasan a la función para personalizar su comportamiento.
   - Las funciones pueden o no tener un valor de retorno. Si no se especifica un valor de retorno, la función puede realizar acciones sin devolver un resultado específico.

Ejemplo de declaración de función:
```php
function saludar() {
    echo "¡Hola! Bienvenido al curso de PHP.";
}
```

2. Paso de parámetros a las funciones:
   - Los parámetros se definen dentro de los paréntesis de la declaración de la función. Puedes definir uno o varios parámetros separados por comas.
   - Los parámetros permiten que los datos sean pasados a la función para su procesamiento interno. Puedes utilizar los parámetros como variables dentro de la función.

Ejemplo de función con parámetros:
```php
function saludar($nombre) {
    echo "¡Hola, $nombre! Bienvenido al curso de PHP.";
}
```

3. Retorno de valores desde una función:
   - Una función puede devolver un valor utilizando la palabra clave `return`, seguida del valor que deseas devolver.
   - El valor devuelto puede ser utilizado en otras partes del código, asignado a una variable o utilizado directamente en expresiones.

Ejemplo de función con retorno de valor:
```php
function sumar($a, $b) {
    return $a + $b;
}
```

Ejemplos de uso de las funciones:

- Ejemplo 1: Llamada a una función sin parámetros:
```php
saludar();  // Imprime: ¡Hola! Bienvenido al curso de PHP.
```

- Ejemplo 2: Llamada a una función con parámetros:
```php
saludar("Juan");  // Imprime: ¡Hola, Juan! Bienvenido al curso de PHP.
```

- Ejemplo 3: Llamada a una función con retorno de valor:
```php
$resultado = sumar(5, 3);  // Asigna el valor 8 a la variable $resultado.
echo "El resultado de la suma es: " . $resultado;  // Imprime: El resultado de la suma es: 8.
```

Estos ejemplos ilustran cómo declarar funciones en PHP, pasar parámetros a ellas y utilizar el valor devuelto. Las funciones son una poderosa herramienta para encapsular bloques de código y reutilizarlos en diferentes partes de tu aplicación. Te permiten modularizar tu código y hacerlo más legible y mantenible.