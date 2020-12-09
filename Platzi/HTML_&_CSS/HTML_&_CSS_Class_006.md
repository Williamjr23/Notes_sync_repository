Reto 1 Organiza el siguiente bloque de código de forma semántica

> Reto realizado en los archivos:
> * Ejercicio_004_reto.html
> * Ejercicio_004_resuelto.html

### Ejercicio_004_reto.html:
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reto 1: Organiza de forma semántica</title>
</head>
<body>
    <div>
        Platzi-video
        <ul>
            <div>Cuenta</div>
            <div>Cerrar Sesión</div>
        </ul>
    </div>

    <div>Sección principal</div>

    <div>
        <div>Contáctanos</div>
        <div>Política de privacidad</div>
        <div>Términos y condiciones</div>
    </div>
</body>
</html>
```

### Ejercicio_004_resuelto.html:
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reto 1: Organiza de forma semántica</title>
</head>
<body>
    <header>
        <h1>Platzi-video</h1>
        <ul>
            <li><button onclick="">Cuenta</button></li>
            <br>
            <li><button onclick="">Cerrar sesión</button></li>
        </ul>
    </header>
    <section>Sección principal</section>
    <footer>
        <ul>
        <li><a href="platzi.com">Contáctanos</a></li>
        <li><a href="platzi.com">Política de privacidad</a></li>
        <li><a href="platzi.com">Términos y condiciones</a></li>
        </ul>
    </footer>
</body>
</html>
```

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reto 1: Organiza de forma semántica</title>
</head>
<body>
    <header>
        <h1>Platzi-video</h1>
        <ul>
            <li><button onclick="">Cuenta</button></li>
            <br>
            <li><button onclick="">Cerrar sesión</button></li>
        </ul>
    </header>
    <section>Sección principal</section>
    <footer>
        <ul>
        <li><a href="www.platzi.com">Contáctanos</a></li>
        <li><a href="www.platzi.com">Política de privacidad</a></li>
        <li><a href="www.platzi.com">Términos y condiciones</a></li>
        </ul>
    </footer>
</body>
</html>