# Unidad 8: Estática del sólido rígido

## Descripción general

En esta unidad se estudia el equilibrio de cuerpos rígidos. A diferencia del análisis de una partícula, aquí interesa no solo la traslación del cuerpo, sino también su posible rotación. Para ello se introduce el concepto de **torque** o **momento de una fuerza**, que mide la tendencia de una fuerza a producir un giro alrededor de un punto o eje.

Se establecerán las condiciones necesarias para que un sólido rígido permanezca en equilibrio estático.

## Objetivo de aprendizaje

Al finalizar esta unidad, el estudiante será capaz de:

- comprender el concepto de torque y su significado físico;
- calcular el torque de una fuerza respecto de un punto o eje;
- aplicar la convención de signos para el sentido de rotación;
- identificar las condiciones de equilibrio estático;
- resolver problemas simples de barras y cuerpos rígidos en equilibrio.

---

## 1. Introducción a la estática del sólido rígido

La estática es la parte de la mecánica que estudia las condiciones bajo las cuales un cuerpo permanece en reposo.

Cuando se trata de un sólido rígido, no basta con exigir que la fuerza neta sea cero. También es necesario que no exista tendencia a rotar.

Por ello, en el estudio del equilibrio de un cuerpo rígido intervienen dos condiciones:

- equilibrio traslacional;
- equilibrio rotacional.

---

## 2. Sólido rígido

Un sólido rígido es un modelo ideal de cuerpo cuyas partículas mantienen distancias fijas entre sí, aun cuando actúen fuerzas externas.

Aunque en la realidad todo cuerpo puede deformarse, este modelo es muy útil para estudiar:

- barras;
- vigas;
- balanzas;
- estructuras simples;
- cuerpos en equilibrio.

---

## 3. Torque o momento de una fuerza

El torque mide la tendencia de una fuerza a producir una rotación alrededor de un punto o eje.

En forma vectorial se define como:

$$
\vec{\tau} = \vec{r} \times \vec{F}
$$

donde:

- $\vec{r}$ es el vector posición desde el eje o punto de giro hasta el punto de aplicación de la fuerza;
- $\vec{F}$ es la fuerza aplicada.

### Magnitud del torque

La magnitud del torque se calcula como:

$$
\tau = rF\sin\theta
$$

donde:

- $r$ es la distancia desde el eje al punto de aplicación;
- $F$ es la magnitud de la fuerza;
- $\theta$ es el ángulo entre $\vec{r}$ y $\vec{F}$.

### Unidad de medida

La unidad del torque en el Sistema Internacional es:

$$
\text{N}\cdot\text{m}
$$

---

## 4. Interpretación física del torque

El torque depende de tres factores:

- la magnitud de la fuerza;
- la distancia al eje de rotación;
- el ángulo con que actúa la fuerza.

### Consecuencias

- una fuerza más grande produce mayor tendencia al giro;
- una fuerza aplicada más lejos del eje produce mayor torque;
- si la fuerza actúa en la misma dirección de $\vec{r}$, el torque es cero.

Esto explica por qué resulta más fácil abrir una puerta empujando lejos de las bisagras que cerca de ellas.

---

## 5. Brazo de palanca

En muchos problemas, el torque puede calcularse usando el **brazo de palanca**, que es la distancia perpendicular desde el eje de rotación hasta la línea de acción de la fuerza.

Entonces:

$$
\tau = Fd_\perp
$$

donde $d_\perp$ es el brazo de palanca.

Esta forma es equivalente a la expresión:

$$
\tau = rF\sin\theta
$$

y muchas veces resulta más intuitiva.

---

## 6. Convención de signos para el torque

Para trabajar en dos dimensiones, se adopta una convención de signos:

- si la fuerza tiende a producir una rotación **antihoraria**, el torque es **positivo**;
- si la fuerza tiende a producir una rotación **horaria**, el torque es **negativo**.

Esta convención permite sumar algebraicamente los torques en problemas planos.

---

## 7. Torque nulo

El torque es cero en cualquiera de los siguientes casos:

### a) La fuerza es cero

$$
F = 0
$$

### b) La distancia al eje es cero

$$
r = 0
$$

es decir, la fuerza se aplica exactamente sobre el eje de rotación.

### c) La fuerza y el vector posición son paralelos

$$
\theta = 0^\circ \quad \text{o} \quad \theta = 180^\circ
$$

entonces:

$$
\sin\theta = 0
$$

y por tanto:

$$
\tau = 0
$$

---

## 8. Equilibrio estático

Un cuerpo rígido está en equilibrio estático cuando permanece en reposo sin trasladarse ni rotar.

Para que esto ocurra, deben cumplirse simultáneamente dos condiciones.

### Condición 1: equilibrio traslacional

La suma de todas las fuerzas que actúan sobre el cuerpo debe ser cero:

$$
\sum \vec{F} = 0
$$

Esto garantiza que no haya aceleración lineal.

### Condición 2: equilibrio rotacional

La suma de todos los torques respecto de cualquier punto debe ser cero:

