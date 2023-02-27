# AWS Certified Cloud Practitioner Course.

`AWS Database Migration Service`
- servicio utilizado para la migracion de una base de datos a AWS 


Existen dos manera de iniciar sesion en AWS 

```mermaid
flowchart LR; 

 Usuario_Raiz-->Usuario_AIM

```
## Cambio de idioma del Dashboard
****

en la parte inferior del navegadpr buscar el texto que dice `unified settings` donde podemos configurar el idioma de nuestra interfaz y la `Region` predeterminada donde alojaremos nuestros servicios, los nomnbres de los servicios seguiran en ingles.

## Cloud Computig.
****
```mermaid
flowchart LR
cliente --peticion---> red((Red))
red((Red)) --viaja---> database[(Contenido)]
database[(contenido)]--respuesta-->red((Red))
red((Red))--viaja-->cliente
```

los clientes se identifican por medio de una IP , los servidores tambien tienen una IP 
### funcionamiento.
***
un cliente con una IP especifica envia una peticion para acceder a un contenido cuando el servidor recibe la peticion del cliente devuelve una respuesta a esa determinada IP con el contenido que solicito.

### como se compone un servidor.
```mermaid
flowchart TD
cpu --> ram 
cerebro -->cpu
informacion -->almacenamiento
cerebro --->informacion
informacion ---> Router_switch_servidorDNS
ram --> almacenamiento

almacenamiento --> base_de_datos
base_de_datos --> Red
```

### Red.
***
Es lo que nos permite comunicarnos con un destinatario `cables , routers,servidores conectados entre si `

### Router
___
Dispositivo de red que reenvia paquetes de datos entre redes de ordenadores y que saben exactamente donde enviar los paquetes a traves de la red 

### Switch.
___
este dispositivo toma los paquetes y los envia a un servidor al que el cliente se ha conectado 

```mermaid
flowchart LR 
pc --> router
router -->switch
switch --> pc1
switch --> pc2
switch --> pc3
```
`infraestructura de un paquete enviado desde un pc , pasando por un router luego al switch hasta llegar a un despinatario (pc...n)`

## Manera Tradicional de Constuir Infraestructuras
***

```mermaid
flowchart LR
Servidores/Casa ---> Oficinas
```
```
Contras
```
- pago de alquileres 
- pago suministro electrico refrigeracion y mantenimiento de los servidores
- cambio de hardware cada x cantidad de tiempo
- el escalado es limitado (cantidad de clientes soportados)
- contratar un equipo 24/7 para supervisar la insfraestructura
- eventos naturales, incendios, terremotos , apagones



