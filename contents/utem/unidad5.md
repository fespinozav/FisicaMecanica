# Unidad 5: Trabajo y energía mecánica

## Descripción general

En esta unidad se estudia el movimiento desde un punto de vista energético. A diferencia del enfoque dinámico basado en fuerzas y aceleraciones, el enfoque energético permite analizar muchos problemas mediante magnitudes escalares, lo que simplifica notablemente su resolución.

Se introducirán los conceptos de trabajo mecánico, energía cinética, energía potencial, potencia y conservación de la energía mecánica.

```{figure} ../images/trabajo-y-energia.png
---
width: 60%
name: trabajo-y-energia
---

```

## Objetivo de aprendizaje

Al finalizar esta unidad, el estudiante será capaz de:

- interpretar el trabajo como un mecanismo de transferencia de energía.
- calcular el trabajo realizado por fuerzas constantes y por la fuerza neta.
- relacionar el trabajo neto con el cambio de energía cinética.
- comprender el significado físico de la energía potencial.
- aplicar el principio de conservación de la energía mecánica.
- resolver problemas de movimiento usando métodos energéticos.

---

## 1. Introducción al enfoque energético

El estudio de la física desde el punto de vista energético tiene una gran ventaja: muchas de las magnitudes involucradas son escalares.

Esto permite analizar el movimiento sin tener que trabajar siempre con ecuaciones vectoriales completas.

En mecánica clásica, dos formas fundamentales de energía son:

- La energía cinética.
- La energía potencial.

Ambas se relacionan mediante el trabajo mecánico.

---

## 2. Trabajo mecánico

El trabajo mecánico es una forma de transferir energía a un cuerpo mediante la acción de una fuerza durante un desplazamiento.

```{figure} ../images/trabajo_mecanico.png
---
width: 60%
name: trabajo_mecanico
---

```

Si una fuerza constante $\vec{F}$ actúa sobre un cuerpo que se desplaza una cantidad $\Delta \vec{r}$, el trabajo realizado es:

$$
W = \vec{F} * \vec{r}=F \, \Delta r \cos\theta
$$

donde:

- $F$ es la magnitud de la fuerza;
- $\Delta r$ es la magnitud del desplazamiento;
- $\theta$ es el ángulo entre la fuerza y el desplazamiento.

```{note}
- El trabajo es nulo si $r=0$ y/o la fuerza es perpendicular al desplazamiento. ej: el realizado por el peso sobre un cuerpo en una superficie horizontal
- El trabajo el positivo si la fuerza es favorable al movimiento ($cos \theta > 0$).
- El trabajo es negativo si la fuerza se opone al movimiento ($cos \theta < 0$). ej: el realizado por la fuerza de roce

```

### Unidad de medida

La unidad del trabajo en el Sistema Internacional es el **joule**:

$$
1 \text{ J} = 1 \text{ N}\cdot \text{m}
$$

---

## 3. Signo del trabajo

El signo del trabajo depende del ángulo entre la fuerza y el desplazamiento.

### Trabajo positivo

Si la fuerza tiene una componente en la misma dirección del desplazamiento:

$$
0^\circ \leq \theta < 90^\circ
$$

entonces el trabajo es positivo.

Esto significa que la energía se transfiere **desde el entorno hacia el cuerpo**.

### Trabajo negativo

Si la fuerza se opone al desplazamiento:

$$
90^\circ < \theta \leq 180^\circ
$$

entonces el trabajo es negativo.

Esto significa que la energía se transfiere **desde el cuerpo hacia el entorno**.

### Trabajo nulo

Si la fuerza es perpendicular al desplazamiento:

$$
\theta = 90^\circ
$$

entonces:

$$
W = 0
$$

En este caso, la fuerza no transfiere energía al cuerpo.

### Relación entre trabajo y producto escalar

El trabajo puede interpretarse como un producto escalar entre fuerza y desplazamiento:

$$
W = \vec{F} \cdot \Delta \vec{r}
$$

Esto explica por qué el trabajo depende de:

- la magnitud de la fuerza;
- la magnitud del desplazamiento;
- el ángulo entre ambas.

---

## 4. Trabajo de fuerzas frecuentes

