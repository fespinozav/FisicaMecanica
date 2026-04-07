# Oscilaciones

Muchos sistemas mecanicos cercanos al equilibrio exhiben oscilaciones. El oscilador armonico simple es uno de los modelos mas importantes de toda la fisica.

## Objetivos de aprendizaje

- Modelar oscilaciones alrededor de un equilibrio estable.
- Resolver el movimiento armonico simple.
- Relacionar energia, fase, frecuencia y periodo.
- Reconocer el efecto del amortiguamiento y del forzamiento externo.

## Oscilador armonico simple

```{math}
F = -k x
```

```{math}
m \ddot{x} + kx = 0
```

```{math}
x(t) = A \cos(\omega t + \phi), \qquad \omega = \sqrt{\frac{k}{m}}
```

## Energia

```{math}
E = \frac{1}{2} m v^2 + \frac{1}{2} k x^2
```

## Extensiones

- Pendulo simple para angulos pequenos.
- Oscilaciones amortiguadas.
- Resonancia y respuesta forzada.
- Superposicion y descomposicion en modos.
- Fuerzas periodicas y analisis cualitativo de resonancias.

## Amortiguamiento y forzamiento

Una forma clasica de extender el modelo es

```{math}
m\ddot{x}+b\dot{x}+kx=F_0\cos(\omega t)
```

Aqui aparecen tres ideas que conviene distinguir:

- el amortiguamiento reduce la amplitud con el tiempo;
- el forzamiento externo alimenta el sistema;
- y la resonancia ocurre cuando la frecuencia de excitacion se acerca a la frecuencia natural.

## Preguntas de analisis

1. Como cambia el periodo cuando varia `m` o `k`.
1. Que informacion aporta la energia total en un oscilador sin roce.
1. Por que un algoritmo numerico mal elegido puede deformar artificialmente la amplitud.

## Problemas tipo

1. Sistema masa-resorte.
1. Periodo de un pendulo simple.
1. Comparacion entre frecuencia angular y frecuencia ordinaria.
