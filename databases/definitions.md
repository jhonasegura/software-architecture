# Bases de Datos

## Bases de Datos OLTP

Son bases de datos orientadas al procesamiento de transacciones. Una transacción genera un proceso atómico que debe ser validado con un commit o invalidado con un rollback y que puede involucrar operaciones de inserción, modificación y borrado de datos. Es típico de los datamarts.

## Bases de Datos OLAP

Es una tecnología de bases de datos que se ha optimizado para consultas e informes, en lugar de procesar transacciones.

## Bases de Datos NoSQL

Tienen 4 grandes familias: Key Value Stores, basadas en grafos, columnares y basadas en documentos.

**Key Value Stores**: Guardan la información en formato de llaves y valores. Son usadas para guardar cache, información de sesión de los usuarios o cosas muy sencillas. Son muy rápidas de consultar pero no se pueden usar en casos más complejos donde se necesite de estructuras más especiales. El mejor ejemplo de estas bases de datos es Redis.

![key-value-stores](/pictures/key-value-stores.PNG)

**Graph Databases**: Bases de datos basadas en grafos. Nos permiten establecer conexiones entre nuestras entidades para realizar consultas de una forma más eficiente que en bases de datos relacionales. Por ejemplo: Neo4j o JanusGraph.

![graph-databases](/pictures/graph-databases.PNG)

**Wide-column Stores**: Bases de datos columnares. Tienen una llave de fila y otra de columnas para hacer consultas muy rápidas y guardar grandes cantidades de información pero modelar los datos se puede volver un poco complicado. Son usadas en Big Data, IoT, sistemas de recomendaciones, entre otras. Por ejemplo: Cassandra o HBase.

![wide-column-stores](/pictures/wide-column-stores.PNG)

**Document Databases**: Bases de datos basadas en documentos. Nos permiten guardar documentos dentro de colecciones, tienen muy buena performance y flexibilidad que nos permite modelar casos de la vida real de forma sencilla y efectiva. Por ejemplo: MongoDB o CouchBase.

![document-databases](/pictures/document-databases.PNG)

**Casos de Uso para cada tipo:**

![databases-resume](/pictures/databases-resume.PNG)

## MongoDB

Es una base de datos de código abierto No Relacional basada en documentos que nos permite guardar una gran cantidad de documentos de forma distribuida.

Una de sus principales características es que nos permite guardar nuestras estructuras o documentos en un formato muy parecido a JSON para tener una gran flexibilidad a la hora de modelar situaciones de la vida real.

Por ser una base de datos distribuida, se puede hablar de varios servidores o como se conoce con el nombre de Cluster de MongoDB. Gracias a esto se obtiene una gran escalabilidad de forma horizontal.

MongoDB es "Schema Less" lo que permite que los documentos tengan estructuras diferentes sin afectar su funcionamiento, algo que no se puede hacer con las tablas de las bases de datos relacionales. Su lenguaje para realizar queries, índices y agregaciones es muy expresivo.