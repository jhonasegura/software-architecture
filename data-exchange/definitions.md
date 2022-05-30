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

## WSDL (Web Services Description Language)

Es una especificación estándar para describir servicios basados en XML de red. Proporciona a los proveedores de servicios un modo sencillo de describir el formato básico de las peticiones a sus sistemas independientemente de la implementación del motor de ejecución subyacente.

## Comparación de Casos de Uso para REST, GraphQL, Webhooks y gRPC

Como puede ver claramente, ninguna de estas opciones es realmente "mejor" que las demás, sino que encaja en escenarios de interacción únicos. Podemos resumir estos casos de uso de la siguiente manera:

* **REST**: una arquitectura sin estado para la transferencia de datos que depende de hipermedia . REST puede unir una amplia gama de recursos que se pueden solicitar en una variedad de formatos para diferentes propósitos. REST se ocupa fundamentalmente de la gestión de recursos sin estado, por lo que es mejor utilizarlo en tales situaciones. Los sistemas que requieren una iteración rápida y una verborrea HTTP estandarizada encontrarán que REST se adapta mejor a sus propósitos.

* **gRPC**: un sistema ágil y ligero para solicitar datos . gRPC, por otro lado, se usa mejor cuando un sistema requiere una cantidad determinada de datos o procesamiento de forma rutinaria, y en el que el solicitante tiene poca energía o está celoso de los recursos. El IoT es un gran ejemplo de esto.

* **GraphQL**: un enfoque en el que el usuario define los datos esperados y el formato de esos datos . GraphQL es de Facebook, y ese pedigrí demuestra bien su caso de uso: situaciones en las que el solicitante necesita los datos en un formato específico para un uso específico. En esos casos, esos formatos de datos y las relaciones entre ellos son de vital importancia, y ninguna otra solución proporciona el mismo nivel de suministro de datos interconectados.

* **Webhooks**: las actualizaciones de datos se entregarán automáticamente, en lugar de solicitarse . Finalmente, los Webhooks se utilizan mejor cuando la API en cuestión actualiza principalmente a los clientes. Si bien dichas API también pueden tener otras funciones, incluso RESTful, el uso principal de un microservicio de Webhook debe ser actualizar clientes y proporcionar datos actualizados y aprovisionados tras la creación del nuevo recurso actualizado.

Elegir entre estas opciones específicas es realmente una cuestión de alinear las funciones de su negocio con el enfoque apropiado y asegurarse de que los sistemas implementados respondan dentro de los parámetros dados.

## Bibliography

* https://www.redhat.com/architect/apis-soap-rest-graphql-grpc
* https://www.instintoprogramador.com.mx/2020/12/crud-vs-rest-cual-es-la-diferencia.html
* https://www2.deloitte.com/es/es/pages/technology/articles/que-es-orm.html
* https://codigofacilito.com/articulos/orm-explicacion
* https://www.ibm.com/docs/es/rsas/7.5.0?topic=standards-web-services-description-language-wsdl
* https://www.instintoprogramador.com.mx/2021/01/cuando-usar-que-rest-graphql-webhooks-y.html