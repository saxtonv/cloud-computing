# SmartBuy - Planificador de compras

Como configuré mi entorno en el siguiente enlace
> Hito 0 - *[Configuracion del entorno](https://github.com/saxtonv/cloud-computing/blob/main/docs/hito_0/configuracion.md)*

## Problema a Resolver: 
Al momento de realizar las compras de suministros, normalmente, las personas suelen pronosticar cuanto consumiran un determinado articulo, ya sea de manera diaria, semanal, quincenal, mensual, etc. La variabilidad de lo que consumimos y lo que compramos puede llevar a un desorden en las finanzas personales o familiares. 

## Solucion Propuesta:
Para optimizar la planificacion y pronostico de articulos a consumir en un intervalo de tiempo, se propone una solucion web que pueda ayudar en la tarea considerando variables como el consumo realizado en meses anteriores, el grado de importancia de los articulos y que tan bueno era el producto.

## ¿Por que debe estar en la nube?
El usuario podrá acceder desde cualquier lugar y plataforma, y la performance del procesamiento no dependera de su dispositivo.

## Usuarios Objetivos
Mantenedores de hogar
Responsables de compras

## User Journey
1. El usuario compra un articulo registrandolo en el sistema indicando cantidad, costo e importancia
2. El usuario registra cuando un articulo fue consumido, evaluando el articulo.
3. El usuario solicita al sistema la planificacion de compra indicando el intervalo de tiempo.
4. El usuario quita los articulos que no considera en la planificación.
5. El usuario puede valorar la planificacion realizada por el sistema.

### User Story
Registrar compra de articulo
> Como usuario necesito registrar la compra de un articulo

Registrar consumo de articulo
> Como usuario necesito registrar el consumo de un articulo

Solicitud de planificación
> Como usuario solicito una planificación de compra por un intervalo de tiempo

Modificar planificación
> Como usuario necesito quitar los articulo que no me interesan comprar

Evaluar planificación
> Como usuario quiero evaluar la planificación en relación a lo acertada que esta fue.