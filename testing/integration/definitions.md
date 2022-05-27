# Pruebas de Integración

## Pirámide de Automatización de Pruebas

![](/testing/pictures/piramide-testing.png)

1. Extremo a Extremo.
2. Integración. Software que depende de otros elementos.
3. Unitarias.

Entre más arriba se esté en la piramide, la prueba será más lenta, más costosa y más difícil de mantener. Menor número. 

* Bases de Datos(Internas o Externas).
* Servidor.
* Sistema de un tercero.
* Sistema de archivos.
* API públicas

## Problemas Probando Integraciones

Sistema bajo prueba --> Componente del que se depende.

* Acceso lento.
* 