### Trabajo del peso

Si el desplazamiento es horizontal y el peso es vertical, el trabajo del peso es cero porque ambas direcciones son perpendiculares.

### Trabajo de la fuerza normal

La fuerza normal también suele ser perpendicular al desplazamiento, por lo que normalmente no realiza trabajo.

### Trabajo de una tensión

Si la tensión forma un ángulo con el desplazamiento, se aplica directamente la fórmula general del trabajo.

### Trabajo del roce

La fuerza de roce generalmente se opone al movimiento, por lo que su trabajo suele ser negativo.

---

## 5. Trabajo neto

El trabajo neto es la suma de todos los trabajos realizados por las fuerzas que actúan sobre un cuerpo entre dos instantes:

$$
W_{\text{neto}} = \sum_i W_i
$$

Representa la transferencia neta de energía hacia o desde el cuerpo.

### Ejemplo: Subir un bloque por un plano inclinado rugoso (con rozamiento).


```{figure} ../images/bloque_up.png
---
width: 60%
name: bloque_que_sube
---
DCL de bloque que sube por un plano inclinado
```
$$
W_{g} = - mg \sin \theta d 
$$

$$
W_{F} = \vec{F} \vec{d} = F*d
$$

$$
W_{R} = -F_r*d = - \mu m g \cos \theta d 
$$

$$
W = Wg + W_F + W_R = \vec{R} * \vec{d} = R_T d
$$

$$
R_T = F-mg \sin \theta - \mu  mg \cos \theta
$$

---

## 6. Energía cinética

La energía cinética es la energía asociada al movimiento de un cuerpo. Siendo este un escalar con las mismas unidades que el trabajo.

Se define como:

$$
E_c = K = \frac{1}{2}mv^2
$$

donde:

- $m$ es la masa del cuerpo;
- $v$ es la rapidez del cuerpo.

### Propiedades

- es una magnitud escalar.
- siempre es positiva o nula.
- depende del cuadrado de la rapidez.

### Unidad de medida

Su unidad en el Sistema Internacional es el joule.

### Ejemplo: Energía Cinética (K)

Supongamos una partícula de masa m bajo la acción de una fuerza resultante F  que la desplaza a lo largo de una trayectoria:

![alt text](/contents/images/image-1.png)


$$
\begin{align}
W &= \int_A^B \vec{F} \cdot d\vec{r}
   = \int_A^B m\vec{a} \cdot d\vec{r}
   = \int_A^B m\vec{a} \cdot \vec{v}\, dt
   = \int_A^B m\frac{d\vec{v}}{dt} \cdot \vec{v}\, dt
   = \int_A^B m\vec{v} \cdot d\vec{v} \\
  &= \left[\frac{1}{2}m\vec{v} \cdot \vec{v}\right]_A^B
   = \left[\frac{1}{2}mv^2\right]_A^B
   = \frac{1}{2}mv_B^2 - \frac{1}{2}mv_A^2
\end{align}
$$

---

## 7. Teorema trabajo–energía cinética

Uno de los resultados más importantes de esta unidad es el teorema trabajo–energía cinética:

$$
W_{\text{neto}} = \Delta E_c
$$

donde:

$$
\Delta E_c = E_{cf} - E_{ci} = K_f - K_i
$$

Esto significa que el trabajo neto realizado sobre un cuerpo es igual al cambio de su energía cinética.

### Interpretación física

- si el trabajo neto es positivo, la energía cinética aumenta.
- si el trabajo neto es negativo, la energía cinética disminuye.
- si el trabajo neto es cero, la energía cinética permanece constante.

---

## 8. Potencia

La potencia mide la rapidez con la que se transfiere energía o se realiza trabajo.

### Potencia promedio

Se define como:

$$
P_{\text{prom}} = \frac{\Delta W}{\Delta t}
$$

donde:

- $\Delta W$ es el trabajo realizado;
- $\Delta t$ es el intervalo de tiempo.

### Unidad de medida

La unidad de potencia en el Sistema Internacional es el **watt**:

$$
1 \text{ W} = 1 \text{ J/s}
$$

### Interpretación

Una potencia alta significa que la transferencia de energía ocurre más rápidamente.

---

