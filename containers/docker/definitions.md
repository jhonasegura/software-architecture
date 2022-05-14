# Docker

Docker es una plataforma de software que permite crear, probar e implementar aplicaciones rápidamente. Docker empaqueta software en unidades estandarizadas llamadas contenedores que incluyen todo lo necesario para que el software se ejecute, incluidas bibliotecas, herramientas de sistema, código y tiempo de ejecución. Con Docker se puede implementar y ajustar la escala de aplicaciones rápidamente en cualquier entorno con la certeza de saber que el código se ejecutará.

## ¿Cómo Funciona Docker?

Docker proporciona una manera estándar de ejecutar el código. Es un sistema operativo de contenedores. De manera similar a cómo una máquina virtual virtualiza el hardware del servidor, los contenedores virtualizan el sistema operativo de un servidor. Docker se instala en cada servidor y proporciona comandos sencillos que se puede utilizar para crear, iniciar o detener contenedores.

## ¿Por Qué Usar Docker?

Docker permite entregar código con mayor rapidez, estandarizar las operaciones de las aplicaciones, transferir el código con facilidad y ahorrar dinero al mejorar el uso de recursos. Se obtiene un solo objeto que se pued ejecutar de manera fiable en cualquier lugar. La sintaxis sencilla y simple aporta un control absoluto. La amplia adopción significa que existe un gran ecosistema de herramientas y aplicaciones listas para su uso que se puede utilizar con Docker.

* **Enviar más software, más rápido**.

* **Estandarizar las operaciones**.

* **Transferir de manera sencilla**.

* **Ahorrar dinero**.

## Comandos Útiles

!['docker-commands'](/pictures/docker-commands.jpeg)

Ejecutar primero comando para verificar funcionamiento de Docker.

    $ docker run hello-world 

Muestra los contenedores activos.

    $ docker ps (muestra los contenedores activos)

Muestra todos los contenedores.

    $ docker ps -a (muestra todos los contenedores)

Muestra el detalle completo de un contenedor.

    $ docker inspect <containe ID> (m)

Igual que el anterior pero invocado con el nombre.

    $ docker inspect <name> (i)

Le asigna el nombre custom "hello-platzi".

    $ docker run –-name hello-platzi hello-world

Cambia el nombre de "hello-platzi" a "hola-platzi".

    $ docker rename hello-platzi hola-platzy 

Borra un contenedor a partir de su ID o nombre.

    $ docker rm <ID o nombre>

Borra todos lo contenedores que esten parados.

    $ docker container prune

Comandos:

    $ docker run ubuntu (corre un ubuntu pero lo deja apagado)

    $ docker ps -a (lista todos los contenedores)

    $ docker -it ubuntu (lo corre y entro al shell de ubuntu)

-i: interactivo
-t: abre la consola

<h1>cat /etc/lsb-release (veo la versión de Linux)</h1>

Comandos:

    $ docker run -d --name proxy nginx (corro un nginx)

    $ docker stop proxy (apaga el contenedor)
    
    $ docker rm proxy (borro el contenedor)

    $ docker rm -f <contenedor> (lo para y lo borra)

    $ docker run -d --name proxy -p 8080:80 nginx (corro un nginx y expongo el puerto 80 del contenedor en el puerto 8080 de mi máquina)

localhost:8080 (desde mi navegador compruebo que funcione)

    $ docker logs proxy (veo los logs)

    $ docker logs -f proxy (hago un follow del log)

    $ docker logs --tail 10 -f proxy (veo y sigo solo las 10 últimas entradas del log)


Comandos:

    $ mkdir dockerdata (creo un directorio en mi máquina)

    $ docker run -d --name db mongo
    
    $ docker ps (veo los contenedores activos)

    $ docker exec -it db bash (entro al bash del contenedor)

    $ mongo (me conecto a la BBDD)

    $ shows dbs (listo las BBDD)

    $ use platzi ( creo la BBDD platzi)

    $ db.users.insert({“nombre”:“guido”}) (inserto un nuevo dato)

    $ db.users.find() (veo el dato que cargué)

    $ docker run -d --name db -v <path de mi maquina>:<path dentro del contenedor(/data/db mongo)> (corro un contenedor de mongo y creo un bind mount)

## Bibliografía

* https://aws.amazon.com/es/docker/
