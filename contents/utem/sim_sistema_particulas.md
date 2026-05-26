# Simulación: centro de masa de un sistema de partículas

Esta simulación corresponde a los contenidos de la **Unidad 6: Dinámica de un sistema de partículas**. Permite explorar cómo se calcula y se mueve el centro de masa (CM) de un sistema formado por 2, 3 o 4 partículas, observando en tiempo real las ecuaciones de posición y velocidad del CM.

**Conceptos que se pueden explorar:**

- La posición del centro de masa depende de la distribución de masas, no solo de las posiciones.
- El CM se mueve a velocidad constante cuando no hay fuerzas externas netas (conservación del momento lineal).
- La velocidad del CM es el promedio ponderado de las velocidades individuales.
- La cantidad de movimiento total del sistema es $\vec{p}_{total} = M\,\vec{v}_{cm}$.

Las ecuaciones que gobiernan el centro de masa son:

$$
\vec{r}_{cm} = \frac{\displaystyle\sum_{i=1}^{N} m_i\,\vec{r}_i}{\displaystyle\sum_{i=1}^{N} m_i}
\qquad
\vec{v}_{cm} = \frac{\displaystyle\sum_{i=1}^{N} m_i\,\vec{v}_i}{\displaystyle\sum_{i=1}^{N} m_i}
$$

La segunda ley de Newton para el sistema completo toma la forma:

$$
\vec{F}_{ext} = M\,\vec{a}_{cm}
$$

donde $M = \sum m_i$ es la masa total y $\vec{F}_{ext}$ es la fuerza externa neta sobre el sistema.

```{raw} html
<iframe src="../../_static/sistema_particulas_cm.html"
        width="100%"
        height="820"
        style="border:none; border-radius:8px;">
</iframe>
```