## 9. Energía potencial

La energía potencial es la energía asociada a la posición o configuración de un sistema.

En esta unidad se estudiarán principalmente dos formas:

- energía potencial gravitatoria.
- energía potencial elástica.


### Ejemplo: 

Supongamos la fuerza de la gravedad y calculemos el $W$ realizado *sólo por
esta fuerza* ($mg$) al mover un objeto a lo largo de dos caminos diferentes
que unan el punto inicial $A$ y el final $B$:

![alt text](/contents/images/pot_e.png)

**Camino 1:** De $A$ hasta $B$ por el plano inclinado,

$$
W_{AB} = mgd \sin \theta = mgh
$$

**Camino 2:** De $A$ hasta $B$ pasando por $C$,

$$
\left.\begin{aligned}
W_{AC} &= mgh \\
W_{CB} &= 0 \quad (\vec{F} \perp \vec{r})
\end{aligned}\right\}
\quad W_{ACB} = W_{AC} + W_{CB} = mgh
$$

Vemos que **el trabajo es el mismo**. Se puede probar que, aunque elijamos
otro camino, $W$ sólo depende de la diferencia de altura $h$ entre $A$ y $B$.

---

## 10. Energía potencial gravitatoria

Cerca de la superficie terrestre, la energía potencial gravitatoria de un cuerpo se expresa como:

![alt text](/contents/images/grav_pot.png)

$$
\vec{F} = -mg\,\hat{j}
$$

$$
\begin{align}
W_{AB} &= \int_A^B \vec{F} \cdot d\vec{r}
        = -\int_A^B mg\,\hat{j} \cdot (dx\,\hat{i} + dy\,\hat{j}) \\
       &= -\int_A^B mg\, dy
        = -(mgy_B - mgy_A)
\end{align}
$$

$$
W_{AB} = U_A - U_B \quad \Rightarrow \quad U(y) = mgy
$$

$$
\boxed{ U_g = mgy}
$$

donde:

- $m$ es la masa;
- $g$ es la aceleración de gravedad;
- $y$ es la altura respecto de un nivel de referencia.

### Cambio en la energía potencial gravitatoria

Lo relevante físicamente es el cambio de energía potencial:

$$
\Delta U_g = mg(y_f - y_i)
$$

### Interpretación

- si el cuerpo sube, su energía potencial gravitatoria aumenta;
- si baja, disminuye.

---

## 11. Energía potencial elástica

Cuando un resorte ideal se deforma, almacena energía potencial elástica.

![alt text](/contents/images/elast.png)

Se define como:

$$
U_e = \frac{1}{2}kx^2
$$

donde:

- $k$ es la constante elástica del resorte;
- $x$ es la deformación respecto a la posición de equilibrio.

### Interpretación

Tanto si el resorte se estira como si se comprime, la energía potencial elástica aumenta, porque depende de $x^2$.

---

## 12. Fuerzas conservativas y no conservativas

### Fuerzas conservativas

Son aquellas para las cuales el trabajo entre dos puntos no depende de la trayectoria seguida, sino solo de la posición inicial y final.

Ejemplos:

- fuerza gravitatoria.
- fuerza elástica del resorte.

Estas fuerzas permiten definir una energía potencial asociada.

### Fuerzas no conservativas

Son aquellas para las cuales el trabajo sí depende de la trayectoria.

Ejemplo típico:

- fuerza de roce.

Estas fuerzas suelen disipar energía mecánica en otras formas, como calor.

---

## 13. Energía mecánica

La energía mecánica de un sistema es la suma de su energía cinética y su energía potencial:

$$
E_m = K + U
$$

Dependiendo del problema, $U$ puede incluir:

- energía potencial gravitatoria
- energía potencial elástica
- o ambas.

---

## 14. Conservación de la energía mecánica

Si en un sistema solo actúan fuerzas conservativas, entonces la energía mecánica permanece constante:

$$
E_{m,i} = E_{m,f}
$$

o equivalentemente:

$$
K_i + U_i = K_f + U_f
$$

### Interpretación

La energía puede transformarse de una forma a otra:

- de potencial a cinética;
- de cinética a potencial;

pero la suma total permanece constante.

---

