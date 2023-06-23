Ejemplos de uso y ejemplos de código de los bucles: for, while y foreach en PHP:

1. Bucle for:
El bucle for se utiliza para repetir una secuencia de código un número específico de veces.

Sintaxis:
```php
for (inicialización; condición; incremento/decremento) {
  // Código a ejecutar en cada iteración
}
```

Ejemplo de uso:
```php
for ($i = 1; $i <= 5; $i++) {
  echo "Iteración: $i <br>";
}
```

2. Bucle while:
El bucle while se utiliza para repetir un bloque de código mientras se cumpla una condición.

Sintaxis:
```php
while (condición) {
  // Código a ejecutar en cada iteración
  // Se debe actualizar la condición para evitar bucles infinitos
}
```

Ejemplo de uso:
```php
$i = 1;
while ($i <= 5) {
  echo "Iteración: $i <br>";
  $i++;
}
```

3. Bucle foreach:
El bucle foreach se utiliza para iterar sobre los elementos de un array o una colección de datos.

Sintaxis:
```php
foreach ($array as $valor) {
  // Código a ejecutar en cada iteración
}
```

Ejemplo de uso con array numérico:
```php
$colores = array("rojo", "verde", "azul");

foreach ($colores as $color) {
  echo "Color: $color <br>";
}
```

Ejemplo de uso con array asociativo:
```php
$personas = array("Juan" => 25, "María" => 30, "Carlos" => 28);

foreach ($personas as $nombre => $edad) {
  echo "Nombre: $nombre, Edad: $edad <br>";
}
```