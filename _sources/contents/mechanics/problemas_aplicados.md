# Problemas aplicados, tareas y proyectos

El trabajo del curso no se reduce a leer capitulos. La comprension profunda de la mecanica aparece cuando las ideas se ponen a prueba en ejercicios, guias, modelaciones numericas y actividades integradoras.

## Como usar este bloque

Se recomienda combinar cuatro niveles de trabajo:

1. lectura conceptual de cada unidad;
1. resolucion breve de problemas tipo;
1. desarrollo guiado de actividades numericas o de modelacion;
1. y elaboracion de una entrega mas integrada cuando corresponda.

## Ruta sugerida de ejercitacion

### Nivel 1: consolidacion conceptual

- preguntas cortas de definiciones y relaciones entre magnitudes;
- interpretacion de graficos y diagramas;
- y chequeo de unidades, signos y orden de magnitud.

### Nivel 2: problemas estandar

- cinemática en una y dos dimensiones;
- aplicacion de leyes de Newton;
- trabajo, energia, momentum y torque;
- oscilaciones y rotacion;
- y gravitación con enfoque orbital.

### Nivel 3: modelacion numerica

- discretizacion de ecuaciones de movimiento;
- comparacion entre algoritmos;
- control de error y estabilidad;
- y lectura fisica de resultados computacionales.

## Proyectos o evaluaciones integradoras

Una evaluacion integradora puede pedir que el estudiantado:

- modele un sistema mecanico con supuestos explicitos;
- derive ecuaciones de movimiento;
- resuelva el problema analitica o numericamente segun corresponda;
- compare escenarios o parametros;
- y comunique resultados con argumentos fisicos claros.

## Vinculo con las guias del curso

Las [Guias de trabajo UTEM](../utem/guias_trabajo.md) funcionan como base de ejercitacion sistematica. Pueden complementarse con informes breves, tareas computacionales o controles de aplicacion segun la organizacion del semestre.

## Criterios de calidad para una buena entrega

- Definir con claridad el sistema fisico.
- Declarar supuestos y limites del modelo.
- Mostrar el desarrollo matematico esencial.
- Verificar consistencia de unidades y resultados.
- Explicar el significado fisico de la respuesta final.

---
## Ejercicio Integrador: Unidades 1–6

```{admonition} Problema integrador
:class: tip

Un cohete de masa total $M = 12{,}0\ \text{kg}$ es lanzado verticalmente desde el suelo
con velocidad inicial $v_0 = 0$. Sus motores generan una fuerza de empuje constante
$F = 180{,}0\ \text{N}$ durante una fase de ascenso de $h_1 = 80{,}0\ \text{m}$.
Al alcanzar esa altura, el cohete se separa en dos fragmentos iguales
($m_1 = m_2 = 6{,}0\ \text{kg}$):
el **fragmento 1** sale despedido horizontalmente con $\vec{v}_1 = +15{,}0\,\hat{i}\ \text{m/s}$,
y el **fragmento 2** continúa moviéndose.

Determinar:

**(A)** El vector posición del CM al final de la fase de empuje. *(Unidad 1)*

**(B)** La aceleración neta y la velocidad del cohete al final del empuje. *(Unidades 2 y 4)*

**(C)** La velocidad vectorial del fragmento 2 justo después de la separación. *(Unidad 6)*

**(D)** La velocidad del fragmento 2 cuando alcanza su altura máxima. *(Unidad 3)*

**(E)** La energía mecánica total del sistema en el instante de la separación
y la energía cinética de cada fragmento. *(Unidad 5)*

**(F)** La posición del CM en el instante de la separación y su trayectoria posterior. *(Unidad 6)*
```

---

## Datos del problema

| Símbolo | Valor | Unidad | Unidad de origen |
|:-------:|:-----:|:------:|:----------------:|
| $M$ | 12,0 | kg | — |
| $F$ | 180,0 | N | U4 — Dinámica |
| $h_1$ | 80,0 | m | U2 — Cinemática 1D |
| $g$ | 9,8 | m/s² | U4 — Dinámica |
| $v_0$ | 0 | m/s | U2 — Cinemática 1D |
| $m_1 = m_2$ | 6,0 | kg | U6 — Sistema de partículas |
| $v_{1x}$ | +15,0 | m/s | U6 — Sistema de partículas |