## 15. Cambio de energía mecánica con roce

Si actúan fuerzas no conservativas, como el roce, la energía mecánica ya no se conserva.

En ese caso:

$$
W_{\text{nc}} = \Delta E_m
$$

donde $W_{\text{nc}}$ es el trabajo realizado por fuerzas no conservativas.

### Interpretación

Cuando hay roce:

- parte de la energía mecánica se transforma en energía térmica;
- la energía mecánica final es menor que la inicial.

---

## 16. Aplicaciones típicas del método energético

El enfoque energético permite resolver con facilidad problemas como:

- caída libre
- lanzamiento vertical
- bloques sobre superficies con o sin roce
- resortes comprimidos o estirados
- planos inclinados
- sistemas con variación de altura

En muchos casos, usar energía resulta más directo que aplicar Newton en cada etapa del movimiento.

## Aplicación: ritmo cardíaco y leyes de escala

A partir del concepto de tasa metabólica y utilizando las leyes de escala
se puede calcular **cómo varía el ritmo cardíaco con el tamaño de los individuos**.

Como la energía consumida acaba disipándose en forma de calor que escapa a
través de la piel, se encuentra que $P_{\text{met}}$ (potencia metabólica) es proporcional al área
del cuerpo de un animal.

Establecemos una *hipótesis biológica* considerando que el $\text{O}_2$ necesario
para el metabolismo es proporcionado por la sangre y ésta es bombeada por el corazón.

Una $P_{\text{met}}$ elevada se producirá cuanto más grande sea el corazón y más
rápido pueda bombear. Por tanto, podemos suponer que la $P_{\text{met}}$ es
proporcional al volumen del corazón $V$ por la frecuencia de bombeo $f$
(pulsaciones por segundo),

$$
P_{\text{met}} \propto V\, f
$$

