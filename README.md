
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

Sin que importe la naturaleza de las apps que estén intercambiando datos, **es usual el requerimiento de que *los datos de intercambien de forma fiable***. Esta capa revisa que los datos lleguen de manera "fiable". **Los mecanismos que proporcionan esta fiabilidad son independientes de la naturaleza de las aplicaciones**. Estos "mecanismos" se encuentran agrupados en esta única capa común.
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

La estandarización de las redes se refiere a los estándares que se aplican y deben cumplir los distribuidores y proveedores de servicios de red.

Es un proceso de establecer conjuntos de reglas, protocolos y especificaciones técnicas comunes que garantizan la interoperabilidad y la compatibilidad entre dispositivos y sistemas de comunicación en una red de computadoras. Estos estándares son esenciales para que las redes funcionen de manera eficiente y efectiva, permitiendo que dispositivos de diferentes fabricantes y sistemas operativos se comuniquen entre sí de manera coherente y sin problemas.

Los estándares son solo reglas que definen como deben funcionar las cosas, permitiendo una uniformidad que es necesaria para que no haya problemas de compatibilidad.

# Pregunta 6

## ¿Cuál es la función del ITU?

La "International Telecommunication Union" es una agencia especializada de las Naciones Unidas que se encarga de coordinar y regular los asuntos relacionados con las telecomunicaciones y la tecnología de la información a nivel global. La UIT (siglas en español) desempeña un papel fundamental en el desarrollo y la estandarización de las tecnologías de la información y las comunicaciones (TIC) en todo el mundo.
Algunas de sus funciones principales son:

1. Desarrollo de Estándares: trabaja en el desarrollo y la promulgación de estándares técnicos que aseguran la interoperabilidad y la compatibilidad entre diferentes sistemas y redes de telecomunicaciones. Esto incluye estándares para protocolos de comunicación, compresión de datos, calidad de servicio, y otros aspectos tecnológicos clave.

2. Asignación de Espectro de Frecuencia: **asigna y regula el uso de las bandas de frecuencia del espectro radioeléctrico a nivel internacional**. Esto es esencial para garantizar que las comunicaciones inalámbricas, como la telefonía móvil, la radiodifusión y las comunicaciones satelitales, funcionen sin interferencias y de manera ordenada en todo el mundo.

3. Cooperación Internacional: Facilita la cooperación entre los países y las organizaciones en cuestiones relacionadas con las telecomunicaciones y la tecnología de la información. Ayuda a resolver disputas transfronterizas y fomenta la colaboración en proyectos internacionales.

4. Política y Regulación: Proporciona orientación y asesoramiento en la formulación de políticas y regulaciones relacionadas con las TIC. Esto incluye **cuestiones de privacidad, seguridad cibernética, acceso a la información y regulación de mercados** de telecomunicaciones.

5. Desarrollo de Capacidades: La UIT trabaja para **mejorar las capacidades técnicas y de gestión de los países en desarrollo** en el campo de las TIC. Esto incluye programas de formación, asistencia técnica y promoción del acceso a las TIC en todo el mundo.

6. Cumbres y Conferencias Mundiales: Organiza conferencias y cumbres mundiales sobre telecomunicaciones, como la Conferencia Mundial de Radiocomunicaciones (CMR) y la Cumbre Mundial sobre la Sociedad de la Información (CMSI), donde se discuten y establecen directrices globales en materia de TIC.

7. Investigación y Desarrollo: Fomenta la **investigación y el desarrollo en el campo de las telecomunicaciones y la tecnología de la información**, promoviendo la innovación y el avance tecnológico.

# Pregunta 7

## ¿Qué son ITU-T, la IETF y la ISO?

### ITU-T

La tarea del sector ITU-T es hacer recomendaciones técnicas sobre las interfaces de telefonía telegrafía y comunicación de datos. A menudo estas recomendaciones se convierten en estándares con reconocimiento internacional, aunque técnicamente las recomendaciones son sólo sugerencias que los gobiernos pueden adoptar o ignorar según lo deseen.

