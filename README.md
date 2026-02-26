# ejercicios_PHP
Ejercicios para practicar PHP desde principiantes hasta acabar con un nivel avanzado


## Ejercicio 1
Crea un programa que imprima en pantalla la siguiente frase: Hola mundo estoy aprendiendo PHP.

```php
<?php
echo "Hola mundo estoy aprendiendo PHP.";
?>
```


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

## Ejercicio 5

```php
```

Fuentes: 
- https://vaidrollteam.blogspot.com/2023/10/20-ejercicios-basicos-de-php-1.html#google_vignette
- https://vaidrollteam.blogspot.com/2023/11/20-ejercicios-basicos-de-php-2.html#google_vignette