$$
\sum \tau = 0
$$

Esto garantiza que no haya aceleración angular.

---

## 9. Equilibrio traslacional en componentes

En problemas bidimensionales, la condición de equilibrio traslacional suele escribirse en componentes:

$$
\sum F_x = 0
$$

$$
\sum F_y = 0
$$

Estas ecuaciones permiten analizar las fuerzas horizontales y verticales por separado.

---

## 10. Equilibrio rotacional

La condición de equilibrio rotacional se expresa como:

$$
\sum \tau = 0
$$

Es importante recordar que los torques deben calcularse respecto de un mismo punto de referencia.

### Elección del punto de referencia

El punto respecto del cual se calculan torques puede elegirse de manera conveniente.

Una buena elección puede simplificar mucho el problema, por ejemplo anulando el torque de fuerzas desconocidas que pasan por ese punto.

---

## 11. Procedimiento general para resolver problemas de estática

Para resolver un problema de equilibrio estático se recomienda:

1. identificar el cuerpo rígido que se analizará;
2. construir el diagrama de cuerpo libre;
3. elegir un sistema de ejes;
4. elegir un punto de referencia para calcular torques;
5. aplicar las ecuaciones de equilibrio:
   - $\sum F_x = 0$
   - $\sum F_y = 0$
   - $\sum \tau = 0$

---

## 12. Diagrama de cuerpo libre en un sólido rígido

El diagrama de cuerpo libre de un sólido rígido debe incluir:

- todas las fuerzas externas que actúan sobre el cuerpo;
- sus puntos de aplicación;
- las distancias relevantes al eje o punto de giro.

En este tipo de problemas, no basta con indicar solo las fuerzas: también es muy importante mostrar **dónde** actúan, porque eso afecta el torque.

---

## 13. Fuerzas típicas en problemas de estática

En problemas de estática del sólido rígido suelen aparecer fuerzas como:

- peso del cuerpo;
- fuerza normal;
- tensiones;
- fuerzas aplicadas por cuerdas o soportes;
- reacciones en apoyos o pivotes.

Cada una de estas fuerzas puede contribuir al equilibrio traslacional y/o rotacional.

---

## 14. Centro de masa y peso en un cuerpo uniforme

En un cuerpo uniforme, el peso puede considerarse aplicado en el centro de masa.

Por ejemplo:

- en una barra uniforme, el peso actúa en su punto medio;
- en una placa uniforme y simétrica, actúa en el centro geométrico.

Esto es especialmente útil en problemas de barras y vigas en equilibrio.

---

## 15. Ejemplo conceptual: barra en equilibrio

Supongamos una barra horizontal apoyada en su centro y con masas colgando a distintas distancias.

Para resolver el problema se debe:

- aplicar equilibrio de fuerzas para encontrar la reacción del apoyo;
- aplicar equilibrio de torques para determinar las distancias o fuerzas faltantes.

Este tipo de ejercicio muestra que un cuerpo puede tener varias fuerzas actuando y aun así permanecer en reposo si se equilibran tanto los efectos traslacionales como los rotacionales.

---

## 16. Importancia de la distancia al eje

Dos fuerzas de igual magnitud pueden producir torques distintos si se aplican a diferentes distancias del eje.

Esto ilustra una idea central de la estática:

> no solo importa cuánto vale una fuerza, sino también dónde actúa.

Por esta razón, al estudiar sólidos rígidos no basta con sumar fuerzas como en el caso de una partícula.

---

## 17. Aplicaciones típicas de la estática

La estática del sólido rígido es fundamental para estudiar:

- balanzas;
- barras apoyadas;
- vigas;
- escaleras;
- estructuras simples;
- mecanismos en equilibrio;
- distribución de cargas.

Es una base importante para cursos posteriores de mecánica, resistencia de materiales y estructuras.

---

## 18. Síntesis de la unidad

En esta unidad se introdujo el concepto de torque como medida de la tendencia de una fuerza a producir rotación.

Se estudiaron:

- la definición vectorial y escalar del torque;
- la convención de signos;
- el equilibrio traslacional;
- el equilibrio rotacional;
- las condiciones de equilibrio estático de un sólido rígido.

Estos contenidos permiten analizar cuerpos en reposo sometidos a varias fuerzas aplicadas en diferentes puntos.

---

## Conceptos clave

- estática
- sólido rígido
- torque
- momento de una fuerza
- brazo de palanca
- convención de signos
- equilibrio traslacional
- equilibrio rotacional
- equilibrio estático
- centro de masa
- diagrama de cuerpo libre

---

## Fórmulas clave

$$
\vec{\tau} = \vec{r} \times \vec{F}
$$

$$
\tau = rF\sin\theta
$$

$$
\tau = Fd_\perp
$$

$$
\sum \vec{F} = 0
$$

$$
\sum F_x = 0
$$

$$
\sum F_y = 0
$$

$$
\sum \tau = 0
$$

## Guía asociada

- **Guía 8**: Estática del sólido rígido