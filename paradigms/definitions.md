# Paradigmas de Programación

Son una manera o estilo de programación de software. Existen diferentes formas de diseñar un lenguaje de programación y varios modos de trabajar para obtener los resultados que se necesitan.

Se denominan paradigmas de programación a las formas de clasificar los lenguajes de programación en función de sus características. Algunos paradigmas se ocupan principalmente de las implicancias para el modelo de ejecución del lenguaje, como permitir efectos secundarios o si la secuencia de operaciones está definida por el modelo de ejecución. Otros paradigmas se refieren principalmente a la forma en que se organiza el código, como agrupar un código en unidades junto con el estado que modifica el código. Otros se preocupan principalmente por el estilo de la sintaxis y la gramática.

**Los paradigmas de programación comunes incluyen:**

* **Paradigma imperativo.** Tiene dos características principales, establece el orden en el que ocurren las operaciones, con construcciones que controlan explícitamente ese orden, y permiten efectos secundarios, en los que el estado puede modificarse en un momento determinado, dentro de una unidad de código, y luego leer en un momento diferente dentro de una unidad de código diferente. La comunicación entre las unidades de código no es explícita. 

* **Paradigma orientada a objetos.** El código se organiza en objetos que contienen un estado que solo es modificado por el código que forma parte del objeto. La mayoría de los lenguajes orientados a objetos también son lenguajes imperativos. 

* **Paradigma declarativo.** No indican el orden en el que ejecutar las operaciones. En su lugar, proporcionan una serie de operaciones disponibles en el sistema, junto con las condiciones en las que se permite que se ejecute cada una. La implementación del modelo de ejecución del lenguaje rastrea qué operaciones son libres de ejecutar y elige el orden en forma independiente.

## Principales Paradigmas

### Programación Estructurada

Su premisa consiste en evitar el uso de "goto" para seguir una serie de instrucciones en secuencia. Utiliza estructuras de control, entradas/salidas, manejo de errores, excepciones y estructuras de datos.

**Lenguajes que lo implementan:**

* Fortran
* Pascal
* Cobol
* Ada
* C

### Programación Procedural

Su premisa consiste en que el código se agrupa en procedimientos a través de un sistema de pilas. El programa se compone de procedimientos los cuales interactúan entre sí.

* Fortran
* ALGOL
* COBOL
* Basic

### Programación Orientada a Objetos

Su premisa consiste en que los objetos de la vida real pueden ser representados en código, con sus características y comportamientos. Los objetos son un molde para crear instancias con cualidades y comportamientos únicos o compartidos.

* Simula
* Java
* C++
* Python
* PHP

### Programación Funcional

Su premisa consiste en que las funciones son ciudadanos de primera clase y busca reducir los efectos colaterales. La recursividad y funciones de alto orden son prioridad para resolver problemas.

* Lisp
* Scheme
* Clojure
* Erlang
* Haskell
* F#

### Programación Lógica

Su premisa consiste en expresar los objetivos como reglas acerca de los resultados en lógica matemática. Hace uso de cláusulas de Horn para evaluar predicados y definir si son verdaderos o falsos.

* Prolog
* ALF
* Fril
* Visual Prolog
* Mercury

### Programación Dirigida por Eventos

Su premisa consiste en no controlar la secuencia de ejecuciones, sino que reacciona a sucessos ocurridos. Son programas que corren indefinidamente, cambiando su estado según los eventos que detecta.

* Java
* JavaScript
* C#
* Python