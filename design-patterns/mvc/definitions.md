# Modelo Vista Controlador (MVC)

Es un patrón de arquitectura de software que separa los datos y principalmente lo que es la lógica de negocio de una aplicación de su representación y el módulo encargado de gestionar los eventos y las comunicaciones. Se basa en las ideas de reutilización de código y la seperación de conceptos, características que buscan facilitar la tarea de desarrollo de aplicaciones y su ´psterior mantenimiento.

## Descripción del Patrón

De manera genérica, los componentes de MVC se podrían definir en:

* El **Modelo**: Define qué datos debe contener la aplicación. Si el estado de estos datos cambia, el modelo generalmente notificará a la vista (para que pueda cambiar según sea necesario) y, a veces, el controlador (si se necesita una lógica diferente para controlar la vista actualizada).

* La **Vista**: Define cómo se deben mostrar los datos de la aplicación. La vista definiría cómo se presenta la data al usuario y recibiría los datos para mostrar desde el modelo.

* El **Controlador**: Contiene una lógica que actualiza el modelo y/o vista en respuesta a las entradas de los usuarios de la aplicación. 

![modelo-vista-controlador](/design-patterns/pictures/model-view-controller.png)

## Modelos

Son los que se encargan de manejar los datos de la aplicación, van a tener la lógica del problema. Es lo que no se ve visualmente. Se va a comunicar con las vistas, frente a un cambio en los datos, notificará a todos los obsevadores para que se puedan actualizar. Los datos serán guardados, sea en una DB o en el Browser. Siendo el modelo el encargado de almacenar la informaicón.


## Bibliografía

* https://es.wikipedia.org/wiki/Modelo%E2%80%93vista%E2%80%93controlador
* https://developer.mozilla.org/es/docs/Glossary/MVC