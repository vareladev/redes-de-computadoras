# 01 Introducción a las redes de computadoras.

## 1.1 Definición de una red de computadoras.

Una red de computadoras es un conjunto de equipos informáticos conectados entre sí utilizando cables, ondas electromagnéticas o fibra de vidrio como medio de comunicación y transporte de datos. El objetivo es lograr que se puedan compartir información (como archivos), recursos (como una impresora o fotocopiadora) y  servicios (Correo electrónico e Internet). A cada uno de los dispositivos informáticos conectados se les denomina nodo.

## 1.2 Historia.

La siguiente tabla explica un resumen de la historia de las redes de computadoras. 

![cronologia-redes](https://user-images.githubusercontent.com/36117314/49407689-07b2b800-f71f-11e8-8c96-f698433decb6.png)
 
 
## 1.3 Conceptos básicos.

* *Nodo:* 

En redes de computadoras cada una de las máquinas es un nodo, y si la red es Internet, cada servidor constituye también un nodo.

* *Servidor:*

Es una computadora que, formando parte de una red, provee servicios a otras computadoras denominadas clientes. También se suele denominar con la palabra servidor a Una aplicación informática o programa que realiza algunas tareas en beneficio de otras aplicaciones llamadas clientes.

* *Cliente:*

Nodo que realiza peticiones en forma de mensajes de servicio a los proveedores del mismo. Es decir, a los servidores.

* *Red de computadoras:*

Una red de computadoras es un conjunto de equipos informáticos conectados entre sí utilizando un medio y lograr compartir información, recursos  y/o servicios.

* *Medio:*

Elemento físico que los nodos utilizan para comunicarse, este puede ser un cable, vidrio o incluso el aire.

* *Conmutación de circuitos:*

Los nodos que se desean comunicar deben primero definir un camino físico de comunicación, este camino permanece activo durante la comunicación, liberándose al terminar.

* *Conmutación de paquetes:*

El emisor divide los mensajes en un numero arbitrario de pequeñas secciones de igual tamaño llamadas paquetes, que luego serán transmitidos por diferentes medios de conexión, en esta forma de comunicación no es necesario establecer un solo camino físico durante toda la comunicación.


## 1.4 Componentes de una red.

Dentro de una red actual pueden convivir una gran cantidad de componentes, para facilitar la comprensión de las diferentes configuraciones que se pueden realizar, se han tomado algunos iconos que representan de manera gráfica estos componentes; Algunos de los más utilizados son:
 
![componentes de una red](https://user-images.githubusercontent.com/36117314/49407688-07b2b800-f71f-11e8-87ec-fcf3706a128c.png)

* *Computadora de escritorio:*

Nodo básico de una red. Suelen funcionar como componentes clientes, es decir, solicitan información, servicios o recursos a la red.

* *Portátil:*

Equivalente a la computadora de escritorio, con la diferencia que es un nodo que se puede movilizar fácilmente.

* *Firewall:*

Componente físico o programa que controla el acceso de una computadora a la red y de elementos de la red a la computadora, por motivos de seguridad. 

* *Servidor:*

Componente físico o programa que ofrece servicios a los clientes de la red.

* *Switch LAN:*

Dispositivo de interconexión de dispositivos a nivel de capa 2 del modelo TCP/IP, es decir, interconecta nodos de manera local.

* *Router:*

Dispositivo que se encarga de la interconexión de diferentes redes y  trabaja en la capa 3 del modelo TCP/IP.

* *Nube de red:*

Elemento que representa gráficamente una red que no está bajo nuestro control y suele ser desconocida, por ejemplo Internet.

* *Medio LAN:*

Medio de comunicación que interconecta dispositivos de red de manera local.

* *Medio WAN:*

Medio de comunicación que interconecta dispositivos de red de manera remota.


## 1.5 Protocolos de red.

### Definición.

Conjunto de normas standard que especifican el método para enviar y recibir datos entre varios ordenadores. Es una convención que controla o permite la conexión, comunicación, y transferencia de datos entre dos puntos finales.
Generalidades.

Un protocolo puede ser definido como las reglas que dominan la manera en la que los dispositivos de red se comunican; Especifican la sintaxis, semántica y sincronización de la comunicación. Pueden ser implementados de manera física o lógica o una combinación de ambos.
Los protocolos son la solución a uno de los problemas a los que se enfrentaron las redes de computadoras primitivas: cada equipo puede manejar un lenguaje distinto y operar bajo reglas diferentes, esto puede depender de la arquitectura física del host o del sistema operativo que maneja. Los protocolos son necesarios para que todos los posibles host que se conecten a la red "hablen" el mismo idioma cuando intercambian datos.
No existe un único protocolo de red, de hecho, lo normal es que en un host coexistan múltiples protocolos instalados, cada uno para una tarea específica.

Algunos de los protocolos más famosos pueden ser:

* ARP: protocolo de resolución de direcciones, para encontrar la dirección física (MAC) correspondiente a una determinada IP.

* FTP: protocolo de transferencia de archivos, popular en la transferencia de archivos.

* HTTP: protocolo de transferencia de hipertexto, que es popular porque se utiliza para acceder a las páginas web.

* POP: protocolo de oficina de correo, para correo electrónico.

* SMTP: protocolo para transferencia simple de correo, para el correo electrónico.

* Telnet (Telecommunication Network), para acceder a equipos remotos.


## Referencias:

* [http://kal-el.ugr.es/internet/section3_2.html](http://kal-el.ugr.es/internet/section3_2.html)

* [https://www.ecured.cu/Protocolos_de_red](https://www.ecured.cu/Protocolos_de_red)

## Autores

* **Erick Varela** ([vareladev](https://github.com/vareladev/))