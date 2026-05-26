# Simulación plano inclinado de fuerzas

Esta simulación interactiva corresponde a los contenidos de la **Unidad 4: Dinámica de la partícula**. Permite explorar las fuerzas que actúan sobre un bloque en un plano inclinado — peso, normal, roce y la componente paralela del peso — y verificar de forma visual cuándo el bloque se desliza o permanece en reposo.

**Parámetros ajustables:**
- Ángulo de inclinación θ
- Masa del bloque m
- Coeficiente de roce cinético μ

```{raw} html
<iframe src="../../_static/plano_inclinado_fuerzas.html"
        width="100%"
        height="720"
        style="border:none; border-radius:8px;">
</iframe>
```

La condición de deslizamiento se cumple cuando la componente del peso paralela al plano supera la fuerza de roce máxima estática:

$$P_x > f_k \quad\Longleftrightarrow\quad mg\sin\theta > \mu\, mg\cos\theta \quad\Longleftrightarrow\quad \tan\theta > \mu$$
