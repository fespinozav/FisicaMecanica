# Unidad 6: Dinámica de un sistema de partículas

## Descripción general

En esta unidad se extiende el estudio de la mecánica desde una sola partícula hacia un sistema formado por varias partículas. Para describir el movimiento global del sistema se introduce el concepto de **centro de masa**, que permite representar el comportamiento colectivo de todas las partículas mediante un solo punto.

También se estudia cómo se relacionan las fuerzas externas con el movimiento del sistema completo, lo que permite analizar el movimiento del centro de masa y distinguir entre fuerzas internas y externas.

## Objetivo de aprendizaje

Al finalizar esta unidad, el estudiante será capaz de:

- comprender qué es un sistema de partículas;
- calcular la posición y la velocidad del centro de masa;
- interpretar físicamente el centro de masa como descriptor del movimiento global del sistema;
- distinguir entre fuerzas internas y fuerzas externas;
- relacionar la fuerza externa neta con el movimiento del centro de masa;
- aplicar estas ideas al análisis de sistemas discretos simples.

---

## 1. Introducción a los sistemas de partículas

Hasta ahora se ha estudiado principalmente el movimiento de una partícula individual. Sin embargo, muchos sistemas físicos reales están formados por varias partículas o varios cuerpos que interactúan entre sí.

Ejemplos:

- dos masas unidas por una barra;
- un sistema planeta–satélite;
- un conjunto de cuerpos en colisión;
- un objeto extenso modelado como varias partículas.

Cuando se analiza un sistema de partículas, interesa estudiar:

- el movimiento de cada partícula;
- el movimiento global del sistema como un todo.

---

## 2. Centro de masa

El **centro de masa** es el punto en el cual puede considerarse concentrada toda la masa del sistema para describir su movimiento global.

Para un sistema de $N$ partículas, su vector posición se define como:

$$
\vec{r}_{cm} = \frac{\sum_{i=1}^{N} m_i \vec{r}_i}{\sum_{i=1}^{N} m_i}
$$

donde:

- $m_i$ es la masa de la partícula $i$;
- $\vec{r}_i$ es su vector posición.

### Interpretación física

El centro de masa describe cómo se mueve el sistema como un todo.

Si la densidad del cuerpo es uniforme, el centro de masa puede coincidir con el centro geométrico, pero en general depende de cómo esté distribuida la masa.

---

## 3. Centro de masa en una dimensión

Si las partículas están distribuidas sobre el eje $x$, la posición del centro de masa se calcula como:

$$
x_{cm} = \frac{\sum_{i=1}^{N} m_i x_i}{\sum_{i=1}^{N} m_i}
$$

### Caso de dos partículas

Para dos masas $m_1$ y $m_2$ ubicadas en posiciones $x_1$ y $x_2$:

$$
x_{cm} = \frac{m_1x_1 + m_2x_2}{m_1 + m_2}
$$

### Interpretación

- el centro de masa queda más cerca de la partícula de mayor masa;
- si ambas masas son iguales, el centro de masa queda en el punto medio.

---

## 4. Centro de masa en dos y tres dimensiones

En forma vectorial:

$$
\vec{r}_{cm} = x_{cm}\hat{i} + y_{cm}\hat{j} + z_{cm}\hat{k}
$$

con:

$$
x_{cm} = \frac{\sum m_i x_i}{\sum m_i}
\qquad
y_{cm} = \frac{\sum m_i y_i}{\sum m_i}
\qquad
z_{cm} = \frac{\sum m_i z_i}{\sum m_i}
$$

Esto permite trabajar con sistemas distribuidos en el plano o en el espacio.

---

## 5. Velocidad del centro de masa

La **velocidad del centro de masa** es la derivada temporal de su posición.

Se define como:

$$
\vec{v}_{cm} = \frac{\sum_{i=1}^{N} m_i \vec{v}_i}{\sum_{i=1}^{N} m_i}
$$

donde $\vec{v}_i$ es la velocidad de la partícula $i$.

### Interpretación física

La velocidad del centro de masa es una velocidad promedio ponderada por las masas del sistema.

Esto significa que las partículas más masivas influyen más en el movimiento global del sistema.

### En una dimensión

$$
v_{cm} = \frac{\sum_{i=1}^{N} m_i v_i}{\sum_{i=1}^{N} m_i}
$$

---

## 6. Aceleración del centro de masa

La **aceleración del centro de masa** es la derivada temporal de la velocidad del centro de masa:

$$
\vec{a}_{cm} = \frac{d\vec{v}_{cm}}{dt}
$$

o equivalentemente:

$$
\vec{a}_{cm} = \frac{\sum_{i=1}^{N} m_i \vec{a}_i}{\sum_{i=1}^{N} m_i}
$$

Esta magnitud describe cómo cambia el movimiento global del sistema.

---

## 7. Fuerzas internas y fuerzas externas

En un sistema de partículas pueden actuar dos tipos de fuerzas.

### Fuerzas internas

Son las fuerzas que las partículas del sistema se ejercen entre sí.

Ejemplos:

- tensión entre partes de un sistema;
- fuerza elástica entre masas unidas por un resorte;
- interacción gravitatoria entre cuerpos del sistema.

### Fuerzas externas

Son las fuerzas ejercidas por cuerpos que no pertenecen al sistema.

Ejemplos:

- peso total del sistema;
- fuerza normal del entorno;
- fuerza aplicada por una persona o una máquina;
- roce con una superficie externa.

---

## 8. Movimiento del centro de masa y fuerza externa neta

Uno de los resultados más importantes en dinámica de sistemas es que el movimiento del centro de masa está gobernado únicamente por la **fuerza externa neta**.

Matemáticamente:

$$
\sum \vec{F}_{ext} = M\vec{a}_{cm}
$$

donde:

- $M = \sum m_i$ es la masa total del sistema;
- $\vec{a}_{cm}$ es la aceleración del centro de masa.

### Interpretación física

Las fuerzas internas se cancelan entre sí al considerar el sistema completo, por lo que solo las fuerzas externas pueden modificar el movimiento global del sistema.

Este resultado permite tratar al sistema completo como si toda su masa estuviera concentrada en el centro de masa.

---

## 9. Momentum lineal de un sistema

El momentum lineal total de un sistema de partículas se define como la suma de los momenta individuales:

$$
\vec{P} = \sum_{i=1}^{N} m_i \vec{v}_i
$$

Como la velocidad del centro de masa es:

$$
\vec{v}_{cm} = \frac{\sum m_i \vec{v}_i}{\sum m_i}
$$

se obtiene:

$$
\vec{P} = M\vec{v}_{cm}
$$

Esto muestra que el momentum total del sistema puede calcularse usando la masa total y la velocidad del centro de masa.

---

## 10. Relación entre fuerza externa y cambio de momentum

La fuerza externa neta también puede expresarse como la variación temporal del momentum total:

$$
\sum \vec{F}_{ext} = \frac{d\vec{P}}{dt}
$$

Dado que:

$$
\vec{P} = M\vec{v}_{cm}
$$

si la masa total del sistema permanece constante:

$$
\sum \vec{F}_{ext} = M\vec{a}_{cm}
$$

Esta ecuación conecta directamente la dinámica del sistema con el movimiento de su centro de masa.

---

## 11. Sistema aislado

Un sistema se considera **aislado** si la fuerza externa neta que actúa sobre él es cero:

$$
\sum \vec{F}_{ext} = 0
$$

Entonces:

$$
\vec{a}_{cm} = 0
$$

y por tanto:

$$
\vec{v}_{cm} = \text{constante}
$$

### Interpretación

Si no actúan fuerzas externas netas, el centro de masa permanece en reposo o se mueve con velocidad constante.

---

## 12. Aplicaciones típicas del centro de masa

El concepto de centro de masa es útil para:

- describir el movimiento de cuerpos extensos;
- analizar sistemas de varias masas;
- estudiar colisiones;
- comprender trayectorias de objetos compuestos;
- separar el movimiento global del sistema del movimiento interno entre sus partes.

---

## 13. Ejemplo conceptual sencillo

Supongamos dos masas:

- $m_1 = 3\text{ kg}$ en $x_1 = 2\text{ m}$;
- $m_2 = 5\text{ kg}$ en $x_2 = 6\text{ m}$.

Entonces:

$$
x_{cm} = \frac{m_1x_1 + m_2x_2}{m_1 + m_2}
$$

$$
x_{cm} = \frac{3(2) + 5(6)}{3+5}
= \frac{6+30}{8}
= 4.5\text{ m}
$$

Esto muestra que el centro de masa queda más cerca de la masa mayor.

---

## 14. Interpretación del movimiento global

Un sistema puede tener movimientos internos complejos y, aun así, su centro de masa moverse de forma simple.

Por ejemplo:

- en una explosión, las partículas salen en distintas direcciones, pero el centro de masa sigue obedeciendo a las fuerzas externas;
- en un objeto lanzado al aire, aunque rote o cambie de orientación, su centro de masa sigue una trayectoria determinada por la fuerza de gravedad.

---

## 15. Diferencia entre movimiento interno y movimiento del centro de masa

En un sistema de partículas pueden coexistir dos tipos de movimiento:

- el movimiento del centro de masa;
- el movimiento relativo de las partículas respecto del centro de masa.

Esta separación es muy útil porque permite estudiar primero el movimiento global del sistema y luego los movimientos internos si es necesario.

---

## 16. Síntesis de la unidad

En esta unidad se introdujo el concepto de sistema de partículas y se estudió el centro de masa como herramienta para describir el movimiento global del sistema.

Se analizaron:

- la posición del centro de masa;
- la velocidad y aceleración del centro de masa;
- la diferencia entre fuerzas internas y externas;
- la relación entre fuerza externa neta y movimiento del centro de masa;
- el momentum lineal total del sistema.

Estos conceptos preparan el estudio del impulso, la conservación del momentum y el análisis de colisiones.

---

## Conceptos clave

- sistema de partículas
- centro de masa
- posición del centro de masa
- velocidad del centro de masa
- aceleración del centro de masa
- fuerzas internas
- fuerzas externas
- masa total
- momentum lineal del sistema
- sistema aislado

---

## Fórmulas clave

$$
\vec{r}_{cm} = \frac{\sum_{i=1}^{N} m_i \vec{r}_i}{\sum_{i=1}^{N} m_i}
$$

$$
x_{cm} = \frac{\sum_{i=1}^{N} m_i x_i}{\sum_{i=1}^{N} m_i}
$$

$$
\vec{v}_{cm} = \frac{\sum_{i=1}^{N} m_i \vec{v}_i}{\sum_{i=1}^{N} m_i}
$$

$$
\vec{a}_{cm} = \frac{\sum_{i=1}^{N} m_i \vec{a}_i}{\sum_{i=1}^{N} m_i}
$$

$$
\sum \vec{F}_{ext} = M\vec{a}_{cm}
$$

$$
\vec{P} = \sum_{i=1}^{N} m_i \vec{v}_i
$$

$$
\vec{P} = M\vec{v}_{cm}
$$

$$
\sum \vec{F}_{ext} = \frac{d\vec{P}}{dt}
$$

## Guía asociada

- **Guía 6**: Dinámica de un sistema de partículas