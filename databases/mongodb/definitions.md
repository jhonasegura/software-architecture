# MongoDB

Es una base de datos de código abierto No Relacional basada en documentos que nos permite guardar una gran cantidad de documentos de forma distribuida.

Una de sus principales características es que nos permite guardar nuestras estructuras o documentos en un formato muy parecido a JSON para tener una gran flexibilidad a la hora de modelar situaciones de la vida real.

Por ser una base de datos distribuida, se puede hablar de varios servidores o como se conoce con el nombre de Cluster de MongoDB. Gracias a esto se obtiene una gran escalabilidad de forma horizontal.

![mongodb-structure](/pictures/mongodb-structure.PNG)

MongoDB es "Schema Less" lo que permite que los documentos tengan estructuras diferentes sin afectar su funcionamiento, algo que no se puede hacer con las tablas de las bases de datos relacionales. Su lenguaje para realizar queries, índices y agregaciones es muy expresivo.

![mongodb-queries](/pictures/mongodb-queries.PNG)

Entre los proveedores que permiten utilizar o alquilar MongoDB como servicio está MongoDB Atlas, los cuales son los mismos desarrolladores de MongoDB.

Entre sus características está:

* Aprovisionamiento automático de clusters con MongoDB.
* Alta disponibilidad.
* Altamente escalable.
* Seguro.
* Disponible en AWS, GCP y Microsoft Azure.
* Fácil monitoreo y optimización.

![arquitectura-mongodb](/pictures/arquitectura-mongodb.PNG)

### Bases de Datos
Son los contenedores físicos para las colecciones. Cada base de datos tiene un archivo propio en el sistema de archivos de cada computadora o servidor y un Cluster puede tener múltiples bases de datos.

### Colecciones
Son agrupaciones de documentos. Son equivalentes a las tablas en bases de datos relacionaes pero NO imponen un esquema o estructura rígida para guardar información.

### Documentos
Son registros dentro de las colecciones. Son la unidad básica de MongoDB y son análogos a los objetos JSON pero en realidad son BSON.

**La estructura sería la siguiente:**
![mongodb-coleccion](/pictures/mongodb-coleccion.PNG)

Ruta para ejecutar la consola en local de MongoDB.

C:\Program Files\MongoDB\Server\5.0\bin

**Ejecutar el archivo .exe**

![mongodb-ruta-exe](/pictures/mongodb-ruta-exe.PNG)

**Consola local de MongoDB**

![mongodb-consola](/pictures/mongodb-consola.PNG)

Insertar un registro.

    > db.inventory.insertOne({ item: "canvas", qty: 100, tags: ["cotton"], size: { h: 28, w: 35.5, uom: "cm"}})

![mongodb-comman-struct](/pictures/mongodb-comman-struct.jpg)


![mongodb-comman-struct](/pictures/mongodb-comman-struct-2.jpg)

Instrucciones y comandos:

Conexión con el cluster de MongoDB Atlas: mongo "URL DE NUESTRO CLUSTER", (recuerda añadir tu IP a la lista de IPs permitidas para no tener problemas en esta parte).

Listar las bases de datos de nuestro cluster: show dbs.

Seleccionar una base de datos: use NOMBRE_BD. Debemos crear por lo menos un documento si la base de datos es nueva porque MongoDB no crea bases de datos vacías.

Recordar qué base de datos estamos usando: db.

Listar las colecciones de nuestra base de datos: show collections.

Crear una colección (opcional) y añadir un elemento en formato JSON: db.NOMBRE_COLECCIÓN.insertOne({ ... }). La base de datos responde true si la operación fue exitosa y crea el campo irrepetible de _id si nosotros no lo especificamos.

Crear una colección (opcional) y añadir algunos elementos en formato JSON: db.NOMBRE_COLECCIÓN.insertMany([{ ... }, { ... }]). Recibe un array de elementos y devuelve todos los IDs de los elementos que se crearon correctamente.

Encontrar elementos en una colección: db.NOMBRE_COLECCIÓN.find() Podemos aplicar filtros si queremos o encontrar solo el primer resultado con el método findOne().

Listar todos los posibles comandos que podemos ejecutar: db.NOMBRE_COLECCIÓN.help().

## Tipos de Datos

![mongodb-tipos-datos](/pictures/mongodb-tipos-datos.PNG)

![mongodb-tipos-datos-2](/pictures/mongodb-tipos-datos-2.PNG)

![mongodb-tipos-datos-3](/pictures/mongodb-tipos-datos-3.PNG)

![mongodb-tipos-datos-3](/pictures/mongodb-tipos-datos-4.PNG)

## Esquemas y Relaciones

Los **esquemas** son la forma en que se organiza los documentos en las colecciones. MongoDB no impone ningún esquema pero se pueden seguir buenas prácticas y estructurar los documentos de forma parecida para aprovechar la flexibilidad y escalabilidad de la base de datos sin aumentar la complejidad de la aplicación.

Las **relaciones** son la forma en que las entidades o documentos se encuentran enlazadas unos con otros.

### Relaciones Entre Documentos

Los documentos embebidos ayudan a guardar la información en un solo documentos y ahorra el tiempo que se tarda en consultar diferentes doucmentos a partir de referencias. Sin embargo, las referencias siguen siendo muy importantes cuando se debe actualizar informaicón en diferentes lugares de forma continua.

## Queries y Proyecciones

**Proyecciones**.

![mongodb-proyecciones](/pictures/mongodb-proyecciones.PNG)

**Operadores de comparación**.

![mongodb-operadores-comparacion](/pictures/mongodb-operadores-comparacion.PNG)

**Operadores por elemento**.

![mongodb-operadores-elemento](/pictures/mongodb-operadores-elemento.PNG)

**Operadores para arreglos**.

![mongodb-operadores-arreglos](/pictures/mongodb-operadores-arreglos.PNG)

## Agregaciones

Son operaciones avanzadas que se pueden realizar sobre la base de datos con un poco más de flexibilidad en los documentos.

* **Pipeline de agregaciones**: Es un grupo de múltiples etapas que ejecutan agregaciones en diferentes momentos. Se debe tener en cuenta el **performance** de las agregaciones porque pueden corre en todo el **cluster**.

* **Map-reduce**: Permite definir funciones de JavaScript para ejecutar operaciones avanzadas. la función de **map** permite definir o **mappear** los campos que se desea usar y la función **reduce** permite ejecutar operaciones y devolver resultados especiales. 

* **Agregaciones de propósito único**. Son funciones ya definidas que ayudan a calcular un resultado especial pero se debe tener cuidado porque pueden mejorar o afectar el **performance** de la base de datos.

