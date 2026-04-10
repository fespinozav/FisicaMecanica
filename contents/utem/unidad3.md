# Unidad 3: Cinemática bidimensional de la partícula

## Descripción general

En esta unidad se estudia el movimiento de una partícula en dos dimensiones. A diferencia de la cinemática en una dimensión, aquí la posición, la velocidad y la aceleración se describen mediante componentes en ejes perpendiculares, lo que permite analizar trayectorias en el plano.

Se abordarán dos casos fundamentales:

- El movimiento parabólico;
- El movimiento circunferencial.

## Objetivo de aprendizaje

Al finalizar esta unidad, el estudiante será capaz de:

- describir el movimiento de una partícula en el plano usando componentes cartesianas;
- aplicar ecuaciones cinemáticas en dos dimensiones;
- analizar el movimiento parabólico como combinación de MRU y MRUA;
- identificar magnitudes angulares en el movimiento circunferencial;
- relacionar rapidez angular, rapidez tangencial y aceleraciones asociadas al movimiento circular.

---

## 1. Introducción a la cinemática en dos dimensiones

La cinemática bidimensional estudia el movimiento de un cuerpo cuya trayectoria ocurre en un plano.

En este caso, la posición de la partícula se expresa mediante dos coordenadas:

- $x(t)$, posición horizontal;
- $y(t)$, posición vertical.

La descripción del movimiento se hace separando el análisis en cada eje.

---

## 2. Ecuaciones de movimiento en dos dimensiones

Si la partícula tiene aceleraciones constantes $a_x$ y $a_y$, las ecuaciones de movimiento son:

### Eje $x$

$$
x(t) = x_i + v_{x,i}(t-t_i) + \frac{1}{2}a_x(t-t_i)^2
$$

$$
v_x(t) = v_{x,i} + a_x(t-t_i)
$$

$$
v_x^2(t) = v_{x,i}^2 + 2a_x(x-x_i)
$$

### Eje $y$

$$
y(t) = y_i + v_{y,i}(t-t_i) + \frac{1}{2}a_y(t-t_i)^2
$$

$$
v_y(t) = v_{y,i} + a_y(t-t_i)
$$

$$
v_y^2(t) = v_{y,i}^2 + 2a_y(y-y_i)
$$

En la mayoría de los problemas introductorios se toma:

$$
t_i = 0
$$

por lo que las ecuaciones se simplifican.

---

## 3. Interpretación física

La gran ventaja del tratamiento bidimensional es que el movimiento puede descomponerse en dos movimientos independientes:

- uno en el eje horizontal;
- otro en el eje vertical.

Esto permite resolver problemas complejos usando herramientas conocidas de cinemática en una dimensión.

---

## 4. Movimiento parabólico

El movimiento parabólico es un caso particular de movimiento en dos dimensiones.

Se produce cuando un cuerpo es lanzado con una velocidad inicial que forma un ángulo con la horizontal y luego queda sometido solamente a la aceleración de gravedad.

### Consideraciones del modelo

Para estudiar este movimiento se asume que:

- la fricción del aire es despreciable;
- la aceleración de gravedad es constante;
- el movimiento ocurre en un plano;
- la trayectoria es parabólica.

Además:

- el tiempo total en el aire se llama **tiempo de vuelo**;
- la distancia horizontal recorrida se llama **alcance**;
- el punto más alto de la trayectoria corresponde a la **altura máxima**.

---

## 5. Descomposición de la velocidad inicial

Si un proyectil es lanzado con rapidez inicial $v_0$ y ángulo $\theta$ respecto de la horizontal, entonces sus componentes iniciales son:

$$
v_{x,0} = v_0 \cos\theta
$$

$$
v_{y,0} = v_0 \sin\theta
$$

Esto permite estudiar el movimiento por separado en cada eje.

---

## 6. Ecuaciones del movimiento parabólico

### En el eje horizontal

En el eje $x$ no hay aceleración:

$$
a_x = 0
$$

Por tanto, el movimiento horizontal es un **MRU**:

$$
x(t) = x_0 + v_{x,0}t
$$

$$
v_x(t) = v_{x,0}
$$

### En el eje vertical

En el eje $y$ la aceleración es constante e igual a la gravedad:

$$
a_y = -g
$$

Por tanto, el movimiento vertical es un **MRUA**:

$$
y(t) = y_0 + v_{y,0}t - \frac{1}{2}gt^2
$$

$$
v_y(t) = v_{y,0} - gt
$$

$$
v_y^2(t) = v_{y,0}^2 - 2g(y-y_0)
$$

---

## 7. Magnitudes importantes en el movimiento parabólico

### Tiempo de vuelo

Corresponde al tiempo total que el proyectil permanece en el aire.

### Altura máxima

Se alcanza cuando la velocidad vertical se anula:

$$
v_y = 0
$$

### Alcance horizontal

Es la distancia total recorrida sobre el eje horizontal durante el tiempo de vuelo.

### Alcance máximo

En el modelo ideal, el alcance horizontal es máximo cuando el ángulo de lanzamiento es:

$$
\theta = 45^\circ
$$

---

## 8. Velocidad en cualquier punto de la trayectoria

La velocidad total del proyectil en un instante cualquiera tiene dos componentes:

$$
\vec{v}(t) = v_x(t)\hat{i} + v_y(t)\hat{j}
$$

Su magnitud se calcula como:

$$
v(t) = \sqrt{v_x^2 + v_y^2}
$$

Esto permite conocer tanto la rapidez como la dirección del movimiento en cualquier punto.

---

## 9. Trayectoria parabólica

Como el movimiento horizontal es uniforme y el vertical es uniformemente acelerado, la trayectoria que describe el proyectil es una parábola.

