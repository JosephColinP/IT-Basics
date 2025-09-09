# Communication Protocols



Communication in our daily lives takes many forms and occurs in many environments. We have different expectations depending on whether we are chatting via the internet or participating in a job interview. Each situation has its corresponding expected behaviors and styles.

Before beginning to communicate with each other, we establish rules or agreements to govern the conversation. These agreements include the following:
• What method of communication should we use?
• What language should we use?
• Do we need to confirm that our messages are received?

These rules, or protocols, must be followed in order for the message to be successfully delivered and understood.

The same principle applies to computer communication, the computer must know how it's gonna send the message, in what language and if it needs a confirmation.

Networking protocols define many aspects of communication over the local network. As shown in the table, these include message format, message size, timing, encoding, encapsulation, and message patterns.



| Protocol Characteristic | Description                                                  |
| ----------------------- | ------------------------------------------------------------ |
| Message format          | Is the format or structure that the computer gives depending on the type of message and the channel that is used to deliver the message. |
| Message size            | There're rules that govern the size of each message. When a long message is sent from host to another, it may be necessary to break the massage into smaller pieces in order to ensure the reliability. |
| Timing                  | Timing determines the speed at which the bits are transmitted across the network. |
| Encoding                | The messages sent across the network are first converted into bits by sending host. Each bit is encoded into a pattern of sound, light waves, or eletrical impulses, depending on the network media over which the bits are transmitted. |
| Encapsulation           | Each message transmitted on a network must include a  header that contains addressing information that identifies the source and destination hosts, otherwise it cannot be delivered. |
| Message Pattern         | Some messages requrie an acknowledment before the next message can be sent. This type of request/response pattern is a common aspect of many protocols. |



## IP (Internet Protocol)

Esta es una etiqueta numérica que se le asigna a un sistema que se comunica bajo un protocolo de internet para identificarlo en una red. Esta etiqueta facilita las funciones de ruteo que permiten la transmisión de datos de un sistema a otro. Existen dos versiones de IPs: 

1. IPV4: Contiene 32 bits.
2. IPV6: Contiene 128 bits.

También existen dos tipos de IP:

1. **LAN (Local address Network):** Se encuentra dentro de una red local, esta IP se puede comunicar con equipos de la misma red.

2. **WAN (Wide Area Network):** Son IPs globales, se puede comunicar con cualquier dirección IP global e internet. Pero no pueden acceder directamente a una dirección IP local sin estar en esta.

   

## TCP (Transmission Control Protocol)

Mediante este protocolo los paquetes de datos son enviados de manera precisa y segura. Para esto lleva verificaciones a través de paquetes, llamado “Three-way Handshake” debido a que se realizan tres verificaciones antes de establecer una conexión y mandar datos. Estas verificaciones se llaman; **SYN, ACK/SYN, ACK:**

1. **SYN:** El cliente manda un paquete para establecer una comunicación con el servidor.
2. **ACK/SYN:** El servidor responde con este paquete para reconocer que ha recibido la solicitud de comunicación y pide al cliente que abra una conexión.
3. **ACK:** El cliente regresa el paquete para finalmente comenzar una comunicación estable.

Esto se realiza para confirmar que la máquina puede recibir los datos, el primero avisa si pueden comunicarse, el segundo paquete es la otra máquina confirmando la comunicación, y el último paquete es el que inicia la comunicación.



## UDP (User Datagram Protocol)

En este protocolo solo se enfoca a la velocidad sin confirmar que han sido recibidos los paquetes. Este protocolo se usa por ejemplo para eventos en vivo como videollamadas.





## Common Protocols

1. TCP (Transmission Control Protocol): Es un protocolo de comunicación orientado a conexión que garantiza la entrega confiable de datos.
2. UDP (User Datagram Protocol): Es un protocolo de comunicación sin conexión que no garantiza la entrega de datos.
3. HTTP (Hypertext Transfer Protocol): Es un protocolo de comunicación utilizado para transferir información en la World Wide Web.
4. FTP (File Transfer Protocol): Es un protocolo de comunicación utilizado para transferir archivos entre sistemas.
5. SMTP (Simple Mail Transfer Protocol): Es un protocolo de comunicación utilizado para transferir correo electrónico entre sistemas.
6. DNS (Domain Name System): Es un protocolo de comunicación utilizado para traducir nombres de dominio en direcciones IP.
