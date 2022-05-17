# Modelo Vista Controlador (MVC)

Es un patrón de arquitectura de software que separa los datos y principalmente lo que es la lógica de negocio de una aplicación de su representación y el módulo encargado de gestionar los eventos y las comunicaciones.

## Modelos

Son los que se encargan de manejar los datos de la aplicación, van a tener la lógica del problema. Es lo que no se ve visualmente. Se va a comunicar con las vistas, frente a un cambio en los datos, notificará a todos los obsevadores para que se puedan actualizar. Los datos serán guardados, sea en una DB o en el Browser. Siendo el modelo el encargado de almacenar la informaicón.