Esta es una de las aplicaciones más clásicas de la cinemática bidimensional.

---

## 10. Movimiento circunferencial

Otro caso importante de movimiento bidimensional es el movimiento circunferencial, en el cual la partícula describe una trayectoria circular.

En este tipo de movimiento se introducen magnitudes angulares para describir la posición y la rapidez de giro.

---

## 11. Arco recorrido y desplazamiento angular

Cuando una partícula recorre una circunferencia de radio $r$, la longitud del arco recorrido $\Delta s$ se relaciona con el desplazamiento angular $\Delta\theta$ mediante:

$$
\Delta s = r\Delta\theta
$$

Esta expresión permite conectar las magnitudes lineales con las angulares.

---

## 12. Posición angular, rapidez angular y aceleración angular

### Posición angular

La posición angular describe el ángulo barrido por la partícula:

$$
\theta(t)
$$

### Rapidez angular

La rapidez angular indica qué tan rápido cambia el ángulo con el tiempo:

$$
\omega(t) = \omega_i + \alpha(t-t_i)
$$

### Aceleración angular

La aceleración angular mide la variación de la rapidez angular:

$$
\alpha = \text{constante}
$$

Cuando es constante, las ecuaciones del movimiento angular son análogas a las del MRUA lineal.

---

## 13. Ecuaciones del movimiento angular

Si la aceleración angular es constante, entonces:

$$
\theta(t) = \theta_i + \omega_i(t-t_i) + \frac{1}{2}\alpha(t-t_i)^2
$$

$$
\omega(t) = \omega_i + \alpha(t-t_i)
$$

Estas ecuaciones son la versión angular de las ecuaciones de movimiento lineal.

---

## 14. Rapidez tangencial

La rapidez tangencial corresponde a la rapidez lineal de la partícula sobre la circunferencia y se relaciona con la rapidez angular mediante:

$$
v = r\omega
$$

Esta expresión muestra que, para un mismo radio, una mayor rapidez angular implica una mayor rapidez lineal.

---

## 15. Aceleración tangencial

Si la rapidez angular cambia en el tiempo, existe una aceleración tangencial dada por:

$$
a_t = r\alpha
$$

Esta aceleración es tangente a la trayectoria y está asociada al cambio en la magnitud de la velocidad.

---

## 16. Aceleración centrípeta

En todo movimiento circular existe una aceleración radial dirigida hacia el centro de la trayectoria, llamada **aceleración centrípeta**.

Su magnitud es:

$$
a_c = \frac{v^2}{r}
$$

o equivalentemente:

$$
a_c = r\omega^2
$$

Esta aceleración no cambia la rapidez, sino la dirección de la velocidad.

---

## 17. Período y frecuencia

### Período

El período $T$ es el tiempo que tarda la partícula en dar una vuelta completa.

### Frecuencia

La frecuencia $f$ es el número de vueltas por unidad de tiempo:

$$
f = \frac{1}{T}
$$

Además, la rapidez angular se relaciona con el período y la frecuencia mediante:

$$
\omega = \frac{2\pi}{T}
$$

$$
\omega = 2\pi f
$$

---

## 18. Movimiento circular uniforme

Cuando la partícula se mueve en una circunferencia con rapidez constante, el movimiento se llama **movimiento circular uniforme**.

En este caso:

- la rapidez angular es constante;
- la aceleración angular es cero;
- la única aceleración presente es la centrípeta.

---

## 19. Síntesis de la unidad

En esta unidad se estudió el movimiento de una partícula en el plano, separando el análisis en dos direcciones perpendiculares.

Se trabajaron dos modelos principales:

- el movimiento parabólico, donde el eje horizontal sigue MRU y el vertical sigue MRUA;
- el movimiento circunferencial, donde aparecen magnitudes angulares y aceleraciones asociadas al cambio de dirección y de rapidez.

Estos contenidos sirven de base para comprender trayectorias más complejas y preparar el estudio posterior de la dinámica.

---

## Conceptos clave

- cinemática bidimensional
- movimiento parabólico
- tiempo de vuelo
- altura máxima
- alcance
- velocidad inicial
- componentes de la velocidad
- movimiento circunferencial
- desplazamiento angular
- rapidez angular
- aceleración angular
- rapidez tangencial
- aceleración tangencial
- aceleración centrípeta
- período
- frecuencia

---

## Fórmulas clave

$$
x(t) = x_i + v_{x,i}(t-t_i) + \frac{1}{2}a_x(t-t_i)^2
$$

$$
y(t) = y_i + v_{y,i}(t-t_i) + \frac{1}{2}a_y(t-t_i)^2
$$

$$
v_{x,0} = v_0\cos\theta
$$

$$
v_{y,0} = v_0\sin\theta
$$

$$
x(t) = x_0 + v_{x,0}t
$$

$$
y(t) = y_0 + v_{y,0}t - \frac{1}{2}gt^2
$$

$$
v_y(t) = v_{y,0} - gt
$$

$$
\Delta s = r\Delta\theta
$$

$$
\theta(t) = \theta_i + \omega_i(t-t_i) + \frac{1}{2}\alpha(t-t_i)^2
$$

$$
\omega(t) = \omega_i + \alpha(t-t_i)
$$

$$
v = r\omega
$$

$$
a_t = r\alpha
$$

$$
a_c = \frac{v^2}{r}
$$

$$
a_c = r\omega^2
$$

$$
f = \frac{1}{T}
$$

$$
\omega = \frac{2\pi}{T}
$$

$$
\omega = 2\pi f
$$

## Guía asociada

- **Guía 3:** Cinemática bidimensional
