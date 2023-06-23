Ejemplos de uso y ejemplos de código para la inclusión de archivos y la reutilización de código en PHP:

1. Importación de archivos externos utilizando include y require:
   - La instrucción `include` se utiliza para importar y ejecutar un archivo PHP en el punto donde se coloca. Si el archivo no se encuentra, se generará una advertencia pero el script continuará su ejecución.
   - La instrucción `require` tiene el mismo propósito que `include`, pero si el archivo no se encuentra, se generará un error fatal y la ejecución del script se detendrá.

Ejemplo de uso:
```php
// Importar archivo externo usando include
include 'funciones.php';

// Importar archivo externo usando require
require 'clase.php';
```

2. Creación de archivos de funciones y clases para organizar y reutilizar código:
   - Puedes crear archivos separados que contengan funciones o clases para organizar y reutilizar código en diferentes partes de tu aplicación.
   - Las funciones y clases definidas en estos archivos pueden ser utilizadas en otros scripts PHP mediante la inclusión del archivo correspondiente.

Ejemplo de uso:
Archivo `funciones.php`:
```php
<?php
// Definición de una función en el archivo funciones.php
function saludar() {
    echo "¡Hola desde funciones.php!";
}
?>
```

Archivo `script.php`:
```php
<?php
// Incluir el archivo funciones.php
include 'funciones.php';

// Llamar a la función definida en funciones.php
saludar(); // Imprimirá "¡Hola desde funciones.php!"
?>
```

3. Utilización de herencia y composición para reutilizar código en la programación orientada a objetos:
   - En la programación orientada a objetos, puedes utilizar la herencia para crear una clase que herede propiedades y métodos de una clase base.
   - La composición te permite crear una clase que contiene instancias de otras clases para reutilizar funcionalidades.

Ejemplo de uso (herencia):
```php
class Animal {
    protected $nombre;

    public function __construct($nombre) {
        $this->nombre = $nombre;
    }

    public function comer() {
        echo $this->nombre . " está comiendo.";
    }
}

class Perro extends Animal {
    public function ladrar() {
        echo $this->nombre . " está ladrando.";
    }
}

$perro = new Perro("Fido");
$perro->comer(); // Imprimirá "Fido está comiendo."
$perro->ladrar(); // Imprimirá "Fido está ladrando."
```

Ejemplo de uso (composición):
```php
class Motor {
    public function encender() {
        echo "El motor se ha encendido.";
    }
}

class Automovil {
    private $motor;

    public function __construct() {
        $this->motor = new Motor();
    }

    public function encenderMotor() {
        $this->motor->encender();
    }
}

$auto = new Automovil();
$auto->encenderMotor(); // Imprimirá "El motor se ha encendido."
```

<font color="#ffc000">En resumen</font>, puedes utilizar la inclusión de archivos para importar código de otros archivos PHP, ya sean funciones, clases o cualquier otro tipo de código. Esto te permite organizar y reutilizar código de manera efectiva. Además, en la programación orientada a objetos, la herencia y la composición son herramientas poderosas para aprovechar la reutilización de código.