---

## Diagramas de cuerpo libre

```{raw} html
<svg width="100%" viewBox="0 0 680 980" role="img"
     xmlns="http://www.w3.org/2000/svg"
     style="font-family: sans-serif; font-size: 12px;">
  <title>Diagramas de cuerpo libre — Ejercicio integrador cohete bietápico</title>
  <desc>Cuatro DCL: fase de empuje, fragmento 1, fragmento 2 y sistema CM post-separación</desc>
  <defs>
    <marker id="arw" viewBox="0 0 10 10" refX="8" refY="5"
            markerWidth="6" markerHeight="6" orient="auto-start-reverse">
      <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke"
            stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
    </marker>
  </defs>

  <!-- ── DCL 1: Cohete completo ── -->
  <rect x="40" y="30" width="600" height="26" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="340" y="47" text-anchor="middle" dominant-baseline="central"
        font-weight="500" font-size="13">DCL fase 1 — Cohete completo durante el empuje (M = 12,0 kg)</text>

  <line x1="340" y1="295" x2="340" y2="80"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="348" y="84" font-size="11" fill="#888">ĵ</text>
  <line x1="240" y1="200" x2="460" y2="200"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="462" y="204" font-size="11" fill="#888">î</text>
  <circle cx="340" cy="200" r="3" fill="#888"/>
  <text x="328" y="215" font-size="11" fill="#888">O</text>

  <!-- Cohete -->
  <polygon points="340,115 315,170 365,170"
           fill="#e8e8e8" stroke="#555" stroke-width="1.2"/>
  <rect x="315" y="170" width="50" height="55" rx="3"
        fill="#e8e8e8" stroke="#555" stroke-width="1.2"/>
  <polygon points="325,225 340,255 355,225"
           fill="#f5c542" stroke="#c8a000" stroke-width="0.8" opacity="0.9"/>

  <!-- F empuje -->
  <line x1="340" y1="200" x2="340" y2="100"
        stroke="#0f6e56" stroke-width="2.2" marker-end="url(#arw)"/>
  <rect x="350" y="94" width="135" height="20" rx="4"
        fill="#e1f5ee" opacity="0.9"/>
  <text x="355" y="107" font-size="11" fill="#0f6e56">F = 180,0 N ↑ (empuje)</text>

  <!-- W peso -->
  <line x1="340" y1="200" x2="340" y2="280"
        stroke="#993c1d" stroke-width="2.2" marker-end="url(#arw)"/>
  <rect x="350" y="275" width="170" height="20" rx="4"
        fill="#faece7" opacity="0.9"/>
  <text x="355" y="288" font-size="11" fill="#993c1d">W = Mg = 117,6 N ↓ (peso)</text>

  <!-- a_cm -->
  <line x1="260" y1="200" x2="260" y2="152"
        stroke="#534ab7" stroke-width="2"
        stroke-dasharray="5 3" marker-end="url(#arw)"/>
  <text x="172" y="165" font-size="11" fill="#534ab7">a = 5,2 m/s² ↑</text>

  <!-- Cajas resultado -->
  <rect x="40" y="290" width="270" height="36" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="52" y="305" font-size="11">ΣF = F − W = 62,4 N</text>
  <text x="52" y="318" font-size="11">a = ΣF / M = 5,2 m/s²</text>

  <rect x="370" y="290" width="270" height="36" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="382" y="305" font-size="11">v_A² = 2 a h₁ = 832 m²/s²</text>
  <text x="382" y="318" font-size="11">v_A = 28,8 m/s ĵ</text>

  <!-- Separador -->
  <line x1="40" y1="348" x2="640" y2="348"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="6 4"/>

  <!-- ── DCL 2a: Fragmento 1 ── -->
  <rect x="40" y="362" width="600" height="26" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="340" y="379" text-anchor="middle" dominant-baseline="central"
        font-weight="500" font-size="13">DCL fase 2a — Fragmento 1 (m₁ = 6,0 kg, proyectil)</text>

  <line x1="220" y1="580" x2="220" y2="420"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="228" y="424" font-size="11" fill="#888">ĵ</text>
  <line x1="130" y1="510" x2="320" y2="510"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="322" y="514" font-size="11" fill="#888">î</text>
  <circle cx="220" cy="510" r="3" fill="#888"/>

  <rect x="196" y="476" width="48" height="38" rx="5"
        fill="#e8e8e8" stroke="#555" stroke-width="1.2"/>
  <text x="220" y="498" text-anchor="middle" font-size="11">m₁</text>

  <line x1="220" y1="510" x2="220" y2="575"
        stroke="#993c1d" stroke-width="2.2" marker-end="url(#arw)"/>
  <text x="230" y="580" font-size="11" fill="#993c1d">W₁ = 58,8 N ↓</text>

  <line x1="220" y1="495" x2="295" y2="495"
        stroke="#0f6e56" stroke-width="2"
        stroke-dasharray="5 3" marker-end="url(#arw)"/>
  <text x="230" y="488" font-size="11" fill="#0f6e56">v₁ = +15,0 î m/s</text>

  <rect x="40" y="598" width="300" height="48" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="52" y="614" font-size="11">Solo actúa W₁ (proyectil sin roce)</text>
  <text x="52" y="628" font-size="11">Trayectoria parabólica.</text>
  <text x="52" y="642" font-size="11">En altura máx.: v_y = 0, v_x = +15,0 m/s</text>

  <!-- ── DCL 2b: Fragmento 2 ── -->
  <line x1="520" y1="580" x2="520" y2="420"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="528" y="424" font-size="11" fill="#888">ĵ</text>
  <line x1="390" y1="510" x2="620" y2="510"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="622" y="514" font-size="11" fill="#888">î</text>
  <circle cx="520" cy="510" r="3" fill="#888"/>

  <rect x="496" y="476" width="48" height="38" rx="5"
        fill="#e8e8e8" stroke="#555" stroke-width="1.2"/>
  <text x="520" y="498" text-anchor="middle" font-size="11">m₂</text>

  <line x1="520" y1="510" x2="520" y2="575"
        stroke="#993c1d" stroke-width="2.2" marker-end="url(#arw)"/>
  <text x="530" y="580" font-size="11" fill="#993c1d">W₂ = 58,8 N ↓</text>

  <line x1="520" y1="510" x2="520" y2="432"
        stroke="#0f6e56" stroke-width="2"
        stroke-dasharray="5 3" marker-end="url(#arw)"/>
  <text x="530" y="440" font-size="11" fill="#0f6e56">v₂y = +57,6 m/s ↑</text>

  <line x1="520" y1="495" x2="440" y2="495"
        stroke="#534ab7" stroke-width="2"
        stroke-dasharray="5 3" marker-end="url(#arw)"/>
  <text x="348" y="489" font-size="11" fill="#534ab7">v₂x = −15,0 m/s ←</text>

  <rect x="360" y="598" width="280" height="48" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="372" y="614" font-size="11">Solo actúa W₂ (proyectil sin roce)</text>
  <text x="372" y="628" font-size="11">v⃗₂ = −15,0 î + 57,6 ĵ m/s</text>
  <text x="372" y="642" font-size="11">Por conservación de momentum</text>

  <!-- Separador -->
  <line x1="40" y1="664" x2="640" y2="664"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="6 4"/>

  <!-- ── DCL Sistema CM post-separación ── -->
  <rect x="40" y="678" width="600" height="26" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="340" y="695" text-anchor="middle" dominant-baseline="central"
        font-weight="500" font-size="13">DCL sistema — CM post-separación (M = 12,0 kg)</text>

  <line x1="340" y1="900" x2="340" y2="730"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="348" y="734" font-size="11" fill="#888">ĵ</text>
  <line x1="230" y1="830" x2="460" y2="830"
        stroke="#b0b0b0" stroke-width="0.5" stroke-dasharray="4 3"/>
  <text x="462" y="834" font-size="11" fill="#888">î</text>
  <circle cx="340" cy="830" r="5" fill="#534ab7" opacity="0.75"/>
  <text x="350" y="846" font-size="11" fill="#534ab7">CM</text>

  <line x1="340" y1="830" x2="340" y2="900"
        stroke="#993c1d" stroke-width="2.2" marker-end="url(#arw)"/>
  <text x="350" y="910" font-size="11" fill="#993c1d">W = Mg = 117,6 N ↓</text>

  <line x1="340" y1="830" x2="340" y2="760"
        stroke="#534ab7" stroke-width="2"
        stroke-dasharray="5 3" marker-end="url(#arw)"/>
  <text x="350" y="754" font-size="11" fill="#534ab7">v_cm = 28,8 ĵ m/s (conservada)</text>

  <rect x="196" y="806" width="42" height="30" rx="4"
        fill="#e8e8e8" stroke="#b0b0b0" stroke-width="0.8" opacity="0.55"/>
  <text x="217" y="824" text-anchor="middle" font-size="10" opacity="0.55">m₁</text>

  <rect x="412" y="806" width="42" height="30" rx="4"
        fill="#e8e8e8" stroke="#b0b0b0" stroke-width="0.8" opacity="0.55"/>
  <text x="433" y="824" text-anchor="middle" font-size="10" opacity="0.55">m₂</text>

  <rect x="40" y="918" width="600" height="46" rx="6"
        fill="#f5f5f5" stroke="#b0b0b0" stroke-width="0.5"/>
  <text x="340" y="936" text-anchor="middle" font-size="11">
    Las fuerzas internas (explosión) no modifican el estado del CM.
  </text>
  <text x="340" y="952" text-anchor="middle" font-size="11">
    Solo W actúa sobre el sistema → el CM sigue trayectoria de proyectil vertical.
  </text>
</svg>
```

