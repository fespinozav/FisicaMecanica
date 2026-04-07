# Fisica Mecanica, Universidad Tecnologica Metropolitana, 2026

Jupyter Book del curso: [https://fespinozav.github.io/FisicaMecanica/](https://fespinozav.github.io/FisicaMecanica/)

Este repositorio contiene el material principal del curso de **Fisica Mecanica**. Aqui se organiza el ebook del curso, la programacion oficial, las unidades de catedra, las guias de trabajo y los notebooks de apoyo adaptados desde `PHY321`.

El trabajo del curso se apoya en dos espacios principales:

- el repositorio GitHub: [fespinozav/FisicaMecanica](https://github.com/fespinozav/FisicaMecanica)
- el Jupyter Book del curso: [https://fespinozav.github.io/FisicaMecanica/](https://fespinozav.github.io/FisicaMecanica/)

Aqui encontraras una vista general del curso, con recursos, evaluacion, materiales y resultados de aprendizaje.

## Recursos principales del curso

| Recurso | Enlace | Uso principal |
| --- | --- | --- |
| Jupyter Book | [Abrir book](https://fespinozav.github.io/FisicaMecanica/) | Recorrido principal del curso y lectura de capitulos |
| Repositorio GitHub | [Abrir repo](https://github.com/fespinozav/FisicaMecanica) | Archivos fuente, versionado y materiales descargables |
| Programacion oficial | [Programacion oficial del curso](contents/phy321/schedule.md) | Fechas y ponderaciones oficiales |
| Unidad 0 | [Unidad 0](contents/utem/unidad0.md) | Presentacion, reglamentos y politicas |
| Unidades locales | [Unidad 1](contents/utem/unidad1.md) | Inicio del trabajo tematico del curso |

## Equipo docente, evaluacion y aspectos practicos

| Componente | Descripcion |
| --- | --- |
| Curso | Fisica Mecanica |
| Institucion | Universidad Tecnologica Metropolitana |
| Modalidad del repositorio | Ebook del curso, materiales descargables y notebooks |
| Material base | Unidades locales, guias de trabajo y adaptacion de `PHY321` |

## Evaluacion y fechas oficiales

La evaluacion oficial del curso se organiza de la siguiente manera:

| Actividad | Sigla | Ponderacion | Fecha oficial |
| --- | --- | --- | --- |
| Control 1 | C1 | 20% | Semana del 20 al 26 de abril de 2026 |
| Prueba 1 | P1 | 30% | Viernes 15 de mayo de 2026 |
| Semana de autoaprendizaje | - | - | Del 18 al 24 de mayo de 2026 |
| Control 2 | C2 | 20% | Semana del 8 al 14 de junio de 2026 |
| Prueba 2 | P2 | 30% | Viernes 3 de julio de 2026 |
| Prueba recuperativa | - | - | Viernes 10 de julio de 2026 |
| Termino de clases | - | - | Viernes 17 de julio de 2026 |
| Examen | - | - | Viernes 24 de julio de 2026 |

Para el trabajo semanal dentro del repositorio, conviene combinar:

- lectura del Jupyter Book,
- revision de las unidades locales,
- resolucion de guias,
- y desarrollo de notebooks y tareas cuando corresponda.

## Textos y materiales de apoyo

Los materiales principales del curso se articulan en cuatro capas:

- material docente local del curso, incluyendo unidad 0, programacion, unidades 1 a 3 y guias de trabajo;
- ebook del curso en GitHub Pages, con navegacion por capitulos y material complementario;
- material base adaptado desde `PHY321`;
- y bibliografia de apoyo para profundizacion conceptual.

### Referencias base en APA

- Hjorth-Jensen, M., & Pratt, S. (2023). *PHY321, Classical Mechanics I* [Repositorio de curso y Jupyter Book]. GitHub. https://github.com/mhjensen/Physics321
- Espinoza Vidal, F. (2026). *Programacion Mecanica Clasica* [Programacion de asignatura]. Universidad Tecnologica Metropolitana.
- Espinoza Vidal, F., adaptado de Amigo, N. (2026). *Mecanica Clasica: Unidades 1 a 3 y material de apertura del curso* [Presentaciones y documentos docentes]. Universidad Tecnologica Metropolitana.
- Universidad Tecnologica Metropolitana, Departamento de Fisica. (2026). *Guias 1 a 8 de Mecanica Clasica* [Guias de ejercitacion]. Universidad Tecnologica Metropolitana.
- Serway, R. A., & Jewett, J. W., Jr. (2018). *Fisica para ciencias e ingenieria* (Vol. 1, 10a ed.). Cengage Learning.
- Taylor, J. R. (2005). *Classical mechanics*. University Science Books.
- Malthe-Sorenssen, A. (2015). *Elementary mechanics using Python: A modern course combining analytical and numerical techniques*. Springer.

## Estructura del repositorio

Dentro del book y del repositorio, el recorrido principal queda organizado asi:

- [Introduccion y objetivos del curso](contents/phy321/intro.md)
- [Unidad 0: presentacion, reglamentos y politicas](contents/utem/unidad0.md)
- [Fundamentos previos: vectores, coordenadas y operadores basicos](contents/phy321/fundamentos_previos.md)
- [Programacion oficial del curso](contents/phy321/schedule.md)
- [Serway y Jewett como apoyo bibliografico](contents/phy321/serway_apoyo.md)
- [Criterios editoriales y uso de materiales](contents/phy321/source_attribution.md)

El bloque de contenidos principales del ebook cubre:

- fundamentos matematicos y numericos para mecanica clasica,
- movimiento y leyes de Newton,
- trabajo, energia, momentum y conservacion,
- oscilaciones armonicas,
- problemas de dos cuerpos,
- marcos no inerciales,
- y formulacion lagrangiana.

## Resultados de aprendizaje

Al finalizar el curso, se espera que puedas:

- analizar fuerzas e interacciones y formular ecuaciones de movimiento con base en las leyes de Newton;
- resolver problemas de trabajo, energia, momentum lineal y momentum angular;
- interpretar oscilaciones, problemas de dos cuerpos y marcos no inerciales;
- usar herramientas numericas para estudiar sistemas mecanicos;
- y documentar soluciones con claridad conceptual, matematica y computacional.

## Nota de procedencia y uso de materiales

Parte importante del material de este repositorio fue adaptada desde `PHY321`. El contenido local del curso se integra con esa estructura para construir una version en espanol y alineada con la programacion oficial.

El material docente propio puede reorganizarse y adaptarse libremente dentro del repositorio. Los textos externos de apoyo se usan como referencia conceptual y bibliografica, sin redistribuir material protegido por copyright. El detalle editorial puede revisarse en [Criterios editoriales y uso de materiales](contents/phy321/source_attribution.md).

## Compilacion local

Para compilar este libro:

1. Crear un entorno virtual de Python.
2. Instalar dependencias con `pip install -r requirements.txt`.
3. Ejecutar `jupyter-book build .`.
4. Revisar la salida generada en `_build/html/`.
