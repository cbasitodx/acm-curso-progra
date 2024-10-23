---
theme: default
colorSchema: 'dark'
background: https://images.unsplash.com/photo-1615869442320-fd02a129c77c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1334&q=80
highlighter: shiki
class: text-left
lineNumbers: true
info: |
  ## Introducción a Programación I (2024)
  Presentación del curso de programación I de ACM UPM 2024
drawings:
  persist: false
transition: slide-left
fonts:
    sans: Jost
    mono: mononoki, Source Code Pro
    local: mononoki
author: Borja Martinena & Sebastián Conde
---

## [ACM]
# **Introdución a la programación**

¿Qué significa programar y cómo hacerlo bien?

Borja Martinena & Sebastián Conde

<style>
    h1 {
      background-image: linear-gradient(to right bottom, #d48d8d, #de94a1, #e69db7, #e9a7ce, #e9b3e4);
      background-size: 100%;
      -webkit-background-clip: text;
      -moz-background-clip: text;
      -webkit-text-fill-color: transparent;
      -moz-text-fill-color: transparent;
  padding-bottom: 1rem;
    }
</style>
<!--
Introduccíon:
- ¿Qué es ACM?
- ¿Quien soy yo?
- ¿Qué vamos a dar en el curso?
-->
---
layout: center
class: text-center
---

# Material

<br>

https://github.com/aafrecct/acm-curso-progra

<br>

https://www.programiz.com/java-programming/online-compiler/

<br>
---

# **Índice**

<v-clicks>

1. **Elementos básicos de la programación**
    - Números
    - Strings
    - Condiciones
    - Bucles
    - Colecciones
    - Funciones
    - Tipos
    - Null
    - Errores y excepciones

</v-clicks>

---

# **Índice**

<v-clicks>

2. **Java** 
    - Estructura básica del código
    - Tipos
    - Control de flujo
    - Bucles
    - Funciones

</v-clicks>

---
layout: section
---

### PARTE 1
# **Aprendamos a programar**

---
layout: quote
---

### Números

```java
int numero_naranjas = 2000;
int nota_programacion_1 = 10;
```
<span class="lang">java</span>

---
layout: quote
---

### Números

```java {all|1|2|3}
short a = 32767;              // 2 bytes
int b = 2147483647;           // 4 bytes 
long c = 9223372036854775807; // 8 bytes
```
<span class="lang">java</span>

---
layout: quote
---

### Números

```java
int numero = 129;
System.out.println(numero);
```
<span class="lang">java</span>

<br>

<v-click>

```
129
```

</v-click>

---
layout: quote
---

### Números

```java
int a = 32;
int b = 8;

// Prueba los siguientes operadores: + - * / mod
int suma = a + b;
int resta = a - b;
int mult = a * b;
int div = a / b; // NO redondea! Trunca
int mod = a % mod;

System.out.println(suma);
System.out.println(resta);
System.out.println(mult);
System.out.println(div);
System.out.println(mod);
```
<span class="lang">java</span>

<br>

<v-click>

```
40, 24, 256, 4, 0
```

</v-click>

---
layout: quote
---

### Strings

```java
String saludo = "hola mundo";
```
<span class="lang">java</span>

---
layout: quote
---

### Strings

<div class="overflow-scroll ">

|ASCII            | Letra representada |
|:---------------:|:------------------:|
| 104             | h                  |
| 111             | o                  |
| 108             | l                  |
| 97              | a                  |
| 32              | \<espacio\>        |
| 109             | m                  |
| 117             | u                  |
| 110             | n                  |
| 100             | d                  |
| 111             | o                  |
| 0               | \<null\>           |

</div>

---
layout: quote
---

### Strings

```java
String a = "Las cadenas son secuencias de ";
String b  = "caracteres";
char c = 'a'

System.out.println(a + b); // Concatenacion de strings!
```
<span class="lang">java</span>

<br>

<v-click>

```
Las cadenas son secuencias de caracteres
```

</v-click>

---
layout: quote
---

### Booleanos

```java
boolean a = true;
boolean b = false;
```
<span class="lang">java</span>

---
layout: quote
---

### Booleanos

``` java
System.out.println(2005 > 2001);
System.out.println(9 == 11);
System.out.println("torre".contains("t"));
```
<span class="lang">java</span>

<br>

<v-click>

```
true
false
true
```

</v-click>

---
layout: quote
---

### Condiciones

```java
int numero = 1945;

if (numero % 2) == 0:
  System.out.println("PAR");
else:
  System.out.println("IMPAR");
```
<span class="lang">java</span>

<br>

<v-click>

```
IMPAR
```

</v-click>

---
layout: quote
---
### Bucles

```java
int i = 0;
int j = 1;

System.out.println(i);
System.out.println(j);

i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
i = i + j;
System.out.println(i);
j = j + i;
System.out.println(i);
...
```
<span class="lang">java</span>

---
layout: quote
---

### Bucles FOR

``` java
int i = 0;
int j = 1;
int k = 0;

System.out.println(i);
System.out.println(j);

for (int c = 3; c < 5; c++) {
	k = i + j;
	i = j;
	j = k;
	System.out.println(k);
}
```
<span class="lang">java</span>

---
layout: quote
---

### Condiciones en un bucle FOR
``` java
String miString = "hol";

int x = 1;
for (; miString.contains("a"); x++) {
	miString += "a";
}

System.out.println(x);
```

<br>

<v-click>

```
1
```

</v-click>

---
layout: quote
---

### Bucles WHILE

```java
int i = 0;
int j = 1;
int k = 0;
int c = 0;

System.out.println(x);
System.out.println(x);

while k < 10000:
	k = i + j
	i = j
	j = k
	c = c + 1
	echo c & ": " & k
```
<span class="lang">nim</span>

---
layout: quote
---

### Colecciones

```nim
var notas_progra: array[8, int] = [1, 5, 2, 5, 7, 3, 6, 7]

echo notas_progra[3]

var suma: int = 0
var media: float

for nota in notas_progra:
  suma = suma + nota

media = suma / 8
echo media
```
<span class="lang">nim</span>

---
layout: quote
---

### Funciones

```nim {all|1|2-3|5-8|10-12|14|16}
proc mcd(num1: int, num2: int): int =
  var min: int
  var mcd: int
  
  if num1 < num2:
    min = num1
  else:
    min = num2
  
  for i in 1..min:
    if num1 mod i == 0 and num2 mod i == 0:
      mcd = i
  
  return mcd

echo mcd(15, 30)
```
<span class="lang">nim</span>

---
layout: quote
---

### Null, Nil, None...

```c
char * cadena = NULL;
```
<span class="lang">c</span>

```java
String cadena = null;
```
<span class="lang">java</span>

```python
cadena = None
```
<span class="lang">python</span>

---
layout: quote
---

### Alternativas

```rust
fn checked_division(dividend: i32, divisor: i32) -> Option<i32> {
    if divisor == 0 {
        None
    } else {
        Some(dividend / divisor)
    }
}
```
<span class="lang">rust</span>

---
layout: default
---

### Errores

<br>

<v-clicks>

<div>

#### <line-md-align-left /> **Errores de compilación:**

_Algo está mal y nuestro código no compila._

</div>
<div>

#### <line-md-alert-twotone /> **Errores de ejecución:**

_Hemos hecho algo raro y mientras nuestro programa se estaba ejecutando ha aparecido un error._

</div>
<div>

#### <line-md-coffee-twotone-loop/> **Bugs**:
    
_Nuestro programa funciona... Pero_

</div>
<div>

#### <line-md-loading-loop /> **Otros (errores de seguridad, performance...)**

</div>
</v-clicks>

---
layout: quote
---

### Excepciones

```java
int a = 0;
int b = 10;
int c;

try {
	c = b / a
} catch (ArithmeticException e) {
	System.out.println("División entre 0")
	c = 0
}
```
<span class="lang">java</span>

---
layout: quote
---

## Una pequeña nota sobre paradigmas de programación.
No hace falta memorizar esto, pero puede ayudarte a entender algunas cosas.

---
layout: section
---

### PARTE 2
## Programación imperativa en
# Java

---

### Estructura del código

```java {all|1|3,6|4|8,15|11-14}
public class Estructura {
    
    static double circunferencia (int radio){
        double tau = 6.28;
        return tau * radio;
    }

    public static void main (String[] args) {
        int radio = 2;

        System.out.println("Esto es el programa principal.");
        System.out.format("La circunferencia de radio %d mide %.2f\n",
                          radio,
                          circunferencia(radio));
    }
}
```

---

### Tipos

```java {all|3|4|5|6|8|9|11|12-13|14}
public class Tipos {
    public static void main (String[] args) {
        byte  b = 1;
        short s = 1000;
        int   i = 900000;
        long  l = 9999999999;
        
        float  f = 3.141592;
        double d = 6.283184;

        System.out.format("%d + %d = %d", i, 99999, i + 99999);
        System.out.println(i++);
        System.out.println(++i);
        System.out.println(i);
    }
}
```

---

### Tipos

```java {all|3|4|6|7|9|10}
public class Tipos {
    public static void main (String[] args) {
        char letra = 'c';
        boolean check = true;

        String saludo = "Hola mundo";
        String saludoPersonal = "Hola" + "Ferrero";

        byte[] notas = {3, 4, 5, 6, 2, 3, 5, 6};
        byte[] ceros = new byte[100];
    }
}
```

---

### Condiciones

```java {all|4|6|9|all}
public class IfElse {
    public static void main (String[] args) {
        int num_alumnos = 50
        if (num_alumnos > 150) {
            System.out.println("No puedes tener tantos alumnos en una clase.");
        } else if (num_alumnos > 80) {
            System.out.println("¿Como consigues que tantos alumnos" + 
                               "vayan a tu clase?");
        } else {
            System.out.println("Debes de dar alguna optativa...");
        }
    }
}
```

---

### Condiciones

```java {all|7-8}
public class IfElse {
    public static void main (String[] args) {
        int numero_ganador_1 = 23;
        int numero_ganador_2 = 68;
        int tu_numero = 23;

        // and (&&), or (||), not (!)
        if (tu_numero == numero_ganador_1 || tu_numero == numero_ganador_2) {
            System.out.println("¡Has ganado!")
        }
    }
}
```

---

### Otras condiciones

```java {all|4|5|7|8|10|all|14}
public class MatchCase {
    public static void main (String[] args) {
        int numero = 87;
        boolean es_par = numero % 2 == 0;
        int valor_compuesto = es_par ? 100 - numero : 0;

        match (valor_compuesto) {
            case 0:
                System.out.println("No era par :(");
                break;
            case 13:
                System.out.println("Era par :)");
                break;
            default:
                System.out.println("Alguien ha cambiado el valor de `numero`")
        }
    }
}
```

---

### Bucles FOR

```java {all|3-6|8-12}
public class ForLoops {
    public static void main (String[] args) {
        // FOR
        for (int i = 0; i < 10; i++) {
            System.out.println(i);
        }

        // FOR EACH
        char[] palabra = {'A', 'C', 'M', '4', 'E', 'V', 'E', 'R'}
        for (char c : palabra) {
            System.out.print(c);
        }
    }
}
```

---

### Bucles WHILE

```java {all|3-14}
public class WhileLoops {
    public static void main (String[] args) {
        // WHILE
        int i = 293840;

        while (true) {
            System.out.println(i);
            if (i == 1) {
                break;
            } else if (i % 2 == 0) {
                i = i / 2;
            } else {
                i = 3 * i + 1;
            }
        }
    }
}
```

---

### Bucles WHILE

```java {all|3-6|8-11}
public class WhileLoops {
    public static void main (String[] args) {
        hacer_algo();
        while (condición) {
            hacer_algo();
        }

        // DO WHILE
        do {
            hacer_algo();
        } while (condición)
    }
}
```

---

### Procedimientos

```java {all|3-6|8-11}
public class WhileLoops {

    void hacer_algo () {
        Thread.sleep(1000);
    }

    public static void main (String[] args) {
        hacer_algo();
    }
}
```

---
layout: section
---

# FIN
