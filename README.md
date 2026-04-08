# Fisica Mecanica

Este repositorio contiene el material principal del curso de **Fisica Mecanica**. Aqui se organiza el ebook del curso, la programacion oficial, las unidades de catedra, las guias de trabajo y los notebooks de apoyo.

El trabajo del curso se apoya en dos espacios principales:

- Repositorio GitHub: [fespinozav/FisicaMecanica](https://github.com/fespinozav/FisicaMecanica)
- Jupyter Book del curso: [https://fespinozav.github.io/FisicaMecanica/](https://fespinozav.github.io/FisicaMecanica/)

Aqui encontraras una vista general del curso, con recursos, evaluacion, materiales y resultados de aprendizaje.

## Evaluacion y aspectos practicos

| Componente | Descripcion |
| --- | --- |
| Curso | FISB4020/541 |
| Institucion | Universidad Tecnologica Metropolitana |
| Modalidad del repositorio | Ebook del curso, materiales descargables y notebooks |
| Material base | Unidades locales, guias de trabajo |

## Evaluaciones primer semestre de 2026
### FÍSICA MECÁNICA COD:FISB4020/541

La evaluacion oficial del curso se organiza de la siguiente manera:

| Actividad | Sigla | Ponderacion | Fecha |
| --- | --- | --- | --- |
| Control 1 | C1 | 20% | Semana del 20 al 26 de abril de 2026 |
| Prueba 1 | P1 | 30% | Viernes 15 de mayo de 2026 |
| Semana de autoaprendizaje | - | - | Del 18 al 24 de mayo de 2026 |
| Control 2 | C2 | 20% | Semana del 8 al 14 de junio de 2026 |
| Prueba 2 | P2 | 30% | Viernes 3 de julio de 2026 |
| Prueba recuperativa | - | - | Viernes 10 de julio de 2026 |
| Termino de clases | - | - | Viernes 17 de julio de 2026 |
| Examen | - | 40% | Viernes 24 de julio de 2026 |

Para el trabajo semanal dentro del repositorio, conviene combinar:

- Lectura del Jupyter Book,
- Revision de apuntes del profesor y en clases,
- Resolucion de guias,
- Desarrollo de notebooks y tareas cuando corresponda.

## Textos y materiales de apoyo

Los materiales principales del curso se articulan en cuatro capas:

- Material docente local del curso, programacion, unidades 1 a 8 y guias de trabajo.
- Ebook del curso en GitHub Pages, con navegacion por capitulos y material complementario.
- Bibliografia de apoyo para profundizacion conceptual.

### Referencias base

- Universidad Tecnologica Metropolitana, Departamento de Fisica. (2026). *Guias 1 a 8 de Mecanica Clasica* [Guias de ejercitacion]. Universidad Tecnologica Metropolitana.
- Serway, Raymond A. (2004). Física. Tomo I, Madrid, España: Mc Graw Hill.
- Tipler Paul A.(1999). Física. Volumen I. Barcelona, España: Reverte. +
- Alonso & Finn. (1992). Física. Volumen I, México: Fondo Educacional Internacional
- Malthe-Sorenssen, A. (2015). *Elementary mechanics using Python: A modern course combining analytical and numerical techniques*. Springer.

## Estructura del repositorio

Dentro del book y del repositorio, el recorrido principal queda organizado asi:

- [Introduccion y objetivos del curso](contents/phy321/intro.md)
- [Programacion oficial del curso](contents/phy321/schedule.md)
- [Fundamentos previos: vectores, coordenadas y operadores basicos](contents/phy321/fundamentos_previos.md)
- [Unidad 0: Presentacion, reglamentos y politicas](contents/utem/unidad0.md)
- [Unidad 1: Sistema de unidades, magnitudes y vectores](contents/utem/unidad1.md)
- [Unidad 2: Cinemática de la partícula en una dimensión](contents/utem/unidad2.md)
- [Unidad 3: Cinemática bidimensional de la partícula](contents/utem/unidad3.md)
- [Unidad 4: Dinámica de la partícula](contents/utem/unidad4.md)
- [Unidad 5: Trabajo y energía mecánica](contents/utem/unidad5.md)
- [Unidad 6: Dinámica de un sistema de partículas](contents/utem/unidad6.md)
- [Unidad 7: Impulso y momento lineal](contents/utem/unidad7.md)
- [Unidad 8: Estática del sólido rígido](contents/utem/unidad8.md)
- [Anexo 1: Serway y Jewett como apoyo bibliografico](contents/phy321/serway_apoyo.md)
- [Anexo 2: Criterios editoriales y uso de materiales](contents/phy321/source_attribution.md)
- [Anexo 3: Mecánica elemental con Python](contents/utem/mechpython)

El bloque de contenidos principales del ebook cubre:

- fundamentos matematicos y numericos para mecanica clasica,
- Movimiento y leyes de Newton,
- Trabajo, energia, momentum y conservacion,
- Oscilaciones armonicas,
- Problemas de dos cuerpos,
- Marcos no inerciales,
- Formulacion lagrangiana.

## Resultados de aprendizaje

Al finalizar el curso, se espera que puedas:

- Analizar fuerzas e interacciones y formular ecuaciones de movimiento con base en las leyes de Newton;
- resolver problemas de trabajo, energia, momentum lineal y momentum angular;
- Interpretar oscilaciones, problemas de dos cuerpos y marcos no inerciales;
- Usar herramientas numericas para estudiar sistemas mecanicos;
- Documentar soluciones con claridad conceptual, matematica y computacional.

## Nota de procedencia y uso de materiales

El material docente propio puede reorganizarse y adaptarse libremente dentro del repositorio. Los textos externos de apoyo se usan como referencia conceptual y bibliografica, sin redistribuir material protegido por copyright.

## Compilacion local

Para compilar este libro:

1. Crear un entorno virtual de Python.
2. Instalar dependencias con `pip install -r requirements.txt`.
3. Ejecutar `jupyter-book build .`.
4. Revisar la salida generada en `_build/html/`.
