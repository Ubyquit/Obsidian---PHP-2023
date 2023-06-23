Ejemplos de uso y ejemplos de código para las estructuras de control if, else y switch en PHP:

1. Uso del condicional if para tomar decisiones con base en condiciones:
El condicional if permite ejecutar un bloque de código si se cumple una condición. Si la condición evaluada es verdadera, el código dentro del bloque if se ejecutará. Aquí tienes un ejemplo:

```php
$edad = 25;

if ($edad >= 18) {
    echo "Eres mayor de edad. Puedes ingresar.";
}
```

En este ejemplo, se evalúa la variable `$edad` y, si es mayor o igual a 18, se imprime el mensaje "Eres mayor de edad. Puedes ingresar."

2. Utilización del condicional else para ejecutar un bloque de código alternativo cuando la condición no se cumple:
El condicional else se utiliza junto con if para ejecutar un bloque de código alternativo cuando la condición evaluada es falsa. Aquí tienes un ejemplo:

```php
$edad = 15;

if ($edad >= 18) {
    echo "Eres mayor de edad. Puedes ingresar.";
} else {
    echo "Eres menor de edad. No puedes ingresar.";
}
```

En este ejemplo, si la variable `$edad` es menor que 18, se imprimirá el mensaje "Eres menor de edad. No puedes ingresar."

3. Implementación del condicional `switch` para simplificar la toma de decisiones múltiples:
El condicional switch se utiliza para simplificar la toma de decisiones cuando hay múltiples casos posibles. Aquí tienes un ejemplo:

```php
$diaSemana = "viernes";

switch ($diaSemana) {
    case "lunes":
        echo "Hoy es lunes. Ánimo, comienza la semana.";
        break;
    case "martes":
    case "miércoles":
    case "jueves":
        echo "Hoy es un día laboral. Sigue adelante.";
        break;
    case "viernes":
        echo "¡Es viernes! ¡Fin de semana pronto!";
        break;
    default:
        echo "Es un día desconocido.";
}
```

En este ejemplo, según el valor de la variable `$diaSemana`, se imprimirá un mensaje correspondiente al día de la semana.

Estos ejemplos muestran cómo utilizar las estructuras de control if, else y switch en PHP para tomar decisiones basadas en condiciones.