---

## Parte A — Vector posición al final del empuje

**Unidad 1: vectores y sistema de referencia**

El cohete asciende verticalmente. El origen se ubica en el punto de lanzamiento con $\hat{j}$ apuntando hacia arriba.

$$
\vec{r}_A = h_1\,\hat{j} = \boxed{80{,}0\,\hat{j}\ \text{m}}
$$ (I.1)

---

## Parte B — Aceleración y velocidad al final del empuje

**Unidad 4: Segunda Ley de Newton | Unidad 2: cinemática 1D (M.R.U.A.)**

### Segunda Ley de Newton sobre el eje $\hat{j}$

$$
F - Mg = Ma
$$ (I.2)

$$
a = \frac{F - Mg}{M} = \frac{180{,}0 - (12{,}0)(9{,}8)}{12{,}0} = \frac{180{,}0 - 117{,}6}{12{,}0} = \frac{62{,}4}{12{,}0}
$$ (I.3)

$$
\boxed{a = 5{,}2\ \text{m/s}^2\ \hat{j}}
$$ (I.4)

### Cinemática 1D — velocidad al final del empuje

Desde reposo ($v_0 = 0$) con aceleración constante $a$:

$$
v_A^2 = v_0^2 + 2a\,h_1 = 0 + 2(5{,}2)(80{,}0) = 832{,}0\ \text{m}^2/\text{s}^2
$$ (I.5)

