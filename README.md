
# Networks and Computer Security
>
> This repo was created to address some teorical questions about networks posed by the 'Networks and Computer Security' class.
>
>
> *Este repositorio fue creado para abordar algunas preguntas teóricas sobre redes planteadas por la clase 'Redes y Seguridad Informática'*.
>

# Pregunta 1

## ¿Cuáles son las funciones del protocolo tcp/ip?

TCP/IP es un conjunto de protocolos que **determina cómo los ordenadores transfieren datos** de un dispositivo a otro. *Estos datos deben ser exactos* para que el receptor obtenga la misma información enviada por el emisor.

Consta de varios protocolos individuales, y cada uno tiene funciones específicas. Pero los más importantes son:

- IP (Internet Protocol):
  - Direccionamiento:
      IP es responsable de **asignar direcciones únicas a cada dispositivo en una red IP**, lo que permite que los datos se enruten correctamente a su destino.
  - Enrutamiento:
      IP **determina la mejor ruta para que los paquetes de datos viajen desde el remitente hasta el destinatario** a través de una red de múltiples dispositivos interconectados.

- TCP (Transmission Control Protocol):
  - Control de flujo:
      TCP **asegura que los datos se transmitan de manera confiable y en orden** entre dos dispositivos. Esto se logra mediante la *numeración y el seguimiento de los paquetes de datos*, así como la *solicitud de retransmisión en caso de pérdida o daño de datos*.
  - Establecimiento y finalización de conexiones:
      TCP permite la creación de conexiones entre dos dispositivos a través de un "proceso de tres vías de apretón de manos (handshake)" y su cierre adecuado al finalizar la comunicación.
  - Segmentación y reensamblaje:
      TCP divide los datos en segmentos más pequeños para su transmisión y luego los **reensambla en el orden correcto en el destino**.

- UDP (User Datagram Protocol):
  - Transmisión sin conexión:
      A diferencia de TCP, UDP es un protocolo sin conexión que no garantiza la entrega de datos ni el orden. Es **útil para aplicaciones que requieren una transmisión rápida y no crítica de datos, como la transmisión de audio** y video en tiempo real.

- DNS (Domain Name System):
  - Resolución de nombres:
      DNS **se encarga de traducir nombres de dominio legibles por humanos** (como <www.mi-sitio.com>) en direcciones IP numéricas que las computadoras pueden entender y utilizar para localizar servidores en la red.

- HTTP (Hypertext Transfer Protocol):
  - Transferencia de hipertexto:
      HTTP es un **protocolo de la capa de aplicación utilizado para la transferencia de páginas web y otros recursos en la World Wide Web**. Facilita la solicitud y la respuesta entre navegadores web y servidores web.

- SMTP (Simple Mail Transfer Protocol) y POP/IMAP:
  - Correo electrónico:
      SMTP se utiliza para **enviar correos electrónicos desde un cliente de correo a un servidor de correo**, mientras que POP (Post Office Protocol) e IMAP (Internet Message Access Protocol) se utilizan para recibir correos electrónicos desde un servidor de correo a un cliente de correo.

- FTP (File Transfer Protocol):
  - Transferencia de archivos:
      FTP se utiliza para transferir archivos entre un cliente y un servidor a través de una red. Facilita la copia de archivos de un sistema a otro.

# Pregunta 2

## ¿Cuáles son las capas del modelo tcp/ip? Explique brevemente cada una de ellas

**El modelo TCP/IP estructura el problema de la comunicación en 5 capas relativamente independientes entre sí**.

### Capa física

Define la interfaz física entre el dispositivo de transmisión de datos (por ejemplo, la estación de trabajo) y el medio de transmisión o red.
Se encarga de las características del medio de comunicación.

### Capa de Acceso a la Red

Responsable del intercambio de datos entre el sistema final (servidor, estación de trabajo, etc.) y la red a la cual está conectado. El emisor debe proporcionar a la red la dirección del destino, de tal manera que esta pueda encaminar los datos hasta el destino apropiado. El emisor puede requerir ciertos servicios que pueden ser proporcionados por el nivel de red, por ejemplo, solicitar una determinada prioridad.
Se encarga de enviar un paquete desde nuestro equipo hasta el receptor.

### Capa de Internet

En situaciones donde los dispositivos estén conectadas a redes diferentes, se necesita una serie de procedimientos que permitan q los datos atraviesen distintas redes interconectadas; esta es la función de esta capa.
Se encarga de buscar la ruta necesaria para hacer llegar los paquetes a destinos.
En esta capa se utiliza el protocolo de internet (IP).

### Capa de Transporte (o capa de extremo a extremo)

Sin que importe la naturaleza de las apps que estén intercambiando datos, **es usual el requerimiento de que _los datos de intercambien de forma fiable**_. Esta capa revisa que los datos lleguen de manera "fiable". **Los mecanismos que proporcionan esta fiabilidad son independientes de la naturaleza de las aplicaciones**. Estos "mecanismos" se encuentran agrupados en esta única capa común.
Dentro de esta capa está el TCP, y es el más utilizado para proporcionar la fiabilidad necesaria.

### Capa de aplicación

Contiene toda la lógica necesaria para posibilitar las distintas aplicaciones de usuario.

# Pregunta 3

## ¿Qué es internet?

Conjunto descentralizado de redes de comunicación interconectados que utilizan la familia de protocolos TCP/IP, garantizando que las redes físicas heterogéneas que la componen funcionen como una red lógica única, de alcance mundial.

# Pregunta 4

## ¿Cuáles son algunos servicios que ofrece internet? Describa brevemente

1. **Navegación Web**: Permite a los usuarios acceder y explorar sitios web, blogs, foros y otras páginas en línea utilizando navegadores web como Google Chrome, Mozilla Firefox o Safari.

2. **Correo Electrónico**: Facilita el envío y recepción de mensajes y documentos a través de servicios de correo electrónico como Gmail, Outlook o Yahoo Mail.

3. **Redes Sociales**: Plataformas como Facebook, X, Instagram y LinkedIn permiten a las personas conectarse, compartir contenido, interactuar y comunicarse con amigos, familiares y colegas.

4. **Transmisión de Contenido Multimedia**: Servicios como Netflix, YouTube y Spotify ofrecen la transmisión de películas, videos, música y otros contenidos multimedia en línea.

5. **Comercio Electrónico**: Plataformas de comercio electrónico como Amazon, MercadoLibre y Alibaba permiten a los usuarios comprar y vender productos y servicios en línea.

6. **Banca en Línea**: Los servicios bancarios en línea ofrecen a los clientes acceso a sus cuentas bancarias, transferencias de dinero y pagos en línea de forma segura.

7. **Educación en Línea**: Plataformas como Coursera, edX y Udemy ofrecen cursos y recursos educativos en línea para el aprendizaje a distancia.

# Pregunta 5

## ¿A qué se refiere la estandarización de las redes?

# Pregunta 6

## ¿Cuál es la función del ITU?

# Pregunta 7

## ¿Qué son ITU-T, la IETF y la ISO?

# Pregunta 8

## ¿En qué versión de la web cree que estamos? Justifique
