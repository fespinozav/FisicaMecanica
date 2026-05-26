# Simulación montaña rusa con resorte

Esta simulación interactiva corresponde a los contenidos de la **Unidad 5: Trabajo y energía mecánica**. Un carro de masa fija ($m = 10$ kg) parte desde una altura $H$ con velocidad inicial $v_0$, desciende por una pista curva y comprime un resorte de constante $k$ ubicado al final del tramo horizontal.

Presiona **▶ Iniciar** para correr la simulación. Modifica los parámetros y observa cómo varía la distribución de energía.

**Sin roce** ($\mu = 0$): la energía mecánica total se conserva en todo instante:

$$E_0 = K + U_m + U_e = \tfrac{1}{2}mv^2 + mgy + \tfrac{1}{2}kx^2 = \text{cte.}$$

**Con roce** ($\mu > 0$): la fricción cinética realiza trabajo negativo a razón de $dE^f = \mu\,m\,g\,ds$, de modo que la energía mecánica **disminuye** con la distancia recorrida $s$:

$$E^f = \mu\,m\,g\,s \qquad \Rightarrow \qquad E_m(s) = E_0 - E^f$$

y la ecuación de energía toma la forma:

$$K + U_m + U_e = E_0 - \mu\,m\,g\,s$$

El carro se detiene cuando $E_m \to 0$, es decir, cuando toda la energía inicial ha sido disipada por roce.

**Parámetros ajustables:**
- Altura inicial $H$
- Velocidad inicial $v_0$
- Constante del resorte $k$
- Coeficiente de roce $\mu$

```{raw} html
<iframe src="../../_static/montana_rusa_resorte.html"
        width="100%"
        height="860"
        style="border:none; border-radius:8px;">
</iframe>
```

La compresión máxima ocurre cuando toda la energía mecánica disponible es potencial elástica. **Sin roce** se tiene la expresión exacta:

$$x_{\max} = \sqrt{\dfrac{m v_0^2 + 2 m g H}{k}}$$

**Con roce**, la energía disponible al llegar al resorte es $E_0 - \mu\,m\,g\,s_0$ (donde $s_0$ es la distancia recorrida hasta el punto de contacto), por lo que la compresión real es menor que el valor anterior.
