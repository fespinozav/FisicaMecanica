# Simulación: cinemática en dos dimensiones

Esta simulación corresponde a los contenidos de las **Unidades 1–2: Cinemática**. Permite explorar el movimiento de una partícula en el plano bajo velocidad inicial y aceleración constante en cada eje, observando cómo cambia la trayectoria y las ecuaciones de movimiento según las condiciones iniciales.

**Casos que se pueden explorar:**

- Si $v_{x0} = 0$ y $a_x = 0$: **tiro vertical** (movimiento unidimensional en Y).
- Si $v_{y0} = 0$ y $a_y = 0$: **movimiento rectilíneo horizontal** (MRU o MRUA en X).
- Si ambas componentes son distintas de cero: **movimiento parabólico** (tiro oblicuo).
- Si $a_x = a_y = 0$: **MRU diagonal** (velocidad constante en ambas direcciones).

Las ecuaciones cinemáticas que gobiernan el movimiento son:

$$x(t) = v_{x0}\,t + \tfrac{1}{2}\,a_x\,t^2 \qquad y(t) = v_{y0}\,t + \tfrac{1}{2}\,a_y\,t^2$$

$$v_x(t) = v_{x0} + a_x\,t \qquad v_y(t) = v_{y0} + a_y\,t$$

Cuando $a_x = 0$ y $v_{x0} \neq 0$, es posible eliminar el tiempo y obtener la **ecuación de itinerario**:

$$y(x) = \frac{v_{y0}}{v_{x0}}\,x + \frac{a_y}{2\,v_{x0}^2}\,x^2$$

```{raw} html
<iframe src="../../_static/cinematica_2d.html"
        width="100%"
        height="860"
        style="border:none; border-radius:8px;">
</iframe>
```