$$
\boxed{v_A = 28{,}8\ \text{m/s}\ \hat{j}}
$$ (I.6)

---

## Parte C — Velocidad del fragmento 2 (conservación de momentum)

**Unidad 6: sistema de partículas**

En el instante de la separación solo actúan fuerzas internas (explosión). Por lo tanto el sistema es aislado en ese instante y el momentum se conserva:

$$
\vec{P}_i = M\,v_A\,\hat{j} = (12{,}0)(28{,}8)\,\hat{j} = 345{,}6\,\hat{j}\ \text{kg·m/s}
$$ (I.7)

$$
\vec{P}_f = m_1\vec{v}_1 + m_2\vec{v}_2 = \vec{P}_i
$$ (I.8)

$$
345{,}6\,\hat{j} = (6{,}0)(15{,}0\,\hat{i}) + (6{,}0)\vec{v}_2
$$ (I.9)

**Componente $\hat{i}$:**

$$
0 = 90{,}0 + 6{,}0\,v_{2x} \implies v_{2x} = -15{,}0\ \text{m/s}
$$ (I.10)

**Componente $\hat{j}$:**

$$
345{,}6 = 0 + 6{,}0\,v_{2y} \implies v_{2y} = 57{,}6\ \text{m/s}
$$ (I.11)

$$
\boxed{\vec{v}_2 = -15{,}0\,\hat{i} + 57{,}6\,\hat{j}\ \text{m/s}}
$$ (I.12)

