# Creación-y-uso-de-elementos-básicos-en-php

Prueva de funcionamiento de submodulos


## Bloque 1: Conceptos básicos (introducción a php)

### Variables y Condicionales

1. **Mayor de dos números**  
   Pide dos números y muestra cuál es mayor o si son iguales.

```php
<?php
    $numero1 = 8;
    $numero2 = 8;
    $respuesta = "El mayor es $numero1";
    if ($numero1 < $numero2) {
        $respuesta = "El mayor es $numero2";
    }
    if ($numero1 == $numero2) {
        $respuesta = "Los numeros son iguales";
    }
    echo $respuesta;
?>
```

2. **Edad permitida**  
   Pide la edad de una persona y muestra:  
   - `"Eres menor de edad"` si es < 18.  
   - `"Eres mayor de edad"` si es ≥ 18.  

```php
<?php
    $edad = 18;
    $respuesta = "Eres menor de edad";
    if ($edad >= 18) {
        $respuesta = "Eres mayor de edad";
    }
    echo $respuesta;
?>
```

3. **Positivo, negativo o cero**  
   Comprueba si un número almacenado en una variable es positivo, negativo o cero.  

```php
<?php
    $numero = 4;
    $respuesta = "El numero es positivo";
    if ($numero < 0) {
        $respuesta = "El numero es negativo";
    }
    if ($numero == 0) {
        $respuesta = "El numero es 0";
    }
    echo $respuesta;
?>
```

4. **Nota final**  
   Pide la nota de un alumno y muestra:  
   - `"Suspenso"` (< 5), `"Aprobado"` (5–6), `"Notable"` (7–8), `"Sobresaliente"` (9–10).  

```php
<?php
    $nota = 11;
    switch ($nota) {
        case $nota < 5:
            echo "Suspendido";
            break;
        case 5:
        case 6:
            echo "Aprobado";
            break;
        case 7:
        case 8:
            echo "Notable";
            break;
        case 9:
        case 10:
            echo "Sobresaliente";
            break;
        default:
            echo "ERROR: La nota no solo puede estar entre 0 y 10";
            break;
    }
?>
```

---

### 2️⃣ Bucles (for, while, foreach)

5. **Contar del 1 al 100**  
   Muestra los números del 1 al 100 en pantalla.

```php
<?php
    for ($i=1; $i < 101; $i++) { 
        echo $i;
        echo "<br>";
    }
?>
```

6. **Suma acumulada**  
   Calcula la suma de los números del 1 al 50 usando un bucle.  

```php
<?php
    $sumaTotal = 0;
    for ($i=0; $i < 51; $i++) {
        $sumaTotal = $sumaTotal + $i;
    }
    echo $sumaTotal;
?>
```

7. **Tabla de multiplicar**  
   Pide un número y genera su tabla de multiplicar del 1 al 10.  

```php
<?php
    $numero = 7;
    for ($i=0; $i < 11; $i++) {
        $multi = $numero*$i;
        echo "$numero x $i = $multi";
        echo "<br>";
    }
?>
```

8. **Números pares**  
   Muestra todos los números pares entre 1 y 50.  

```php
<?php

?>
```

9. **Cuenta atrás**  
   Haz un bucle que cuente de 10 a 1 y luego muestre `"¡Fin!"`.  

```php
<?php

?>
```

10. **Factorial**  
    Calcula el factorial de un número introducido (ejemplo: `5! = 120`).  

```php
<?php

?>
```

---

### 3️⃣ Combinando Condicionales y Bucles

11. **Números primos**  
    Escribe un algoritmo que muestre los números primos entre 1 y 50.  

```php
<?php

?>
```

12. **Fibonacci**  
    Genera los primeros 20 términos de la secuencia de Fibonacci.  

```php
<?php

?>
```

13. **Múltiplos de un número**  
    Pide un número `n` y muestra sus múltiplos hasta 100.  

```php
<?php

?>
```

14. **Suma de pares e impares**  
    Calcula la suma de los números pares e impares entre 1 y 100 por separado.  

```php
<?php

?>
```

15. **Adivinar número**  
    Genera un número aleatorio entre 1 y 20.  
    Pide al usuario que lo adivine y usa un bucle con condicionales para dar pistas: `"Mayor"` o `"Menor"`.  

```php
<?php

?>
```

---

### 4️⃣ Construcción de Algorítmicos

16. **Número perfecto**  
    Comprueba si un número es perfecto (la suma de sus divisores propios es igual al número).  

```php
<?php

?>
```

17. **Invertir número**  
    Escribe un algoritmo que invierta los dígitos de un número (ejemplo: `123 → 321`).  

```php
<?php

?>
```

18. **Palíndromo**  
    Comprueba si una palabra almacenada en una variable es palíndroma.  

```php
<?php

?>
```

19. **Máximo común divisor (MCD)**  
    Escribe un algoritmo que calcule el MCD de dos números.  

```php
<?php

?>
```

20. **Triángulo de asteriscos**  
    Muestra en pantalla un triángulo de altura `n` usando `*`.  
    Ejemplo con `n = 5`:  
    ```
    *
    **
    ***
    ****
    *****
    ```

```php
<?php

?>
```

---