Sea $k$ el factor de escala entre dos animales semejantes, según el modelo
de semejanza geométrica ($k = L'/L$;\ $k^2 = A'/A$;\ $k^3 = V'/V$):

$$
\left.\begin{aligned}
\dfrac{P_{\text{met}}'}{P_{\text{met}}} &= k^2 \\[10pt]
\dfrac{P_{\text{met}}'}{P_{\text{met}}} &= \dfrac{V'\,f'}{V\,f} = k^3\,\dfrac{f'}{f}
\end{aligned}\right\}
\quad \Rightarrow \quad f' = \frac{1}{k}\,f
$$

Así que **el corazón de un animal mayor late más lentamente que el de uno pequeño**.

Puede comprobarse cómo el ritmo cardíaco en bebés es superior. En ratones también
se aprecia claramente. El mamífero con mayor ritmo cardíaco que existe es la musaraña.

Por ejemplo, si comparamos a seres humanos (adultos) con el mono (rhesus) con un
factor de escala entre ambos de $2.5$:

$$
f_{\text{corazón humano}} = \frac{1}{2.5}\,f_{\text{mono}} = 0.4\,f_{\text{mono}}
\qquad (\text{experimentalmente se obtiene } 0.5)
$$

---

## 17. Ejercicios de ejemplo

## Ejemplo 1 — Simple: Caída libre desde altura $h$

```{figure} ../images/caida_simple.png
---
width: 40%
name: ejemplo_1
---
```

**Situación:** Una masa $m$ se suelta desde el reposo a una altura $h$
sobre el suelo. No hay rozamiento.

**Estado inicial $A$ (en la cima):**

$$
K_A = 0, \qquad U_A = mgh, \qquad E_A = mgh
$$

**Estado final $B$ (en el suelo):**

$$
K_B = \frac{1}{2}mv_B^2, \qquad U_B = 0, \qquad E_B = \frac{1}{2}mv_B^2
$$

**Aplicando conservación de energía mecánica:**

$$
E_A = E_B \quad \Rightarrow \quad mgh = \frac{1}{2}mv_B^2
\quad \Rightarrow \quad \boxed{v_B = \sqrt{2gh}}
$$

---

## Ejemplo 2: Plano inclinado con rozamiento y potencia


```{figure} ../images/plano_simple.png
---
width: 40%
name: ejemplo_2
---
```

**Situación:** Una masa $m$ parte del reposo y desliza una distancia $d$
sobre un plano inclinado un ángulo $\theta$, con coeficiente de rozamiento
cinético $\mu_k$.

### Paso 1 — Trabajo de cada fuerza

$$
W_{\text{grav}} = mg\,d\sin\theta
$$

$$
W_{\text{roz}} = -f_k\,d = -\mu_k\,mg\cos\theta\cdot d
$$

$$
W_{\text{normal}} = 0 \qquad (\vec{N} \perp d\vec{r})
$$

### Paso 2 — Teorema trabajo-energía cinética

$$
W_{\text{total}} = \Delta K \quad \Rightarrow \quad
mg\,d\sin\theta - \mu_k\,mg\cos\theta\,d = \frac{1}{2}mv_B^2
$$

$$
\boxed{v_B^2 = 2g\,d\left(\sin\theta - \mu_k\cos\theta\right)}
$$

### Paso 3 — Balance energético con fuerzas disipativas

$$
\frac{1}{2}mv_B^2 = mgh - \Delta E_{\text{térmica}}
$$

$$
\frac{1}{2}mv_B^2 = mg\,d\sin\theta - \mu_k\,mg\cos\theta\cdot d
$$

### Paso 4 — Potencia instantánea al llegar a $B$

$$
P_{\text{grav}} = \vec{F}_{\text{grav}}\cdot\vec{v}_B = mg\sin\theta\cdot v_B
$$

$$
\boxed{P_{\text{grav}} = mg\sin\theta\sqrt{2g\,d\left(\sin\theta - \mu_k\cos\theta\right)}}
$$

---

## Ejercicio 1.2 — Trabajo de la Gravedad y Energía Cinética en Caída Libre

```{admonition} Enunciado
:class: tip

Una masa de $2.0 \ \text{kg}$ cae $400 \ \text{cm}$. ¿Cuánto trabajo fue realizado sobre la masa
por la fuerza de gravedad? Si se trata de una caída libre, es decir, si no hay otras fuerzas
que actúen sobre la masa, determine el cambio de energía cinética y la rapidez de la masa
tras caer $400 \ \text{cm}$ si partió del reposo.
```

**Datos del problema**

| Cantidad | Símbolo | Valor |
|---|---|---|
| Masa | $m$ | $2.0 \ \text{kg}$ |
| Distancia de caída | $h$ | $400 \ \text{cm} = 4.00 \ \text{m}$ |
| Velocidad inicial | $v_0$ | $0 \ \text{m/s}$ (reposo) |
| Aceleración de gravedad | $g$ | $9.8 \ \text{m/s}^2$ |

---

### Marco conceptual — Teorema Trabajo-Energía

La gravedad es una **fuerza constante** $\vec{G} = -mg\hat{j}$. Para una fuerza constante,
el trabajo depende únicamente del desplazamiento[^Malthe-Sorensen_10]:

$$W = \vec{F} \cdot \Delta\vec{r} \tag{1.2.1}$$

El **Teorema Trabajo-Energía** relaciona ese trabajo con el cambio en energía cinética:

$$W_{\text{neto}} = \Delta K = K_1 - K_0 \tag{1.2.2}$$

---

### Paso 1 — Diagrama de cuerpo libre

En caída libre, la **única** fuerza que actúa y realiza trabajo es el peso:

| Fuerza | Dirección | ¿Hace trabajo? |
|---|---|---|
| Peso $G = mg$ | $-\hat{j}$ (hacia abajo) | ✅ Sí — paralela al desplazamiento |

La fuerza normal y la fricción están **ausentes** en caída libre.

---

### Parte (a) — Trabajo realizado por la gravedad

La fuerza gravitacional actúa en la misma dirección del desplazamiento:

$$W_G = mg \cdot h \tag{1.2.3}$$

$$W_G = (2.0 \ \text{kg})(9.8 \ \text{m/s}^2)(4.00 \ \text{m})$$

$$\boxed{W_G = 78.4 \ \text{J}}$$

---

### Parte (b) — Cambio en energía cinética

En caída libre $W_{\text{neto}} = W_G$, por lo tanto:

$$\Delta K = W_{\text{neto}} = W_G \tag{1.2.4}$$

$$\boxed{\Delta K = +78.4 \ \text{J}}$$

El signo positivo indica que la masa **gana** energía cinética al descender.

---

### Parte (c) — Rapidez final

Como la masa parte del reposo, $K_0 = \frac{1}{2}mv_0^2 = 0$, entonces $\Delta K = K_1$:

$$\Delta K = \frac{1}{2}mv_1^2 \tag{1.2.5}$$

Despejando $v_1$:

$$v_1 = \sqrt{\frac{2\,\Delta K}{m}} = \sqrt{\frac{2\,W_G}{m}} \tag{1.2.6}$$

$$v_1 = \sqrt{\frac{2(78.4 \ \text{J})}{2.0 \ \text{kg}}} = \sqrt{78.4 \ \text{m}^2/\text{s}^2}$$

$$\boxed{v_1 \approx 8.85 \ \text{m/s}}$$

---

### Verificación — Cinemática independiente

$$v_1 = \sqrt{2gh} = \sqrt{2(9.8 \ \text{m/s}^2)(4.00 \ \text{m})} = \sqrt{78.4} \approx 8.85 \ \text{m/s} \checkmark$$

Ambos métodos son consistentes, confirmando la validez del Teorema Trabajo-Energía.

---

### Verificación — Análisis de casos límite

| $h \ (\text{m})$ | $W_G \ (\text{J})$ | $v_1 \ (\text{m/s})$ | Interpretación |
|---|---|---|---|
| $0$ | $0$ | $0$ | Sin caída, sin trabajo |
| $1$ | $19.6$ | $4.43$ | Caída pequeña |
| $4$ | $78.4$ | $8.85$ | **Este problema** |
| $9$ | $176.4$ | $13.3$ | $v_1$ crece como $\sqrt{h}$ |

---

### Interpretación física

La gravedad realiza un trabajo positivo de $78.4 \ \text{J}$, íntegramente convertido en
energía cinética dado que no existe ninguna fuerza disipativa. La rapidez final de
$8.85 \ \text{m/s}$ escala como $\sqrt{h}$: duplicar la altura de caída no duplica la
velocidad, sino que la multiplica por $\sqrt{2}$, consecuencia directa de la relación
cuadrática entre energía cinética y velocidad.

## Ejercicio 2.4 — Saco en Riel sin Fricción (A → B)

```{admonition} Enunciado
:class: tip

Un saco es descargado por un riel sin fricción desde el punto A como muestra la figura,
de tal forma que una persona los recibe en el punto B. Si el saco es liberado con rapidez
inicial $v_A$ a una altura $h = 5 \ \text{m}$ y llega al punto B con rapidez $10 \ \text{m/s}$,
determine el valor de $v_A$.
```

**Datos del problema**

| Cantidad | Símbolo | Valor |
|---|---|---|
| Altura inicial respecto a B | $h$ | $5 \ \text{m}$ |
| Rapidez en B (final) | $v_B$ | $10 \ \text{m/s}$ |
| Rapidez en A (inicial) | $v_A$ | ? |
| Fricción | — | nula |

---

### Marco conceptual — Conservación de Energía Mecánica

El riel es **sin fricción** y la fuerza normal es siempre perpendicular al movimiento,
por lo tanto **no realiza trabajo**. Las únicas fuerzas son conservativas (gravedad).
Se aplica conservación de energía mecánica[^Malthe-Sorensen_11]:

$$E_A = E_B \tag{2.4.1}$$

$$K_A + U_A = K_B + U_B \tag{2.4.2}$$

Tomando el punto B como referencia de energía potencial ($U_B = 0$):

$$\frac{1}{2}mv_A^2 + mgh = \frac{1}{2}mv_B^2 \tag{2.4.3}$$

---

### Paso 1 — La masa cancela

Dividiendo toda la ecuación por $m$:

$$\frac{1}{2}v_A^2 + gh = \frac{1}{2}v_B^2 \tag{2.4.4}$$

---

### Paso 2 — Despejar $v_A$

$$\frac{1}{2}v_A^2 = \frac{1}{2}v_B^2 - gh \tag{2.4.5}$$

$$v_A = \sqrt{v_B^2 - 2gh} \tag{2.4.6}$$

---

### Paso 3 — Sustitución numérica

$$v_A = \sqrt{(10 \ \text{m/s})^2 - 2(9.81 \ \text{m/s}^2)(5 \ \text{m})}$$

$$v_A = \sqrt{100 - 98.1} = \sqrt{1.9 \ \text{m}^2/\text{s}^2}$$

$$\boxed{v_A \approx 1.38 \ \text{m/s}}$$

---

### Verificación — Análisis de casos límite

| $v_B \ (\text{m/s})$ | $h \ (\text{m})$ | $v_A \ (\text{m/s})$ | Interpretación |
|---|---|---|---|
| $\sqrt{2gh} \approx 9.90$ | $5$ | $0$ | El saco parte del reposo |
| $10$ | $0$ | $10$ | Sin desnivel: $v_A = v_B$ |
| $10$ | $5$ | $1.38$ | **Este problema** |
| $10$ | $6$ | Sin solución real | $v_B$ insuficiente para superar $h$ |

---

### Interpretación física

La energía total del sistema se conserva a lo largo del riel. La energía potencial
gravitacional en A (altura $h = 5 \ \text{m}$) se transforma casi completamente en
energía cinética en B. El saco necesita solo $1.38 \ \text{m/s}$ en A porque la
gravedad aporta casi toda la energía cinética en B. Nótese que si $v_A = 0$,
el saco llegaría a B con $v_B = \sqrt{2gh} \approx 9.90 \ \text{m/s}$; el pequeño
aporte de $v_A$ eleva esa rapidez hasta exactamente $10 \ \text{m/s}$.
La forma de la trayectoria del riel es irrelevante para el resultado: solo importa
la diferencia de altura $h$ entre A y B.

[^Malthe-Sorensen_11]: Malthe-Sørenssen, A. (2015). *Elementary Mechanics Using Python:
A Modern Course Combining Analytical and Numerical Techniques*. Springer.
Cap. 11, §11.2, Ecs. (11.44)–(11.46).

---

## 18. Interpretación física global

La energía ofrece una forma poderosa de entender los fenómenos mecánicos.

Permite describir:

- cómo cambia el movimiento de un cuerpo;
- cómo se almacena energía;
- cómo se transfiere entre cuerpos o sistemas;
- cómo parte de la energía puede disiparse.

Así, el análisis energético complementa y en muchos casos simplifica el análisis dinámico.

---

## 19. Síntesis de la unidad

En esta unidad se estudió el trabajo mecánico como mecanismo de transferencia de energía y se introdujeron las principales formas de energía mecánica.

Se analizaron:

- el trabajo realizado por fuerzas
- el trabajo neto
- la energía cinética
- el teorema trabajo–energía
- la potencia
- la energía potencial gravitatoria
- la energía potencial elástica
- la conservación de la energía mecánica.

Estos conceptos constituyen una herramienta central para resolver problemas de mecánica de manera más eficiente y conceptual.

---

## Conceptos clave

- trabajo mecánico
- trabajo neto
- energía cinética
- teorema trabajo–energía
- potencia
- energía potencial
- energía potencial gravitatoria
- energía potencial elástica
- energía mecánica
- fuerzas conservativas
- fuerzas no conservativas
- conservación de la energía mecánica

---

## Fórmulas clave

$$
W = F \, \Delta r \cos\theta
$$

$$
W_{\text{neto}} = \sum_i W_i
$$

$$
K = \frac{1}{2}mv^2
$$

$$
W_{\text{neto}} = \Delta K
$$

$$
\Delta K = K_f - K_i
$$

$$
P_{\text{prom}} = \frac{\Delta W}{\Delta t}
$$

$$
U_g = mgy
$$

$$
\Delta U_g = mg(y_f - y_i)
$$

$$
U_e = \frac{1}{2}kx^2
$$

$$
E_m = K + U
$$

$$
K_i + U_i = K_f + U_f
$$

$$
W_{\text{nc}} = \Delta E_m
$$

$$
W = \vec{F} \cdot \Delta \vec{r}
$$

## Guía asociada

- **Guía 5**: Trabajo y energía mecánica