---

## Parte D — Velocidad del fragmento 2 en la altura máxima

**Unidad 3: cinemática bidimensional (proyectil)**

El fragmento 2 es un proyectil bajo gravedad. En la altura máxima, la componente vertical se anula. La componente horizontal se conserva (sin rozamiento del aire):

$$
v_{2y}(t_{top}) = 0
$$ (I.13)

$$
v_{2x}(t_{top}) = -15{,}0\ \text{m/s}\ (\text{constante})
$$ (I.14)

$$
\boxed{\vec{v}_2\big|_{max} = -15{,}0\,\hat{i}\ \text{m/s}}
$$ (I.15)

---

## Parte E — Energía mecánica

**Unidad 5: trabajo y energía mecánica**

### Trabajo neto durante el empuje

$$
W_{neto} = W_{empuje} + W_{gravedad} = F\,h_1 - Mg\,h_1
$$ (I.16)

$$
W_{neto} = (180{,}0)(80{,}0) - (12{,}0)(9{,}8)(80{,}0) = 14\,400 - 9\,408 = 4\,992\ \text{J}
$$ (I.17)

Verificación con el teorema trabajo-energía:

$$
\Delta K = \tfrac{1}{2}Mv_A^2 - 0 = \tfrac{1}{2}(12{,}0)(832{,}0) = 4\,992\ \text{J} \quad \checkmark
$$ (I.18)

### Energía potencial en el punto de separación

$$
U_A = Mgh_1 = (12{,}0)(9{,}8)(80{,}0) = 9\,408\ \text{J}
$$ (I.19)

### Energía mecánica total en el instante de la separación

$$
E_A = K_A + U_A = 4\,992 + 9\,408 = \boxed{14\,400\ \text{J}}
$$ (I.20)

Este valor coincide con el trabajo entregado por los motores, consistente con el balance energético total.

### Energía cinética de cada fragmento justo después de la separación

$$
K_1 = \tfrac{1}{2}m_1\,v_1^2 = \tfrac{1}{2}(6{,}0)(15{,}0)^2 = \boxed{675\ \text{J}}
$$ (I.21)

$$
K_2 = \tfrac{1}{2}m_2\,|\vec{v}_2|^2 = \tfrac{1}{2}(6{,}0)\left[(15{,}0)^2 + (57{,}6)^2\right] = 3(225 + 3\,317{,}8) = \boxed{10\,628\ \text{J}}
$$ (I.22)

$$
K_1 + K_2 = 11\,303\ \text{J} > K_A = 4\,992\ \text{J}
$$ (I.23)

```{note}
La diferencia $\Delta K = 6\,311\ \text{J}$ proviene de la energía química liberada por la explosión.
Las fuerzas internas sí pueden hacer trabajo sobre las partes individuales del sistema,
aunque no modifican el estado del CM.
```

---

## Parte F — Posición del CM y trayectoria post-separación

**Unidad 6: dinámica del sistema de partículas**

### Posición del CM en el instante de la separación

Ambos fragmentos parten del mismo punto $\vec{r}_A$:

$$
\vec{r}_{cm}\big|_A = \frac{m_1\vec{r}_A + m_2\vec{r}_A}{M} = \vec{r}_A = \boxed{80{,}0\,\hat{j}\ \text{m}}
$$ (I.24)

### Velocidad del CM post-separación

$$
\vec{v}_{cm} = \frac{m_1\vec{v}_1 + m_2\vec{v}_2}{M}
= \frac{(6{,}0)(15{,}0\,\hat{i}) + (6{,}0)(-15{,}0\,\hat{i} + 57{,}6\,\hat{j})}{12{,}0}
$$ (I.25)

$$
\vec{v}_{cm} = \frac{0\,\hat{i} + 345{,}6\,\hat{j}}{12{,}0} = \boxed{28{,}8\,\hat{j}\ \text{m/s}}
$$ (I.26)

La velocidad del CM es exactamente $v_A\,\hat{j}$: la explosión no la modificó.

### Trayectoria del CM después de la separación

Después de la separación, la única fuerza externa sobre el sistema es la gravedad $\vec{W} = -Mg\,\hat{j}$. Por la Segunda Ley para sistemas:

