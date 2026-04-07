

# Anexo: Mecánica elemental usando Python

## Descripción general

Este anexo introduce el uso básico de Python en el contexto de la mecánica elemental, utilizando cuadernos Jupyter ejecutados en **Google Colab**. Su propósito es entregar a los estudiantes una base práctica para realizar cálculos, definir funciones simples y construir gráficos útiles para apoyar el estudio de la cinemática, la dinámica y la energía.

El enfoque de este anexo está inspirado en una serie de notebooks introductorios orientados a mecánica elemental, organizados en torno a cuatro ejes:

- uso de Python como calculadora;
- scripts y funciones;
- gráficos de datos;
- gráficos de funciones.

## Objetivo de aprendizaje

Al finalizar este anexo, el estudiante será capaz de:

- usar Google Colab para abrir, editar y ejecutar notebooks;
- escribir instrucciones básicas en Python;
- utilizar variables, operaciones aritméticas y funciones matemáticas;
- definir funciones simples para problemas de mecánica;
- generar gráficos básicos con Python;
- interpretar visualmente relaciones físicas a partir de datos y funciones.

---

## 1. ¿Qué es Google Colab?

Google Colab es un entorno en la nube que permite trabajar con notebooks tipo Jupyter sin instalar Python en el computador. En Colab se puede:

- escribir código en celdas;
- agregar texto explicativo en formato Markdown;
- ejecutar cálculos paso a paso;
- insertar gráficos y resultados en el mismo documento.

### Operaciones básicas en Colab

En un notebook existen dos tipos de celdas principales:

- **celdas de código**, para ejecutar Python;
- **celdas de texto**, para escribir explicaciones, fórmulas y comentarios.

### Atajos útiles

- **Shift + Enter**: ejecuta la celda actual y pasa a la siguiente;
- **Ctrl + Enter**: ejecuta la celda actual;
- **Alt + Enter**: ejecuta la celda y crea una nueva debajo.

---

## 2. Python como calculadora científica

Python puede utilizarse como una calculadora para operaciones frecuentes en mecánica.

### Operaciones básicas

```python
2 + 3
10 - 4
6 * 7
8 / 2
2 ** 3
```

### Uso de variables

```python
m = 5
g = 9.81
peso = m * g
peso
```

### Interpretación física

Este tipo de instrucciones permite calcular magnitudes simples como:

- peso;
- rapidez;
- energía cinética;
- trabajo mecánico;
- período;
- frecuencia.

---

## 3. Uso de la librería `math`

Para muchas aplicaciones en mecánica se necesitan funciones matemáticas especiales. Python incluye la librería `math`.

```python
import math
```

### Ejemplos básicos

```python
math.sqrt(16)
math.sin(math.pi / 2)
math.cos(0)
math.pi
```

### Aplicación en mecánica

```python
import math

v0 = 20
theta = math.radians(45)

vx0 = v0 * math.cos(theta)
vy0 = v0 * math.sin(theta)

vx0, vy0
```

Esto permite descomponer vectores y trabajar correctamente con ángulos en radianes.

---

## 4. Scripts simples en Python

Un script es una secuencia ordenada de instrucciones que Python ejecuta paso a paso.

### Ejemplo: cálculo del peso de varios cuerpos

```python
g = 9.81

m1 = 2
m2 = 5
m3 = 10

p1 = m1 * g
p2 = m2 * g
p3 = m3 * g

print(p1)
print(p2)
print(p3)
```

### Utilidad en mecánica

Los scripts son útiles para:

- automatizar cálculos repetitivos;
- comparar resultados;
- evitar errores aritméticos;
- resolver rápidamente ejercicios con varios casos.

---

## 5. Funciones en Python

Las funciones permiten reutilizar cálculos y organizar mejor el trabajo.

### Ejemplo: función para calcular energía cinética

```python
def energia_cinetica(m, v):
    return 0.5 * m * v**2
```

### Uso de la función