### IETF

La IETF (Internet Engineering Task Force) es una organización internacional y una comunidad abierta de ingenieros, diseñadores, operadores de redes y otros profesionales interesados en la evolución y el desarrollo de las tecnologías y protocolos de Internet. La IETF tiene un **enfoque específico en la creación de estándares abiertos y documentos técnicos que impulsan el funcionamiento, la seguridad y la interoperabilidad de Internet**.

La IETF desarrolla y promueve estándares de Internet, cuerpos estándares y referentes en particular a las normas del protocolo TCP / IP y el conjunto de protocolos de Internet.

La misión de la IETF está documentada en RFC (Request for Comments, o en español Solicitud de comentarios). Los RFC son una serie de notas sobre Internet. Cada una de ellas es un documento cuyo contenido es una propuesta oficial para un nuevo protocolo de la red Internet, que se explica con todo detalle para que, en caso de ser aceptado, pueda ser implementado sin ambigüedades.

Las principales características y funciones de la IETF incluyen:

1. **Desarrollo de Estándares**: trabaja en el desarrollo y la estandarización de protocolos y tecnologías clave para Internet. Esto incluye protocolos de comunicación como TCP/IP, HTTP, SMTP, DNS y muchos otros que son fundamentales para el funcionamiento de la red.
2. **Colaboración Abierta**: opera en un modelo de colaboración abierta y voluntaria, donde los expertos de todo el mundo pueden participar en grupos de trabajo y contribuir con sus conocimientos y experiencias. **No es una organización con membresía formal**, y cualquiera puede unirse a sus actividades.

3. **Reuniones y Listas de Correo**: La IETF organiza reuniones presenciales y mantiene listas de correo electrónico donde los participantes discuten y debaten los problemas técnicos y los estándares en desarrollo.

4. **RFC (Request for Comments)**: Los estándares desarrollados por la IETF se documentan en RFC, que son documentos técnicos que describen protocolos, prácticas y estándares relacionados con Internet. Los RFC son ampliamente reconocidos y utilizados en todo el mundo.

5. **Enfoque en la Capa de Aplicación**: Aunque la IETF aborda una amplia gama de temas relacionados con Internet, su **enfoque principal se centra en la capa de aplicación de la arquitectura de Internet**, lo que significa que se ocupan de protocolos y estándares utilizados en aplicaciones y servicios.

6. **Evolución Continua**: **se adapta y evoluciona constantemente para abordar los desafíos** cambiantes de Internet. A medida que surgen nuevas tecnologías y necesidades, la IETF trabaja en la creación de estándares que permitan la expansión y mejora de la red.

### ISO

Los estándares internacionales son producidos por la ISO (Organización Internacional de Estándares, del inglés International Standards Organization), una organización internacional independiente no gubernamental, surgida de un tratado y fundada en 1946. Sus miembros son las organizaciones nacionales de estándares de los 157 países miembros.

# Pregunta 8

## ¿En qué versión de la web cree que estamos? Justifique

Creo que nos encontramos aún en la versión 3 de la web, experimentando una web 3 desarrollada y madura, con grandes prestaciones, ya que el objetivo original de "crear sitios web más inteligentes, conectados y abiertos" está cumplido y con creces.

Ahora bien, se vislumbra una nueva forma de interconexión donde el rol de los usuarios cobra cada vez mayor protagonismo y las redes decentralizadas son la punta de lanza de esta nueva forma de interacción.
También se experimenta un crecimiento expoonencial de dispositivos inteligentes conectados a la web e interactuando entre ellos. Lo que proporciona una nueva forma de las personas de interactuar con el medio.
La inteligencia artificial parece estar en su boom inicial.
Los últimos 3 puntos me hacen pensar que estamos ante un cambio de época, pero aún falta para afirmar que efectivamente iniciamos la web 4.
