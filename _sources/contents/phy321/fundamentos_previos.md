# Fundamentos previos: vectores, coordenadas y operadores basicos

Esta unidad preliminar sintetiza, en espanol, un repaso de vectores y otras magnitudes matematicas utiles para el inicio del curso.

## Para que sirve este repaso

Antes de estudiar leyes de Newton, energia, oscilaciones o problemas de dos cuerpos, conviene fijar un lenguaje comun para describir sistemas mecanicos. Ese lenguaje incluye:

- la eleccion de un origen y de ejes de referencia,
- la orientacion positiva del sistema de coordenadas,
- las unidades fisicas y las dimensiones de cada magnitud,
- y la distincion entre cantidades escalares, vectoriales y matriciales.

Este repaso funciona como puente entre el inicio del curso y el bloque de herramientas matematicas y numericas del libro.

## Preguntas fundamentales al comenzar

Cuando modelamos el movimiento de una particula o de un sistema, aparecen de inmediato preguntas como estas:

- La fisica del problema cambia si movemos el origen de coordenadas.
- Existen direcciones privilegiadas en el espacio.
- La descripcion cambia si usamos un sistema dextrorso o levogiro.
- El resultado depende de la escala elegida para medir longitudes, tiempos o masas.

Estas preguntas ayudan a distinguir entre lo que depende de nuestra representacion y lo que realmente corresponde a una ley fisica.

## Magnitudes y notacion basica

En este curso usaremos unidades SI. Algunas magnitudes centrales son:

- posicion: $\boldsymbol{r}$
- masa: $m$
- tiempo: $t$
- velocidad: $\boldsymbol{v}$
- aceleracion: $\boldsymbol{a}$
- momentum lineal: $\boldsymbol{p}$
- energia cinetica: $K$
- energia potencial: $V$
- frecuencia angular: $\omega$

Tambien es importante distinguir entre **unidad** y **dimension**. Por ejemplo:

- $[\boldsymbol{r}] =$ longitud
- $[\boldsymbol{v}] =$ longitud/tiempo
- $[\boldsymbol{a}] =$ longitud/tiempo$^2$
- $[\boldsymbol{p}] =$ masa por longitud/tiempo
- $[K] =$ energia
- $[\omega] =$ 1/tiempo

## Escalares, vectores y matrices

Un **escalar** queda completamente descrito por su magnitud. La masa, el tiempo o la energia son ejemplos habituales.

Un **vector** requiere modulo, direccion y sentido. En coordenadas cartesianas escribimos, por ejemplo,

$$
\boldsymbol{a}=(a_x,a_y,a_z)
$$

o bien

$$
\boldsymbol{a}=a_x\boldsymbol{e}_1+a_y\boldsymbol{e}_2+a_z\boldsymbol{e}_3,
$$

donde $\boldsymbol{e}_1$, $\boldsymbol{e}_2$ y $\boldsymbol{e}_3$ son vectores unitarios.

Una **matriz** organiza relaciones lineales entre componentes y resulta especialmente util cuando trabajamos con cambios de base, rotaciones o sistemas de ecuaciones.

## Coordenadas cartesianas y polares

En dos dimensiones, un vector posicion puede escribirse como

$$
\boldsymbol{r}=x\boldsymbol{e}_1+y\boldsymbol{e}_2.
$$

La misma informacion puede expresarse en coordenadas polares:

$$
\boldsymbol{r}=\rho\cos\phi\,\boldsymbol{e}_1+\rho\sin\phi\,\boldsymbol{e}_2.
$$

La idea central es que una misma magnitud fisica puede representarse con distintas coordenadas sin cambiar su significado fisico. Cambia la descripcion; no cambia el objeto.

## Vectores unitarios y cambio de base

Los vectores unitarios:

- tienen norma igual a 1,
- apuntan en la direccion de los ejes,
- y forman una base ortonormal cuando son mutuamente perpendiculares.

En una base ortonormal se cumple

$$
\boldsymbol{e}_i\cdot\boldsymbol{e}_j=\delta_{ij}.
$$

Esta idea sera esencial cuando pasemos desde coordenadas cartesianas a coordenadas polares, cilindricas o esfericas, y tambien cuando estudiemos marcos no inerciales.

## Producto punto y producto cruz

Para dos vectores $\boldsymbol{a}$ y $\boldsymbol{b}$:

$$
\boldsymbol{a}\cdot\boldsymbol{b}=|\boldsymbol{a}|\,|\boldsymbol{b}|\cos\theta,
$$

de modo que el **producto punto** entrega un escalar. Se usa, por ejemplo, en trabajo mecanico, proyecciones y calculo de normas.

El **producto cruz** produce un vector perpendicular al plano definido por ambos vectores:

$$
\boldsymbol{a}\times\boldsymbol{b}.
$$

En mecanica aparece de manera natural en el torque y en el momentum angular.

## Derivacion vectorial y operadores diferenciales

Si la posicion depende del tiempo, entonces

$$
\boldsymbol{v}=\frac{d\boldsymbol{r}}{dt},
\qquad
\boldsymbol{a}=\frac{d\boldsymbol{v}}{dt}.
$$

Cuando una magnitud depende del espacio, entran en juego operadores diferenciales basicos:

- **gradiente**: describe como cambia un campo escalar en el espacio,
- **divergencia**: mide fuentes o sumideros de un campo vectorial,
- **rotacional**: cuantifica la tendencia local a rotar,
- **laplaciano**: aparece en ecuaciones diferenciales de amplio uso en fisica.

Aunque estas herramientas se estudian con mas detalle en otros cursos, aqui conviene reconocerlas desde el comienzo porque reaparecen en fuerzas centrales, potenciales y formulaciones mas avanzadas.

## Matrices y rotaciones

Las matrices permiten formalizar cambios de base y rotaciones. En particular, una rotacion conserva longitudes y angulos, de modo que cambia la representacion de un vector sin alterar su norma.

Esta idea anticipa varios temas del curso:

- descripcion del movimiento en distintos sistemas de referencia,
- analisis de simetrias,
- y formulacion mas compacta de relaciones fisicas.

## Como usar este material dentro del curso

Se recomienda leer esta pagina antes de entrar al bloque principal de contenidos y volver a ella cuando aparezcan dificultades con:

- representacion de vectores,
- productos vectoriales y escalares,
- eleccion de coordenadas,
- operadores diferenciales,
- o cambios de base y rotaciones.

Para continuar con la dimension computacional del curso, revisa [Modelacion numerica en mecanica](../mechanics/modelacion_numerica.md).
