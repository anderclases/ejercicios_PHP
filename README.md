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

Fuentes: 
- https://vaidrollteam.blogspot.com/2023/10/20-ejercicios-basicos-de-php-1.html#google_vignette
- https://vaidrollteam.blogspot.com/2023/11/20-ejercicios-basicos-de-php-2.html#google_vignette