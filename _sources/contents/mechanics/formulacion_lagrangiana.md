# Formulacion lagrangiana

La formulacion lagrangiana reorganiza la mecanica clasica a partir de energia y coordenadas generalizadas. Su valor principal es ofrecer una ruta compacta para derivar ecuaciones de movimiento, especialmente en sistemas con restricciones.

## Objetivos de aprendizaje

- Comprender la idea de accion y principio variacional.
- Construir un lagrangiano para sistemas mecanicos simples.
- Derivar ecuaciones de Euler-Lagrange.
- Reconocer ventajas de este enfoque frente a la formulacion newtoniana.

## Del principio de accion al lagrangiano

Se define la accion como

```{math}
S=\int_{t_1}^{t_2} L(q_i,\dot{q}_i,t)\,dt
```

donde `L` es el lagrangiano y, en muchos problemas mecanicos,

```{math}
L = T-U
```

con `T` energia cinetica y `U` energia potencial.

## Ecuaciones de Euler-Lagrange

La condicion de estacionariedad de la accion conduce a

```{math}
\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{q}_i}\right)-\frac{\partial L}{\partial q_i}=0
```

Estas ecuaciones permiten trabajar con coordenadas generalizadas como angulos, distancias curvilineas o variables ligadas por restricciones.

## Ejemplos clasicos

### Particula libre

Si `U=0`, entonces

```{math}
L=\frac{1}{2}m\dot{x}^2
```

y la ecuacion de movimiento recupera aceleracion nula.

### Pendulo simple

Usando el angulo `\theta` como coordenada:

```{math}
L=\frac{1}{2}m\ell^2\dot{\theta}^2-mg\ell(1-\cos\theta)
```

De aqui se obtiene la ecuacion no lineal del pendulo.

## Por que esta formulacion es potente

- Maneja restricciones de forma natural.
- Aprovecha mejor las simetrias del sistema.
- Se adapta con facilidad a coordenadas no cartesianas.
- Sirve de puente hacia mecanica analitica, teoria de campos y fisica moderna.

## Conexion con conservacion

Cuando el lagrangiano no depende explicitamente de cierta coordenada, aparece una cantidad conservada asociada. Esta relacion entre simetrias y conservacion ordena de manera elegante muchos problemas del curso.

## Sugerencias de estudio

1. Comparar una derivacion newtoniana y una lagrangiana del mismo sistema.
1. Identificar coordenadas generalizadas convenientes antes de escribir ecuaciones.
1. Verificar que el resultado final conserva el significado fisico del problema.