```python
energia_cinetica(2, 3)
energia_cinetica(5, 10)
```

### Ejemplo: función para el peso

```python
def peso(m, g=9.81):
    return m * g
```

### Importancia en física

Las funciones son especialmente útiles para representar fórmulas físicas de manera directa y clara.

---

## 6. Arreglos y datos con `numpy`

Cuando se trabaja con muchos valores, conviene usar `numpy`.

```python
import numpy as np
```

### Ejemplo: tiempos igualmente espaciados

```python
t = np.linspace(0, 5, 6)
t
```

Resultado esperado:

```python
array([0., 1., 2., 3., 4., 5.])
```

### Aplicación en cinemática

```python
x0 = 0
v0 = 4
a = 2

t = np.linspace(0, 5, 100)
x = x0 + v0*t + 0.5*a*t**2
```

Esto permite calcular la posición para muchos instantes al mismo tiempo.

---

## 7. Gráficos con `matplotlib`

Para visualizar funciones y datos en mecánica se usa frecuentemente `matplotlib`.

```python
import matplotlib.pyplot as plt
```

### Ejemplo: posición en función del tiempo

```python
import numpy as np
import matplotlib.pyplot as plt

x0 = 0
v0 = 4
a = 2

t = np.linspace(0, 5, 100)
x = x0 + v0*t + 0.5*a*t**2

plt.plot(t, x)
plt.xlabel("Tiempo [s]")
plt.ylabel("Posición [m]")
plt.title("Movimiento rectilíneo uniformemente acelerado")
plt.grid(True)
plt.show()
```

### Interpretación

Este gráfico permite visualizar cómo cambia la posición con el tiempo en un MRUA.

---

## 8. Gráficos de conjuntos de datos

Python también puede graficar datos experimentales o tablas de valores.

### Ejemplo

```python
tiempo = [0, 1, 2, 3, 4]
velocidad = [0, 2, 4, 6, 8]

plt.plot(tiempo, velocidad, marker="o")
plt.xlabel("Tiempo [s]")
plt.ylabel("Velocidad [m/s]")
plt.title("Velocidad en función del tiempo")
plt.grid(True)
plt.show()
```

### Utilidad en el curso

Esto sirve para:

- graficar resultados experimentales;
- comparar teoría y datos;
- identificar tendencias;
- interpretar pendientes y áreas.

---

## 9. Gráficos de funciones en mecánica

Un uso muy valioso de Python es graficar funciones físicas.

### Ejemplo: tiro parabólico

```python
import numpy as np
import matplotlib.pyplot as plt
import math

g = 9.81
v0 = 20
theta = math.radians(45)

t = np.linspace(0, 3, 200)
x = v0 * math.cos(theta) * t
y = v0 * math.sin(theta) * t - 0.5 * g * t**2

plt.plot(x, y)
plt.xlabel("x [m]")
plt.ylabel("y [m]")
plt.title("Trayectoria de un proyectil")
plt.grid(True)
plt.show()
```

### Interpretación

Este tipo de gráfico permite conectar directamente las ecuaciones del movimiento con la forma de la trayectoria.

---

## 10. Buenas prácticas para estudiantes

Cuando trabajes en Colab, se recomienda:

- comentar el código;
- usar nombres de variables claros;
- incluir unidades en los gráficos;
- probar primero ejemplos simples;
- revisar si los resultados tienen sentido físico;
- separar el cálculo, el gráfico y la interpretación.

---

## 11. Aplicaciones sugeridas al curso

Este anexo puede usarse para apoyar contenidos como:

- conversiones de unidades;
- vectores y descomposición;
- cinemática 1D;
- tiro parabólico;
- movimiento circular;
- leyes de Newton;
- energía mecánica;
- momentum lineal.

---

## Conceptos clave

- Google Colab
- notebook
- celda de código
- celda Markdown
- variable
- script
- función
- `math`
- `numpy`
- `matplotlib`
- gráfico
- visualización de datos