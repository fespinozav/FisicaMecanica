# Modelacion numerica en mecanica

La mecanica clasica no se limita a resolver ecuaciones de forma analitica. Muchos sistemas fisicos exigen aproximaciones numericas para explorar trayectorias, verificar conservacion de energia o comparar modelos ideales con situaciones mas realistas.

## Objetivos de aprendizaje

- Comprender por que aparecen los metodos numericos en problemas mecanicos.
- Aproximar derivadas e integrales con esquemas discretos simples.
- Resolver ecuaciones de movimiento con algoritmos elementales.
- Evaluar estabilidad, error y conservacion en simulaciones.

## De la formulacion continua a la discretizacion

Cuando una variable depende del tiempo, las derivadas pueden aproximarse con incrementos finitos:

```{math}
\frac{dx}{dt} \approx \frac{x_{i+1}-x_i}{\Delta t}
```

```{math}
\frac{d^2x}{dt^2} \approx \frac{x_{i+1}-2x_i+x_{i-1}}{\Delta t^2}
```

La idea central consiste en reemplazar un problema continuo por una secuencia ordenada de pasos pequeños.

## Integracion numerica

Para estimar areas o trabajo acumulado se usan reglas como:

```{math}
\int_a^b f(x)\,dx \approx \sum_i \frac{f(x_i)+f(x_{i+1})}{2}\Delta x
```

Esta expresion corresponde a la regla del trapecio. Cuando la funcion es suave, la regla de Simpson mejora la precision usando parabolas locales.

## Algoritmos frecuentes en mecanica

### Euler

```{math}
v_{i+1}=v_i+a_i\Delta t, \qquad x_{i+1}=x_i+v_i\Delta t
```

Es simple de implementar, pero puede acumular error con rapidez.

### Euler-Cromer

```{math}
v_{i+1}=v_i+a_i\Delta t, \qquad x_{i+1}=x_i+v_{i+1}\Delta t
```

Suele comportarse mejor en oscilaciones y sistemas donde interesa controlar la energia.

### Velocity Verlet

```{math}
x_{i+1}=x_i+v_i\Delta t+\frac{1}{2}a_i\Delta t^2
```

```{math}
v_{i+1}=v_i+\frac{1}{2}(a_i+a_{i+1})\Delta t
```

Es muy usado en problemas orbitales y oscilatorios porque combina simplicidad y buena conservacion energetica.

## Que conviene vigilar en una simulacion

- El tamano del paso temporal `\Delta t`.
- La propagacion del error redondeo-truncamiento.
- La conservacion de magnitudes como energia y momentum.
- La sensibilidad a las condiciones iniciales.
- La interpretacion fisica del resultado y no solo la grafica final.

## Situaciones donde esta pagina resulta util

1. Caida de un cuerpo con rozamiento.
1. Oscilaciones donde no se dispone de una solucion cerrada sencilla.
1. Problemas de dos cuerpos y orbitas.
1. Verificacion numerica del teorema trabajo-energia.

## Recomendaciones de trabajo

- Comparar siempre el resultado numerico con un caso analitico sencillo.
- Graficar posicion, velocidad, aceleracion y energia cuando sea posible.
- Justificar la eleccion del algoritmo segun el problema fisico.
- Describir de manera explicita los supuestos del modelo.
