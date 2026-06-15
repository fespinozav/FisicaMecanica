# Simulación: Estática del sólido rígido — DCL interactivo

Esta simulación interactiva corresponde a los contenidos de la **Unidad 8: Estática del sólido rígido**. Permite construir el diagrama de cuerpo libre (DCL) de una barra rígida con pivote, activar o desactivar las fuerzas del sistema, y calcular los torques para determinar el sentido de giro o si el sistema se encuentra en equilibrio rotacional.

**Parámetros ajustables:**
- Longitud y masa de la barra (el peso se aplica automáticamente en el centro de masa)
- Posición del pivote a lo largo de la barra
- Tres fuerzas independientes (F₁, F₂, F₃), cada una con magnitud, posición y dirección (↑ o ↓) configurables
- Activación/desactivación individual de cada fuerza

```{raw} html
<iframe src="../../_static/estatica_barra_dcl.html"
        width="100%"
        height="760"
        style="border:none; border-radius:8px;">
</iframe>
```

El torque de cada fuerza respecto al pivote $x_0$ se calcula como:

$$\tau_i = F_{y,i} \cdot (x_i - x_0)$$

donde $F_{y,i}$ es positivo hacia arriba y negativo hacia abajo. La convención de signos adoptada es:

- $\tau > 0$: tendencia de rotación **antihoraria** (↺)
- $\tau < 0$: tendencia de rotación **horaria** (↻)
- $\sum \tau = 0$: equilibrio rotacional

La reacción en el pivote $N$ se calcula a partir de la condición de equilibrio traslacional:

$$\sum F_y = 0 \implies N = -\sum F_{y,i}$$