$$
\sum\vec{F}_{ext} = M\vec{a}_{cm} \implies \vec{a}_{cm} = -g\,\hat{j}
$$ (I.27)

El CM sigue una trayectoria de proyectil **vertical** idéntica a la de una partícula de masa $M$ lanzada con $v_A\,\hat{j}$ desde $h_1$, independientemente del caos interno de la explosión.

---

## Verificación: tabla de casos límite

| Condición | Predicción | Consistencia |
|:----------|:-----------|:------------:|
| $F = Mg$ | $a = 0$, el cohete no despega | ✓ |
| $m_1 \to 0$ | $\vec{v}_2 \to v_A\,\hat{j}$, sin cambio en el CM | ✓ |
| Fragmentos con velocidades iguales | $\vec{v}_{cm}$ post-explosión = $v_A\,\hat{j}$ | ✓ |
| $K_1 + K_2 = K_A$ | Separación sin energía interna liberada | ✓ (caso especial) |
| $h_1 \to 0$ | $v_A \to 0$, sistema no acumula energía | ✓ |

---

## Interpretación física global

Este ejercicio ilustra la jerarquía conceptual de la mecánica clásica de partículas:

El **sistema de referencia y los vectores** (U1) son el lenguaje en que se expresan todas las demás unidades. La **cinemática** (U2, U3) describe el movimiento sin preguntar por sus causas. La **dinámica** (U4) conecta causas (fuerzas) con efectos (aceleraciones). El **trabajo y la energía** (U5) ofrecen un camino alternativo —escalar— para obtener velocidades sin resolver ecuaciones diferenciales. Finalmente, la **dinámica de sistemas** (U6) revela que el CM es un observador impasible del caos interno: las fuerzas internas, por intensas que sean, no pueden mover al CM si no hay fuerza externa neta.

```{note}
**Referencias:**
Malthe-Sørenssen, A. (2015). *Elementary Mechanics Using Python*. Springer.
§7 (proyectiles), §9 (Segunda Ley), §10 (trabajo y energía), §13 (sistemas de partículas).
```

---

## Código Python

```python
import numpy as np

# ── Datos ──────────────────────────────────────────────────
M  = 12.0   # kg — masa total del cohete
F  = 180.0  # N  — fuerza de empuje
h1 = 80.0   # m  — altura de la fase de empuje
g  = 9.8    # m/s²
m1 = 6.0    # kg — masa fragmento 1
m2 = 6.0    # kg — masa fragmento 2
v1 = np.array([15.0, 0.0])   # m/s — velocidad fragmento 1 (î)

# ── Parte B: aceleración y velocidad al final del empuje ───
W_cohete = M * g
a = (F - W_cohete) / M
vA = np.sqrt(2 * a * h1)
print(f"Aceleración: a = {a:.2f} m/s²")
print(f"Velocidad final empuje: vA = {vA:.2f} m/s")

# ── Parte C: velocidad fragmento 2 ─────────────────────────
P_i = np.array([0.0, M * vA])       # momentum antes
P_frag1 = m1 * v1
v2 = (P_i - P_frag1) / m2
print(f"Velocidad fragmento 2: v2 = {v2} m/s")

# ── Parte D: velocidad frag 2 en altura máxima ─────────────
v2_top = np.array([v2[0], 0.0])
print(f"Velocidad frag 2 en altura máxima: {v2_top} m/s")

# ── Parte E: energías ──────────────────────────────────────
KA   = 0.5 * M * vA**2
UA   = M * g * h1
EA   = KA + UA
K1   = 0.5 * m1 * np.dot(v1, v1)
K2   = 0.5 * m2 * np.dot(v2, v2)
dK   = K1 + K2 - KA
print(f"Energía mecánica total en separación: EA = {EA:.1f} J")
print(f"K1 = {K1:.1f} J  |  K2 = {K2:.1f} J")
print(f"Energía liberada por explosión: ΔK = {dK:.1f} J")

# ── Parte F: velocidad del CM post-separación ──────────────
v_cm = (m1 * v1 + m2 * v2) / M
print(f"Velocidad CM post-separación: v_cm = {v_cm} m/s")
print(f"Coincide con vA ĵ: {np.isclose(v_cm, [0, vA]).all()}")
```