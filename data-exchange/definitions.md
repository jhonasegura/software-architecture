# Data Exchange 

Un Data Exchange permite controlar y gobernar el acceso a los datos cuando se comparten dentro de una empresa o externamente con proveedores, socios o clientes.

## CRUD vs REST

Son dos conceptos destacados en la industria de las API, a menudo confundidas. Mientras que REST es uno de los **estilos de diseño** más populares para API web, CRUD es **simplemente un acrónimo** que se usa para referirse a cuatro operaciones básicas que se pueden realizar en aplicaciones de base de datos: Create, Read, Update and Delete.

### CRUD

Son las cuatro funciones principales que se utilizan para interactuar con las aplicaciones de bases de datos. El acrónimo es popular entre los programadores ya que proporciona un recordatorio rápido de qué funciones de manupulación de datos se necesitan para que una aplicación se sienta completa.

### REST

Es un **estilo arquitectónico** especialemente para API web. Está definido por cinco restricciones de diseño que, cuando se siguen ,producen una aplicación con propiedades específicas que influyen el rendimiento, simplicidad y confiabilidad.

Las cinco restricciones básicas que se definen en una aplicación REST son:

1. **Cliente-Servidor:**: El cliente y el servidor actúan de forma independiente.

2. **Sin estado**: El servidor no registra el estado del cliente.

3. **En caché**: El servidor marca si los datos se pueden almacenar en caché.

4. **Interfaz uniforme**: El cliente y el servidor interactúan de manera uniforme y predecible. Un aspecto importante de esto es que el servidor **expone recursos**.

5. **Sistema en capas**: La aplicación se comporta igual independientemente de los intermediarios entre el cliente y el servidor.

Por la naturaleza de las API REST que se sirven a través d ela web, estas API se comunican con los clientes mediante el protocolo HTTP, que tiene su propio conjunto de métodos para la manipulación de datos: GET, POST, DELETE, PUT y PATCH, entre otros.

## ORM 

Un Object Relational Mapping es un modelo de programación que permite mapear las estructuras de una base de datos relacional RDBMS (Relational Database Management System) sobre una estructura lógica de entidades con el objeto de simplificar y acelerar el desarrollo de aplicaciones. Esto nos permitirá interactuar con la base de datos sin necesidad de conocer SQL, todo mediante programación orientada a objetos.

Las estructuras de la base de datos relacional quedan **vinculadas con las entidades lógicas** o base de datos virtual definida en el ORM, de tal modo que las acciones CRUD a ejecutar sobre la base de datos física se **realizan de forma indirecta** por medio del ORM.

Los ORMs tienen de "liberar" de la escritura o generación manual de código SQL necesario para realizar las queries o soncsultas y gestionar la persistencia de datos en el RDBMS.

Los objetos o entidades de la base de datos virtual creada en el ORM podrá ser manipulados por medio de algún lenguaje según el tipo de ORM utilizado.

### Ventajas

* Cada ORM se encuentra diseñado para un lenguaje en particular, por lo cual no es una preocupación conocer y dominar SQL. Permitiendo enforcar al cien por cierto en el lenguaje que se esté utilizando del lado backend.

* La mayoría de ORMs permiten interactuar con diferentes gestores de base de datos, pudiendo así en caso se necesite, cambiar de un gestor a otro sin muchos problemas.

* Dependiendo del ORM, se puede utilizar transacciones, migraciones, triggers e inclusive la posibilidad de trabajar con vistas o store procedures sin necesidad de conocer sobre SQL.

### Desventajas

* Para consultas complejas que involucren múltiples tablas, condiciones u operaciones es posible que el ORM no llegue a generar las sentencias más óptimas para el gestor o se torne aún más complejo crear las consultas utilizando objetos que utilizando el mismo SQL.

* Es posible que las configuraciones sean tediosas, teniendo que importar, instalar, actualizar o generar nuevos archivos.


## Bibliography

* https://www.redhat.com/architect/apis-soap-rest-graphql-grpc
* https://www.instintoprogramador.com.mx/2020/12/crud-vs-rest-cual-es-la-diferencia.html
* https://www2.deloitte.com/es/es/pages/technology/articles/que-es-orm.html
* https://codigofacilito.com/articulos/orm-explicacion