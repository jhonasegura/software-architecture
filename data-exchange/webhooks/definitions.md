# Webhooks

Es una herramienta que permite que un sistema o aplicación envíe notificaciones sobre un evento específico a otro sistema o aplicación en tiempo real. Un webhook se programa para enviar notificaciones emergentes a una determinada URL cuando se produce una actividad vinculada con un evento específico. 
 
## ¿Cómo Funciona?

EL webhook espera a que ocurra un evento en un sistema o aplicación y a continuación transfiere los datos a otra aplicación o sistema usando una retrollamada HTTP POST a la URL de destino. Esta URL tiene que ser pública y pertenecer al sistema o aplicaicón de destino, se debe configurar como punto de destino de un webhook para que el sistema pueda recibir la notificación.

## ¿Cuál es la Diferencia con un API?

Las APIs funcionan con una técnica de sondeo, un proceso por el cual el servidor envía una solicitud al servidor de la API para comprobar si hay nuevos datos. Por el contrario, un webhook envía los datos automáticamente. 

Este método es más eficiente que revisar constantemente una aplicación para ver si han habido cambios.

## Bibliografía 

* https://es.sendinblue.com/blog/que-es-un-webhook/#:~:text=Un%20webhook%20(tambi%C3%A9n%20conocido%20como,o%20aplicaci%C3%B3n%20en%20tiempo%20real.

* https://www.campusmvp.es/recursos/post/que-son-los-webhooks-en-que-se-diferencian-de-una-api-rest-y-por-que-deberias-conocerlos.aspx