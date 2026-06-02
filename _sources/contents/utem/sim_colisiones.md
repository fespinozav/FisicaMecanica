# Simulación: Colisiones y momentum lineal

Esta simulación interactiva corresponde a los contenidos de la **Unidad 7: Impulso y momentum lineal**. Permite explorar colisiones unidimensionales entre dos bloques y verificar la conservación del momentum lineal, comparando la energía cinética antes y después del choque.

**Parámetros ajustables:**
- Masa y velocidad inicial de cada bloque
- Coeficiente de restitución $e$ (de 0 a 1)

```{raw} html
<iframe src="../../_static/colisiones_momentum.html"
        width="100%"
        height="860"
        style="border:none; border-radius:8px;">
</iframe>
```

El coeficiente de restitución clasifica el tipo de colisión:

$$e = \frac{v_{2,f} - v_{1,f}}{v_{1,i} - v_{2,i}}$$

- $e = 1$: colisión elástica — se conservan momentum y energía cinética;
- $0 < e < 1$: colisión inelástica — se conserva el momentum, pero no la energía cinética;
- $e = 0$: colisión perfectamente inelástica — los bloques quedan unidos con la misma velocidad final.

En todos los casos, el **momentum lineal total** del sistema se conserva:

$$m_1 v_{1,i} + m_2 v_{2,i} = m_1 v_{1,f} + m_2 v_{2,f}$$
