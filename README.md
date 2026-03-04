# ejercicios_PHP
Ejercicios para practicar PHP desde principiantes hasta acabar con un nivel avanzado

Cada una de las páginas que hagamos tienen que tener como <title> el número de ejercicio.


## Ejercicio 1
Crea un programa que imprima en pantalla la siguiente frase: Hola mundo estoy aprendiendo PHP.

```php
<?php
echo "Hola mundo estoy aprendiendo PHP.";
?>
```

### Modificaciones: 
Modifica el código para que haya una variable y para que el echo la imprima, el texto de la variable que se imprime tiene que ser en negrita.


## Ejercicio 2
Crea un programa que pida al usuario su nombre y lo imprima en pantalla.
```php
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <form action="" method="get">
        <input type="text" name="nombre" placeholder="Introduce tu nombre">
        <input type="submit" value="Enviar">
    </form>

    <?php
    if (isset($_GET["nombre"])) {
        $nombre = $_GET["nombre"];
        echo "Hola, " . $nombre . "!";
    }
    ?>
</body>
</html>
```

### Modificaciones: 
Haz que el formulario pida también el apellido cambia la forma de comunicación a POST


## Ejercicio 3 

```php
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <form action="" method="get">
        <input type="number" name="numero1" placeholder="Introduce el primer número">
        <input type="number" name="numero2" placeholder="Introduce el segundo número">
        <input type="submit" value="Enviar">
    </form>

    <?php
    if (isset($_GET["numero1"]) && isset($_GET["numero2"])) {
        $numero1 = $_GET["numero1"];
        $numero2 = $_GET["numero2"];
        $suma = $numero1 + $numero2;
        echo "La suma de los números es " . $suma;
    }
    ?>
</body>
</html>
```

### Modificaciones: 
Haz que se pueda meter un tercer número, meter ese número es opcional (La web tiene que funcionar este o no informado), este en vez de sumar resta al cáculo.

## Ejercicio 4

```php
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <form action="" method="get">
        <input type="number" name="numero" placeholder="Introduce un número">
        <input type="submit" value="Enviar">
    </form>

    <?php
    if (isset($_GET["numero"])) {
        $numero = $_GET["numero"];
        if ($numero % 2 == 0) {
            echo "El número es par";
        } else {
            echo "El número es impar";
        }
    }
    ?>
</body>
</html>
```

### Modificaciones: 
- Haz que el texto que informa que es **par** sea **verde**.
- El texto que informa que es **impar** tiene que ser **rojo**.


## Ejercicio 5

Crea un programa que imprima el día de la semana al seleccionar una fecha.

```php
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <form action="" method="get">
        <input type="date" name="fecha" placeholder="Introduce una fecha">
        <input type="submit" value="Enviar">
    </form>

    <?php
    if (isset($_GET["fecha"])) {
        $fecha = $_GET["fecha"];
		setlocale(LC_TIME, "spanish");
		$dia = strftime("%A", strtotime($fecha));
        echo "El día de la semana es " . $dia;
    }
    ?>
</body>
</html>
```
### Modificaciones: 
Analiza las funciones y explica que hace cada una de ellas:
- `setlocale(LC_TIME, "spanish")` 
- `strftime("%A", strtotime($fecha))`.

Además de mostrar el día de la semana muestra el día del mes.


## Ejercicio X

Siguiente....

```php
```
### Modificaciones: 
texto...

Fuentes: 
- https://vaidrollteam.blogspot.com/2023/10/20-ejercicios-basicos-de-php-1.html#google_vignette
- https://vaidrollteam.blogspot.com/2023/11/20-ejercicios-basicos-de-php-2.html#google_vignette