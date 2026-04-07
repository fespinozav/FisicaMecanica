# Bienvenida al curso de Fisica Mecanica

Este libro organiza el curso de Fisica Mecanica siguiendo, de manera adaptada, la estructura de **PHY321: Classical Mechanics I**. La adaptacion busca conservar la progresion tematica fuerte del curso original y presentarla como un ebook reutilizable para distintos anos academicos.

## Nota de procedencia

Parte importante del material de este libro fue adaptada a partir del repositorio de curso de Hjorth-Jensen y Pratt. Para evitar plagio y mantener trazabilidad academica, el libro incluye atribucion explicita en las paginas editoriales y en cada notebook importado.

**Referencia APA del material fuente principal:** Hjorth-Jensen, M., & Pratt, S. (2023). *PHY321, Classical Mechanics I* [Repositorio de curso y Jupyter Book]. GitHub. https://github.com/mhjensen/Physics321

La licencia del material fuente es **CC0 1.0 Universal**. Puedes revisar el detalle en [Fuente y licencia](contents/phy321/source_attribution.md).

## Proposito formativo

Al finalizar el curso, se espera que puedas:

- Analizar fuerzas e interacciones y formular ecuaciones de movimiento con base en las leyes de Newton.
- Resolver problemas de trabajo, energia, momentum lineal y momentum angular.
- Interpretar sistemas oscilatorios, problemas de dos cuerpos, marcos no inerciales y formulaciones lagrangianas.
- Combinar modelacion analitica con herramientas numericas para estudiar sistemas mecanicos.
- Documentar soluciones con claridad conceptual, matematica y computacional.

## Como esta organizado el libro

El recorrido principal del ebook sigue esta ruta:

- [Introduccion y objetivos del curso](contents/phy321/intro.md)
- [Fundamentos previos: vectores, coordenadas y operadores basicos](contents/phy321/fundamentos_previos.md)
- [Programacion general por semanas](contents/phy321/schedule.md)
- [Equipo docente y evaluacion sugerida](contents/phy321/teachers.md)
- [Textos y referencias en formato APA](contents/phy321/textbooks.md)
- [Fuente, licencia y criterio de adaptacion](contents/phy321/source_attribution.md)

Despues del bloque inicial, el libro se divide en dos grandes tramos:

- Material introductorio: una pagina preliminar sobre vectores, coordenadas y operadores basicos, seguida de capitulos sobre fundamentos matematicos, movimiento, leyes de Newton, trabajo, energia y leyes de conservacion.
- Temas avanzados: oscilaciones, problemas de dos cuerpos, marcos no inerciales y formulacion lagrangiana.

Tambien se incluyen notebooks de tareas y un proyecto parcial heredados del curso fuente para ampliar el trabajo guiado.

## Programacion general del curso

La siguiente programacion conserva la secuencia conceptual de PHY321, pero se presenta sin fechas de calendario para que pueda reutilizarse en otros periodos academicos.

| Semana | Tema central | Enfoque de trabajo |
| --- | --- | --- |
| 1 | Introduccion, vectores y herramientas de trabajo | Espacio, tiempo, movimiento, repaso matematico y organizacion computacional del curso |
| 2 | Fundamentos matematicos y numericos | Coordenadas, vectores, algebra vectorial y apoyo numerico para mecanica |
| 3 | Movimiento y leyes de Newton | Problemas simples de movimiento, fuerzas y ecuaciones de movimiento |
| 4 | Modelos de fuerza y trabajo | Fuerza gravitatoria, fuerza elastica, trabajo mecanico y energia |
| 5 | Conservacion y momentum | Energia, momentum lineal, momentum angular y leyes de conservacion |
| 6 | Potenciales y oscilaciones armonicas | Fuerzas conservativas, equilibrio y oscilador armonico |
| 7 | Oscilaciones amortiguadas y forzadas | Resonancia, modelacion numerica y lectura fisica de soluciones |
| 8 | Problema de dos cuerpos | Centro de masa, coordenadas relativas y formulacion gravitatoria |
| 9 | Orbitas y leyes de Kepler | Fuerzas centrales, orbitas elipticas y clasificacion de trayectorias |
| 10 | Marcos no inerciales | Traslaciones aceleradas, sistemas rotantes y fuerza de Coriolis |
| 11 | Calculo variacional y formulacion lagrangiana | Principio variacional, restricciones y ecuaciones de Euler-Lagrange |
| 12 | Integracion y proyectos | Sintesis de contenidos, trabajo aplicado y cierre del curso |

## Compilacion local

Para compilar este libro:

1. Crear un entorno virtual de Python.
1. Instalar dependencias con `pip install -r requirements.txt`.
1. Ejecutar `jupyter-book build .`.
1. Revisar la salida generada en `_build/html/`.
