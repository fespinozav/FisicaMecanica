# Marcos no inerciales

No todos los sistemas de referencia son equivalentes para aplicar directamente las leyes de Newton. Cuando el observador acelera o rota, aparecen terminos adicionales que permiten describir el movimiento desde ese marco.

## Objetivos de aprendizaje

- Distinguir entre marcos inerciales y no inerciales.
- Identificar fuerzas ficticias asociadas a traslaciones aceleradas y rotaciones.
- Analizar movimiento observado desde plataformas giratorias.
- Relacionar descripcion matematica y significado fisico de cada termino.

## Marcos inerciales

En un marco inercial se cumple la forma habitual de la segunda ley:

```{math}
\sum \vec{F}=m\vec{a}
```

Si el sistema de referencia acelera respecto de un marco inercial, esa expresion necesita correcciones.

## Traslaciones aceleradas

Si el observador se mueve con aceleracion `\vec{A}` respecto de un marco inercial, en el nuevo marco aparece una fuerza inercial efectiva:

```{math}
\vec{F}_{\mathrm{inercial}}=-m\vec{A}
```

Esta fuerza no corresponde a una interaccion fisica nueva, sino al cambio de sistema de referencia.

## Sistemas rotantes

Cuando el marco gira con velocidad angular `\vec{\Omega}`, la aceleracion observada incorpora terminos adicionales. Dos de los mas importantes son:

### Fuerza centrifuga

```{math}
\vec{F}_{\mathrm{centrifuga}}=-m\vec{\Omega}\times(\vec{\Omega}\times\vec{r})
```

### Fuerza de Coriolis

```{math}
\vec{F}_{\mathrm{Coriolis}}=-2m\vec{\Omega}\times\vec{v}_{\mathrm{rel}}
```

La primera depende de la posicion y la segunda de la velocidad relativa dentro del marco giratorio.

## Ejemplos fisicos

- Desvio aparente de masas de aire en la atmosfera terrestre.
- Analisis de objetos sobre una plataforma en rotacion.
- Estudio cualitativo del pendulo de Foucault.
- Movimiento observado desde un vehiculo que acelera.

## Ideas clave

- Las fuerzas ficticias no se dibujan en un diagrama de cuerpo libre dentro de un marco inercial.
- En un marco no inercial se introducen para recuperar una forma util de las ecuaciones de movimiento.
- La eleccion del sistema de referencia influye en la descripcion matematica, no en la fisica del fenomeno.

## Preguntas para estudiar

1. Que cambia si se describe el problema desde el suelo o desde una plataforma giratoria.
1. En que situaciones conviene usar un marco no inercial.
1. Como distinguir una fuerza real de un termino inercial.
