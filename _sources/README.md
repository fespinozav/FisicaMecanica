# Bienvenida al curso de Fisica Mecanica

Este libro acompana un curso introductorio de mecanica clasica. Su proposito es ayudar a construir intuicion fisica, desarrollar una estrategia ordenada de resolucion de problemas y conectar los modelos teoricos con situaciones reales mediante calculo, representaciones graficas y actividades de apoyo con Python cuando aporte claridad.

Aqui encontraras contenidos organizados por unidades, preguntas guia, relaciones matematicas esenciales y una ruta de trabajo pensada para avanzar de manera gradual desde la descripcion del movimiento hasta el estudio de sistemas rotacionales, oscilatorios y gravitacionales.

## Proposito formativo

Al finalizar el curso, se espera que puedas:

- Identificar las magnitudes fisicas relevantes de un problema mecanico.
- Representar sistemas mediante diagramas, ecuaciones y modelos simplificados.
- Aplicar principios de cinematica, dinamica y conservacion en problemas de complejidad creciente.
- Justificar cada paso de una solucion con criterio fisico y consistencia matematica.
- Usar herramientas computacionales como apoyo para visualizar, explorar y comunicar resultados.

## Como trabajar en este libro

1. Revisa cada unidad en el orden sugerido por la navegacion.
1. Estudia primero los conceptos y ecuaciones clave antes de resolver ejercicios.
1. Usa las preguntas guia de cada capitulo para verificar comprension.
1. Contrasta procedimientos algebraicos con interpretaciones fisicas y graficas.
1. Vuelve sobre los temas anteriores cuando una unidad nueva los requiera.

## Ruta del curso

El desarrollo del curso sigue esta progresion:

- Fundamentos: [Introduccion a la Fisica Mecanica](contents/mechanics/intro.md) y [Magnitudes, Unidades y Vectores](contents/mechanics/units_vectors.md)
- Cinematica: [Cinematica en Una Dimension](contents/mechanics/kinematics_1d.md) y [Cinematica en Dos Dimensiones](contents/mechanics/kinematics_2d.md)
- Dinamica: [Leyes de Newton](contents/mechanics/newton_laws.md)
- Conservacion: [Trabajo y Energia](contents/mechanics/work_energy.md) y [Momentum Lineal y Colisiones](contents/mechanics/momentum_collisions.md)
- Sistemas extendidos: [Rotacion de Cuerpos Rigidos](contents/mechanics/rotation.md), [Oscilaciones](contents/mechanics/oscillations.md) y [Gravitacion](contents/mechanics/gravitation.md)

## Programacion general del curso

La siguiente planificacion distribuye el recorrido del curso en 12 semanas y puede reutilizarse en distintos periodos academicos sin depender de fechas especificas.

| Semana | Tema central | Enfoque de trabajo |
| --- | --- | --- |
| 1 | Introduccion al curso y herramientas basicas | Presentacion del enfoque de mecanica, magnitudes fisicas, sistema internacional y analisis dimensional |
| 2 | Vectores y modelacion | Operaciones vectoriales, componentes cartesianas y lectura fisica de diagramas |
| 3 | Cinematica en una dimension | Posicion, velocidad, aceleracion y movimiento con aceleracion constante |
| 4 | Cinematica en dos dimensiones | Movimiento de proyectiles, descripcion vectorial y trayectorias planas |
| 5 | Leyes de Newton I | Diagramas de cuerpo libre, fuerza neta y primera aproximacion a la dinamica |
| 6 | Leyes de Newton II | Rozamiento, tensiones, planos inclinados y sistemas conectados |
| 7 | Trabajo y energia | Trabajo de fuerzas, energia cinetica, energia potencial y conservacion |
| 8 | Momentum lineal y colisiones | Impulso, conservacion del momentum y analisis de choques |
| 9 | Rotacion I | Variables angulares, torque y analogias entre traslacion y rotacion |
| 10 | Rotacion II | Momento de inercia, energia rotacional y momentum angular |
| 11 | Oscilaciones mecanicas | Movimiento armonico simple, energia oscilatoria y sistemas masa-resorte |
| 12 | Gravitacion y cierre integrador | Ley de gravitacion universal, orbitas y sintesis de modelos del curso |

## Bibliografia base

1. John R. Taylor, *Classical Mechanics*
1. David Halliday, Robert Resnick, Jearl Walker, *Fundamentals of Physics*
1. Daniel Kleppner y Robert Kolenkow, *An Introduction to Mechanics*
1. Hugh D. Young y Roger A. Freedman, *University Physics*

## Desarrollo del libro

Este repositorio esta construido con [Jupyter Book](https://jupyterbook.org/en/stable/intro.html) y puede seguir creciendo con apuntes, guias, ejercicios resueltos y actividades computacionales dentro de `contents/mechanics/`.

Para compilar el libro de manera local:

1. Crear un entorno virtual de Python.
1. Instalar dependencias con `pip install -r requirements.txt`.
1. Ejecutar `jupyter-book build .`.
1. Revisar la salida generada en `_build/html/`.
