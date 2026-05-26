# Simulación: movimiento circular

Esta simulación corresponde a los contenidos de la **Unidad 3: Movimiento circular**. Permite comparar el **movimiento circular uniforme (MCU)** y el **movimiento circular uniformemente acelerado (MCUA)**, observando en tiempo real las variables angulares y las magnitudes físicas asociadas.

**Modos disponibles:**

- **MCU** — velocidad angular $\omega$ constante; la aceleración centrípeta $a_n = \omega^2 r$ apunta al centro.
- **MCUA** — aceleración angular $\alpha$ constante; la velocidad angular varía como $\omega(t) = \omega_0 + \alpha\,t$ y aparece una componente tangencial de la aceleración.

Las ecuaciones del movimiento circular son:

$$\theta(t) = \omega_0\,t + \tfrac{1}{2}\,\alpha\,t^2 \qquad \omega(t) = \omega_0 + \alpha\,t$$

Las magnitudes cinemáticas en cualquier instante:

$$v_t = \omega\,r \qquad a_n = \omega^2\,r \qquad a_t = \alpha\,r$$

La simulación muestra el ángulo $\theta$ tanto en **radianes** como en **grados**, el número de **vueltas completas** y los vectores de velocidad tangencial $\vec{v}_t$ (verde) y aceleración centrípeta $\vec{a}_n$ (naranja). En MCUA aparece además el vector de aceleración tangencial $\vec{a}_t$ (rojo).

```{raw} html
<iframe src="../../_static/movimiento_circular.html"
        width="100%"
        height="900"
        style="border:none; border-radius:8px;">
</iframe>
```
