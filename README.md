
# Networks and Computer Security
>
> This repo was created to address some teorical questions about networks posed by the 'Networks and Computer Security' class.
>
>
> *Este repositorio fue creado para abordar algunas preguntas teóricas sobre redes planteadas por la clase 'Redes y Seguridad Informática'*.
>

# Pregunta 1

## ¿Cuáles son las funciones del protocolo tcp/ip?

El protocolo TCP/IP consta de varios protocolos individuales, y cada uno tiene funciones específicas. Pero los más importantes son:

- IP (Internet Protocol):
      - Direccionamiento: IP es responsable de asignar direcciones únicas a cada dispositivo en una red IP, lo que permite que los datos se enruten correctamente a su destino.
      - Enrutamiento: IP determina la mejor ruta para que los paquetes de datos viajen desde el remitente hasta el destinatario a través de una red de múltiples dispositivos interconectados.

- TCP (Transmission Control Protocol):
      - Control de flujo: TCP asegura que los datos se transmitan de manera confiable y en orden entre dos dispositivos. Esto se logra mediante la numeración y el seguimiento de los paquetes de datos, así como la solicitud de retransmisión en caso de pérdida o daño de datos.
      - Establecimiento y finalización de conexiones: TCP permite la creación de conexiones entre dos dispositivos a través de un "proceso de tres vías de apretón de manos (handshake)" y su cierre adecuado al finalizar la comunicación.
      - Segmentación y reensamblaje: TCP divide los datos en segmentos más pequeños para su transmisión y luego los reensambla en el orden correcto **en el destino**.

- UDP (User Datagram Protocol):
      * Transmisión sin conexión: A diferencia de TCP, UDP es un protocolo sin conexión que no garantiza la entrega de datos ni el orden. Es útil para aplicaciones que requieren una transmisión rápida y no crítica de datos, como la transmisión de audio y video en tiempo real.

- DNS (Domain Name System):
      * Resolución de nombres: DNS **se encarga de traducir nombres de dominio legibles por humanos** (como <www.mi-sitio.com>) en direcciones IP numéricas que las computadoras pueden entender y utilizar para localizar servidores en la red.

- HTTP (Hypertext Transfer Protocol):
      Transferencia de hipertexto: HTTP es un protocolo de la capa de aplicación utilizado para la transferencia de páginas web y otros recursos en la World Wide Web. Facilita la solicitud y la respuesta entre navegadores web y servidores web.

- SMTP (Simple Mail Transfer Protocol) y POP/IMAP:
      Correo electrónico: SMTP se utiliza para enviar correos electrónicos desde un cliente de correo a un servidor de correo, mientras que POP (Post Office Protocol) e IMAP (Internet Message Access Protocol) se utilizan para recibir correos electrónicos desde un servidor de correo a un cliente de correo.

- FTP (File Transfer Protocol):
      Transferencia de archivos: FTP se utiliza para transferir archivos entre un cliente y un servidor a través de una red. Facilita la copia de archivos de un sistema a otro.

# Pregunta 2

## ¿Cuáles son las capas del modelo tcp/ip? Explique brevemente cada una de ellas

# Pregunta 3

## ¿Qué es internet?

# Pregunta 4

## ¿Cuáles son algunos servicios que ofrece internet? Describa brevemente

# Pregunta 5

## ¿A qué se refiere la estandarización de las redes?

# Pregunta 6

## ¿Cuál es la función del ITU?

# Pregunta 7

## ¿Qué son ITU-T, la IETF y la ISO?

# Pregunta 8

## ¿En qué versión de la web cree que estamos? Justifique
