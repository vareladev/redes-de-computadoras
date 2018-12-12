# 03 Modelos OSI y TCP/IP.

## 3.1 Modelo de referencia OSI.

Se conoce como suite de protocolos al conjunto de protocolos sobre los que se fundamenta la transmisión de datos en una red de computadoras. Estos definen cada regla de la transmisión.
El modelo OSI si bien es una propuesta sin implementar en la actualidad, se ha convertido en un fundamento teórico para explicar y entender cómo funciona la interconexión de sistemas abiertos. He de ahí que muchos se refieren al modelo OSI como “Modelo de referencia”. El modelo OSI se compone de una serie de capas distribuidas de manera jerárquica, siete en total, cada una cumple con tareas y funciones específicas que son requeridas para lograr comunicar dos sistemas. Cada capa aporta una funcionalidad al proceso, complementando a la capa anterior y ofreciendo sus servicios a la capa superior. Cada vez que dos nodos desean comunicarse, los datos que se  transmite pasan por cada una de las siete capas del modelo OSI.

La siguiente ilustración muestra cada capa, y la jerarquía dentro del modelo de referencia.

![1-modelo-osi-v1](https://user-images.githubusercontent.com/36117314/49886450-4ae7e780-fdff-11e8-8b44-91ca85cf9fdb.png)
 
Las capas de aplicación, presentación, sesión y transporte, forman el conjunto de capas de host y las capas de red, enlace de datos y física el conjunto de datos del medio, estos conjuntos indican donde opera la capa. Cada capa maneja una unidad de datos de protocolos o también llamada PDU, por sus siglas en inglés. Las primeras tres capas trabajan con la PDU datos, La capa de transporte con la PDU segmento, la capa de red utiliza la PDU paquete, la capa de enlace de datos la PDU frame y finalizando con la capa física que utiliza la PDU bits.

![2-modelo-osi-pdu](https://user-images.githubusercontent.com/36117314/49886451-4b807e00-fdff-11e8-8090-0b09ae517eaa.png)

A continuación se describen cada capa del modelo de referencia OSI.

### La capa de aplicación: 

Proporciona los servicios utilizados por las aplicaciones para que los usuarios se comuniquen a través de la red. Es el nivel más cercano al usuario. 

### La capa de presentación: 

Define el formato de los datos que se van a intercambiar entre las aplicaciones, ofreciendo un conjunto de servicios para la transformación de datos.

### La capa de sesión: 

Proporciona los mecanismos para controlar el diálogo entre las aplicaciones de los sistemas finales: abre, mantiene y cierra la sesión entre dos sistemas.

### La capa de transporte: 

Permite intercambiar datos entre sistemas finales, dividiendo el mensaje en varios fragmentos. El servicio de transporte puede ser orientado o no orientado a conexión.

### La capa de red: 

Se encarga de definir el camino que seguirán los datos desde el origen hasta su destino a través de una o más redes conectadas mediante dispositivos de enrutamiento (router).

### La capa de enlace de datos: 

Se ocupa del direccionamiento físico dentro de cualquier topología de red, esta capa nos permite activar, mantener y deshabilitar la conexión, así como la notificación de errores.

### La capa física: 

Controla las señales por donde viajaran los datos (cable de par trenzado, fibra óptica, radio frecuencia).

## 3.1.1 Ventajas del modelo OSI.

* Facilita la comprensión al dividir un problema complejo en partes más simple.

* Evita los problemas de compatibilidad, por ejemplo de red

* Detalla las capas para su mejor aprendizaje.

* Proporciona a los fabricantes un conjunto de estándares que aseguraron una mayor compatibilidad e interoperabilidad entre los distintos tipos de tecnología de red utilizados por las empresas a nivel mundial.

## 3.2 El modelo TCP/IP

El 1968 la Agencia de investigación de Proyectos Avanzados del Departamento de Defensa de EE.UU. (DARPA) inicia el desarrollo de un sistema que permitiese la transmisión de datos entre diferentes computadoras que tenían la característica de esta en diferentes tipos de redes, fue asi como se implementó ARPANET, una red punto a punto que se basaba en las líneas telefónicas, el conjunto de protocolos que se utilizó, posteriormente pasarían a ser llamado TCP/IP. Esta investigación conformada por instituciones educativas, militares y de investigación se convertiría en el núcleo de lo que ahora es Internet.
La suite de protocolos TCP/IP permiten la comunicación entre diferentes dispositivos pertenecientes a una red. TCP/IP basa su nombre en dos de los protocolos más importantes incluidos en el conjunto y significa Protocolo de control de transmisión/Protocolo de Internet.

TCP/IP establece todas las reglas de comunicación para internet y se basa el concepto de dirección IP, es decir, para que un dispositivo pueda pertenecer a una red, es necesario que disponga de una dirección única, llamada dirección IP. La siguiente ilustración describe las capas del modelo TCP/IP:

![3-modelotcp-ip](https://user-images.githubusercontent.com/36117314/49886452-4b807e00-fdff-11e8-8356-157ad4d4e8af.png)
 
### Capa de aplicación:

Es la capa superior del modelo TCP/IP, En ella se encuentran todas las aplicaciones de red que permiten la comunicación del usuario, Algunos de los protocolos que trabajan en esta capa son: 

* FTP (File transfer Protocol), Útil para la trasferencia de archivos.

* HTTP (Hipertext Transfer Protocol), navegación en internet.

* SMTP (Simple Mail Transfer Protocol), Uso de correo electrónico.

* DNS (Domain Name Server), Facilita el contacto con otros dispositivos utilizando nombres fáciles de recordar.

* Telnet  (Telecommunication Network), Conexiones remotas.

### Capa de transporte.

La capa de transporte es la responsable de establecer las conexiones lógicas entre los host emisor y receptor, el conjunto de protocolos pertenecientes a esta capa, segmentan los datos en el host origen para que las capas inferiores realicen el envío y una vez llegan al destino, los segmentos son ensamblados para recuperar el mensaje original, de esta manera se logra una manera de transporte de datos confiable.

La capa de transporte contiene dos protocolos que permiten que dos aplicaciones puedan intercambiar datos independientemente del tipo de red (es decir, independientemente de las capas inferiores). Los dos protocolos son el TCP y UDP, que se diferencian por el tipo de servicio que ofrecen. TCP, es un protocolo orientado a conexión que brinda detección de errores. TCP asegura que cada paquete enviado sea recibido correctamente, En cambio, UDP es un protocolo no orientado a conexión en el que la detección de errores es obsoleta. Y no se detiene a verificar si los paquetes llegaron. 

### Capa de internet.

Esta capa es la responsable de que podamos comunicarnos con cualquier host  del mundo que esté conectado a Internet. tiene como finalidad seleccionar la mejor ruta para transmitir los paquetes por la red, de tal manera que cada paquete atraviese la menor cantidad de routers en el menor tiempo posible. La capa de Internet contiene 5 protocolos: IP, ARP, ICMP, IGMP y RARP. Los primeros tres protocolos son los más importantes para esta capa.

### Capa de acceso a la red.

Esta es la capa inferior del modelo TCP/IP, es la responsable de que dos host puedan comunicarse independientemente del tipo de red física a la que se conectan, es decir, brinda los estándares del medio que se deben implementar para transmitir datos a través de la red. Por lo tanto, la capa de acceso a la red contiene especificaciones relacionadas con la transmisión de datos por una red física,

La siguiente ilustración muestra los protocolos más conocidos del modelo TCP/IP, estos protocolos son los responsables de que Internet funcione como lo conocemos.

![4-suite-protocolos-tcp-ip](https://user-images.githubusercontent.com/36117314/49886455-4c191480-fdff-11e8-814d-7be5a95ae9f7.png)

## 3.2.1 Ventajas del modelo TCP/IP:

* El conjunto TCP/IP está diseñado para enrutar.

* Tiene un grado muy elevado de fiabilidad.

* Es adecuado para redes grandes y  medianas, así como redes empresariales.

* Es compatible con las herramientas estándar para analizar el funcionamiento de la red.

* Proporciona abstracción de capas.

* Puede funcionar en máquinas de todo tamaño (multiplataforma).

* Soporta múltiples tecnologías.

* Imprescindible para Internet.

## 3.3 Comparación entre el modelo OSI y TCP/IP.

Ambos modelos son de gran importancia, han logrado resolver los grandes problemas de compatibilidad entre diferentes tipos de dispositivos y tecnologías, definen los métodos y la forma que se debe realizar las comunicaciones por medio de una arquitectura basada en capas. Existen algunas diferencias entre un modelo y otro aunque el propósito para que el que fueron creados sea muy semejante.

En primer lugar, el modelo OSI describe en más capas su funcionamiento con respecto al modelo TCP/IP. La capa de aplicación del modelo TCP/IP incluye las capas de aplicación, presentación y sesión del modelo de referencia OSI, y la capa de acceso a la red del modelo TCP/IP incluye las capas física y enlace de datos del modelo OSI. 

![5-osi-vs-tcpip](https://user-images.githubusercontent.com/36117314/49886456-4c191480-fdff-11e8-9c0c-016a539f0feb.png)

Sin embargo, aunque OSI es un excelente modelo, solo ha servido como referente teórico por lo general y detallado que es; mientras que en términos prácticos se opta por TCP/IP debido a que los protocolos para este último son más adecuados a la realidad.

## 3.4 Referencias:

* [https://docs.oracle.com/cd/E19957-01/820-2981/ipov-8/index.html](https://docs.oracle.com/cd/E19957-01/820-2981/ipov-8/index.html)

* [https://docs.oracle.com/cd/E19957-01/820-2981/ipov-10/](https://docs.oracle.com/cd/E19957-01/820-2981/ipov-10/)

* [https://www.uaeh.edu.mx/scige/boletin/huejutla/n10/r1.html#refe1](https://www.uaeh.edu.mx/scige/boletin/huejutla/n10/r1.html#refe1)

## 3.5 Autores

* **Erick Varela** ([vareladev](https://github.com/vareladev/))