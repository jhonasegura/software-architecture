# ¿Qué es una funcupon recursiva?

Es aquella que para cumplir su función requiere invocarse a si misma

## ¿Cuáles son las cnsideraciones a tomar en cuenta en un algoritmo recursivo?

* Siempre agregar una condición que termine el ciclo de ejecución.

* Un algoritmo recursivo debe cambiar su estado, en dirección a cumplir la condición de finalización.

* La función debe ser capaz de llamarse a si misma cuando lo requiera.

La velocidad de un algoritmo recursivo es mas lenta debido a que los métodos se van apilando dentro de la pila del sistema. Se recomienda siempre utilizar un loop de ser posible para realizar la misma tarea y evitar el stack overhead (sobrecarga de la pila) que se produce cuando el sistema no tiene mas memoria disponible.

Si no se construye bien el algoritmo y nunca se cumple la condición de finalización, la ejecución del programa consumirá la memoria del sistema.

