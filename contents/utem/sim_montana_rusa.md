# Simulación montaña rusa con resorte

Esta simulación interactiva corresponde a los contenidos de la **Unidad 5: Trabajo y energía mecánica**. Un carro de masa fija ($m = 10$ kg) parte desde una altura $H$ con velocidad inicial $v_0$, desciende sin roce por una pista curva y comprime un resorte de constante $k$ ubicado al final del tramo horizontal.

Presiona **▶ Iniciar** para correr la simulación. Modifica los parámetros y observa cómo la energía se redistribuye entre las formas cinética ($K$), potencial gravitatoria ($U_m$) y potencial elástica ($U_e$), manteniendo constante la energía mecánica total:

$$E = K + U_m + U_e = \tfrac{1}{2}mv^2 + mgy + \tfrac{1}{2}kx^2 = \text{cte.}$$

**Parámetros ajustables:**
- Altura inicial H
- Velocidad inicial v₀
- Constante del resorte k

```{raw} html
<iframe src="../../_static/montana_rusa_resorte.html"
        width="100%"
        height="860"
        style="border:none; border-radius:8px;">
</iframe>
```

La compresión máxima ocurre cuando toda la energía mecánica es potencial elástica:

$$x_{\max} = \sqrt{\dfrac{m v_0^2 + 2 m g H}{k}}$$
