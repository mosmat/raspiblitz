![RaspiBlitz](pictures/raspilogo_tile_400px.png)

*Construye tu propio nodo para Bitcoin y red Lightning.*

`Versión 1.7.0 con lnd 0.12.1 y bitcoin 0.21.0 (o litecoin 0.18.1)`

![RaspiBlitz](pictures/raspiblitz.jpg)

**El Raspiblitz es un nodo para Bitcoin y Lightning del tipo hágalo-usted-mismo. Funciona corriendo LND al mismo tiempo que un Nodo-Completo de Bitcoin usando un RaspberryPi (con 1TB SSD de almacenamiento) y una cómoda pantalla para fácil instalación y monitoreo.**

Raspiblitz está orientado principalmente a aprender a correr un nodo descentralizado desde casa -porque, como dice el dicho: "si no es tu nodo, entonces no son tus reglas"-. Descubre y contribuye al desarrollo del ecosistema de la Red Lightning formando parte de ella. Puedes llevarlo a cabo mediante un [taller](WORKSHOP-ESLA.md) o como un proyecto personal para el fin de semana.

## Un vistazo a los servicios

Existen los siguientes servicios que puedes correr desde tu nodo:

* **Tor** (Corriendo como servicio incógnito) [details](https://en.wikipedia.org/wiki/Tor_(anonymity_network)#Onion_services)
* **ElectRS** (Servidor Electrs en Rust) [details](https://github.com/romanz/electrs)
* **BTCPayServer** (Procesador de pagos en bitcoin) [details](https://btcpayserver.org)
* **BTC-RPC-Explorer** (Explorador de la cadena de bloques de bitcoin) [details](https://github.com/janoside/btc-rpc-explorer)
* **LNbits** (Billeteras Relámpago(Lightning) / Sístema para contaduría y administración para proyectos y empresas) [details](https://twitter.com/lnbits/status/1253700293440741377?s=20)
* **SpecterDesktop** (Billeteras Cadena(On-Chain). Personales y multifirma. Funciona para Billeteras Hardware como ColdCard, Trezor y Ledger) [details](https://github.com/cryptoadvance/specter-desktop)
* **Lightning Terminal (Loop, Pool & Faraday)** (Administración de liquidez para Canales Relámpago) [details](https://github.com/lightninglabs/lightning-terminal#lightning-terminal-lit)
* **JoinMarket** (Servicio para Coinjoin) [details](https://github.com/JoinMarket-Org/joinmarket-clientserver)
* **ThunderHub** (Administrador para nodo con interfaz WEB) [details](https://www.thunderhub.io/)
* **Balance Of Satoshis** (Comandos para administrar y trabajar con la liquidez del nodo) [details](https://github.com/alexbosworth/balanceofsatoshis/blob/master/README.md)
* **Kindle Display** (Pantalla de estado para Bitcoin elaborado con un Kindle desbloqueado) [details](https://github.com/dennisreimann/kindle-display)
* **Stacking Sats Kraken** (Script para hacer auto compras) [details](https://github.com/dennisreimann/stacking-sats-kraken)
* **Circuit Breaker** (Cortafuegos para los Canales Relámpago) [details](https://github.com/lightningequipment/circuitbreaker/blob/master/README.md)
* **PyBlock**  (Utilería en Python y diversiones) [details](https://github.com/curly60e/pyblock/blob/master/README.md)
* **Mempool Explorer** (Explorador para la cadena de bloques de bitcoin. Valida tus propias transacciones. ) [details](https://github.com/mempool/mempool)
* **Sphinx Chat Relay Server** (Servicio para la app de mensajería y transmisión SphinxChat) [details](https://github.com/stakwork/sphinx-relay/blob/master/README.md)
* **Telegraf metrics** [details](https://github.com/rootzoll/raspiblitz/issues/1369)
* **Chantools** (Fund Rescue) [details](https://github.com/guggero/chantools/blob/master/README.md)

Puedes conectar las siguientes aplicaciones-billetera con tu nodo:

* **Zeus** (Android & iOS-TestFlight) [details](https://zeusln.app)
* **Fully Noded** (iOS) [details](https://apps.apple.com/us/app/fully-noded/id1436425586)
* **SendMany** (Android) [details](https://github.com/fusion44/sendmany/blob/master/README.md)
* **Sphinx Chat App** (Android & iOS) [details](https://sphinx.chat)


Además, otras características como Pantalla Táctil, Autopiloto, DNS Dinámico, Túneles SSH, Soporte para UPS, ...


## Video descriptivo (Inglés, Julio 2020)

<a href="https://www.youtube.com/watch?v=QXUGg45CWLo" target="_blank"><img src="pictures/raspiblitz-deepdive.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=QXUGg45CWLo

## Tiempo necesario para montar un Raspiblitz

El Raspiblitz está optimizado para ser montado durante la duración de una conferencia o un taller-repentina (Mira los detalles en [tutorial para talleres](WORKSHOP-ESPLA.md)). Si se trata de montar una copia de la cadena de bloques actualizada, es posible tener un nodo listo en 2 a 3 horas; la mayor parte de la duración de la instalación se trata de tener paciencia.

Si empiezas desde casa ordenando las partes desde Amazon, (mira la lista de compras más abajo) entonces se tratará de un proyecto de fin de semana con un montón de datos por descargar y sincronizar. Puedes hacer otras cosas mientras vigilas los avances de vez en cuando. 

Si actualmente ya cuentas con un nodo como el de Umbrel o myNode, básicamente cuentas con el hardware necesario y podrás correr una [Migración de Raspiblitz desde Umbrel/myNode](#haz-un-raspiblitz-con-tu-umbrel-o-mynode.md) en menos de una hora.

## Hardware Necesario

Todas las partes necesarias cuestan aproximadamente 180-250 USD; según tiendas y localización.

### Compra un RaspiBlitz listo para montar (Alemania, Estados Unidos e Internacional)

Si gustas apoyar el proyecto, puedes ordenar un nodo Raspiblitzo listo para echar a andar con todos los componentes necesarios requeridos para el taller de [raspiblitz.com](https://raspiblitz.com)

Ecuentra una lista de revendedores localizados al rededor del mundo en [raspiblitz.org](https://raspiblitz.org/).

### Lista de compras de Amazon (para comprar las piezas necesarias y hacerlo-usted-mismo)

La forma más barata de correr un nodo es comprando y montando las partes necesarias por piezas. A continuación dos opciones:

*Es importante que se utilicen los modelos exactos de hardware que están recomendados en la lista de compras. Hemos tenido múltiples reportes donde, por ejemplo, algúnos tipos de SSD, cables, carcasas o controladores conllevan a problemas. La idea de la lista de compras es recomendar componentes que han sido probados y que funcionan mejor con el proyecto. Comentarios y recomendaciones son bienvenidos.*


* RaspberryPi 4 4GB (or 8GB) [amazon referral link](https://geni.us/raspiblitz-4gb-new)
* Power Supply - USB-C, 5V, >=3A [amazon referral link](https://geni.us/raspiblitz-ps)
* 1TB SSD - SanDisk SSD Plus 1TB 2.5" : [amazon referral link](https://geni.us/raspiblitz-1000gb-san) *other 1TB SSD models might cause power issues*
* SSD-case - UGREEN 2.5" External USB 3.0 Hard Disk Case with UASP support : [amazon referral link](https://geni.us/raspiblitz-ssd-case)
* MicroSDCard 32GB - Samsung PRO Endurance 32 GB microSDHC UHS-I U1: [amazon referral link](https://geni.us/raspiblitz-sc-card)
* Heatsink Case for RPi4 : [amazon referral link](https://geni.us/heatsink-raspi4)
* LCD - 3.5" RPi Display, GPIO connection, XPT2046 Touch Controller: [amazon referral link](https://geni.us/raspiblitz-touchscreen)

*Si la mencionada pantalla está fuera de venta o agotada, puedes probar con alguna de las siguientes:*
  - Quimat 3,5'' Zoll Inch Touch
  - ELEGOO Display 3.5" Zoll TFT LCD
  - kuman 3.5 Inch Touch Screen TFT Monitor
  - Waveshare 3.5inch Display for Raspberry Pi 

*Por cierto, puedes pagar las piezas de Amazon utilizando bitcoin a través de [Bitrefill](https://blog.bitrefill.com/its-here-buy-amazon-vouchers-with-bitcoin-on-bitrefill-bb2a4449724a).*

[What other case options do I have?](FAQ.md#what-other-case-options-do-i-have)

## Ensambla tu Raspiblitz

Una vez que tienes todas las piezas, lo siguiente es:

- Colocar los disipadores de calor en la RaspberryPi (sigue las instrucciones del paquete)
- Conectar el disco SSD/HDD en su carcasa y conectarlo a su puerto usb correspondiente (color azul).
- Conectar la pantalla sobre los pins como se muestra en la foto, más abajo.
- Conectar el cable del internet. 

Al final, tu Raspiblitz debe verse algo parecido:

![HardwareSetup](pictures/hardwaresetup.jpg)

## Descarga el Software

Hay dos maneras en las que puedes instalar el software de Raspiblitz en tu nodo:

|Método|Instación de imágen de archivo|Recopilar la microtarjeta SD|
|------|-----------------|-----------------|   
|Filosofía|Confianza|Soberanía|
|Nivel de Dificultad|Fácil|Medio|
|Pros|Hace el proyecto disponible para todos|Puedes recopilarlo por ti mismo sin necesidad de confiar en nosotros|
|Contras|Tienes que confiar en quiénes mantienen el proyecto|Tienes que leer y entender los parámetros del archivo build_sdcard.sh para poder modificar el proyecto a tus necesidades|
|Instrucciones|[Descarga la imagen](https://raspiblitz.fulmo.org/images/raspiblitz-v1.7.0-2021-04-25.img.gz) y [Flashea el sistema operativo](README.md#write-the-sd-card-image-to-your-sd-card)|[Recopila tu propia imagen SD](#build-the-sd-card-image)|
|Verifi... ¿Qué?|[Archivo de firma](https://raspiblitz.fulmo.org/images/raspiblitz-v1.7.0-2021-04-25.img.gz.sig) y [Verificación de la firma](FAQ.md#how-to-verify-the-sd-card-image-after-download) o SHA-256 (abajo)|Así es. Todo el código. No confíes; verífica|

Se descargaste la más actual imagen en mantenimiento:
* GPG 64-bit: 1C73 060C 7C17 6461
* SHA-256: e6d70ac1662af3e90e57bee8c50e9a7925239431892e1916c2be80e519befc3f

¿Qué método de verificación debería utilizar: Hash o Signature?
* El archivo firmado comprueba que tu copia de la imagen SD fue realmente recopilado por los desarrolladores del proyecto Raspiblitz. (Método más seguro)
* La función hash comprueba la integridad del archivo. (Poco menos seguro)

El archivo de imagen también puede ser descargado vía torrent:
* [assets/raspiblitz-v1.7.0-2021-04-25.img.gz.torrent](https://github.com/rootzoll/raspiblitz/raw/v1.7/home.admin/assets/raspiblitz-v1.7.0-2021-04-25.img.gz.torrent)

Información valiosa:
* [¿Qué hay de nuevo en la versión 1.7.0 del Raspiblitz?](CHANGES.md#whats-new-in-version-170-of-raspiblitz)
* [¿Cómo actualizo mi Raspiblitz?](README.md#updating-raspiblitz-to-new-version)
* [¿Cómo migrar desde Umbrel o myNode?](#make-a-raspiblitz-out-of-your-umbrel-or-mynode)
* [¿Cómo verificar el archivo de imagen para memoria SD después de haberlo descargado?](FAQ.md#how-to-verify-the-sd-card-image-after-download)

## Flashea el archivo de imagen en tu microtarjeta SD

Necesitas escribir el archivo de imagen descargado (el archivo con extensión .gz) a tu microtarjeta SD (de 16GB como mínimo). Puedes utilizar la herramienta Balena Etcher para hacerlo: https://www.balena.io/etcher/ . Está disponible tanto para Windows como Mac y Linux.

## Arranca tu RaspiBlitz

Inserta la microtarjeta SD y conecta el alimentador de energía.

* Asegúrate de haber conectado el cable de internet LAN*
* Asegúrate de que tu Raspberry y tu computadora se encuentren en una misma red.

**Problemas más comúnes:**

* [No tengo puerto LAN en mi laptop... ¿Cómo me conecto al Raspiblitz?](FAQ.md#i-dont-have-a-lan-port-on-my-laptop---how-to-connect-to-my-raspiblitz)
* [¿Es posible conectarse al Raspiblitz por WiFi en lugar de LAN?](FAQ.md#is-it-possible-to-connect-the-blitz-over-wifi-instead-of-using-a-lan-cable)
* [¿Puedo conectartme directamente al Raspiblitz desde mi laptop?](FAQ.md#can-i-directly-connect-the-raspiblitz-with-my-laptop)
* [Conecté mi disco duro HDD y la pantalla todavía dice que debo conectar un disco](FAQ.md#i-connected-my-hdd-but-it-still-says-connect-hdd-on-the-display)

Cuando todo arranque correctamente, deberás ver la dirección IP local de tu Raspiblitz en la pantalla.

- [¿Cómo encuentro la dirección IP de mi Raspiblitz si no estoy utilizando una pantalla?](FAQ.md#how-do-i-find-the-ip-address-when-running-without-a-display)

![LCD0](pictures/lcd0-welcome.png)

Lo siguiente es abrir una términal ([OSX](https://www.youtube.com/watch?v=5XgBd6rjuDQ)/[Win10](https://www.howtogeek.com/336775/how-to-enable-and-use-windows-10s-built-in-ssh-commands/)) y conectarse mediante SSH con la información mostrada en la pantalla del RaspiBlitz:

`ssh admin@[TUDIRECCIONIP]` → utiliza la contraseña: `raspiblitz`

**Después sigue los diálogos en tu términal. Esto puede tomar algún tiempo, así que prepara algo de café. Al final, tendrás listo un nodo en tu RaspberryPi con el que podrás aprender a usar la Lightning Network y hacer trucos**

* [No puedo conectarme mediante SSH a mi Raspiblitz. ¿Qué hago ahora?](FAQ.md#i-cannot-connect-per-ssh-to-my-raspiblitz-what-to-do)

## Soporte

Si te encuentras con algún problema o todavía tienes preguntas, sigue los pasos a continuación para obtener ayuda. También revisa la [documentación detallada](#setup-process-detailed-documentation) para tener más claro el proceso de instalación.

1. Revisa las [Preguntas Más Frecuentes](FAQ.md) si todavía tienes dudas al respecto.

2. Si tienes problemas con el hardware, asegúrate de que conseguiste los mismos modelos mencionados en la lista de compras mencionada más arriba. Diferentes pantallas o incluso, discos duros distintos pueden causar problemas.

3. Hay un grupo de Telegram en donde los usuarios de Raspiblitz nos echamos la mano: https://t.me/raspiblitz. También existe un grupo para usuarios de habla hispana: https://t.me/raspiblitz_es. 


4. Asegúrate de identificar si tu problema o pregunta corresponde al proyecto Raspiblitz o, por ejemplo, al servicio LND. Es decir, si tienes problemas para enrutar pagos u obtienes erroes al abrir canales, entonces se trata de problemas con el servicio LND y será mejor si consultas con la comunidad desarrolladora del servicio LND: https://dev.lightning.community

5. Anda a la sección de asuntos (Issues) en el Github de RaspiBlitz: https://github.com/rootzoll/raspiblitz/issues para hacer una búsqueda ahí. Recuerda buscar asuntos cerrados removiendo el filtro 'is:open' del cuadro de diálogo de la búsqueda.

6. Si todavía no encuentras respuesta, publica un nuevo asunto en los Issues del Github de Raspiblitz. Tendrás que registrarte una cuenta de Github para esto. Si se trata de un bug en el Raspiblitz, por favor, copa y pega un enlace del Reporte Debug a tu asunto (ver [Preguntas más frecuentes](FAQ.md) para que sepas como se obtiene). Las fotos o captura de pantalla también son útiles para que la comunidad entienda mejor tu problema. 

## Proceso de instalación (Documentación detallada)

*El objetivo es que toda la información necesaria para interactuar con el Raspiblitz está incluída durante la instalación. La documentación de este capítulo es para apoyo, educadores y para algunos casos excepcionales.*
 
Si estás buscando el tutorial para organizar un taller, [mira aquí](WORKSHOP.md).

### Init

Al principio puedes elegir el tipo de instalación para tu Raspiblitz. Puede correr Bitcoin o Litecoin en la Red Lightning. Esto también aplica si estás importanto el archivo de migración desde un Raspiblitz desactualizado. Lee más sobre la migración [más abajo](README.md#import-a-migration-file). La opción por defecto es Bitcoin. 

![SSH0](pictures/ssh0-welcome2.png)

Lo primero es ponerle un nombre a tu Raspiblitz:

![SSH1](pictures/ssh1-name.png)

Este nombre se asigna al Raspiblitz como alias público de nodo para que otros participantes dentro de la red lo identifiquen.

Después, será necesario que asignes 4 contraseñas:

![SSH2](pictures/ssh2-passwords.png)

Puedes usar esta [Hoja de ayuda para contraseñas Raspiblitz (PDF)](https://github.com/rootzoll/raspiblitz/raw/v1.4/home.admin/assets/RaspiBlitzRecoverySheet.pdf) para escribir las contraseñas y también para escribir y guardar tus Palabras Semilla más adelante.

*Las contraseñas A,B,C & D están basadas en el proyecto [Guía de preparación RaspiBolt](https://stadicus.github.io/RaspiBolt/raspibolt_10_preparations.html#write-down-your-passwords). Revísalo para más información*

Entonces, te será requerida la contraseña A:

![SSH3a](pictures/ssh3a-password.png)

Esta es la nueva contraseña que será utilizada cada vez que te conectes al Raspiblitz mediante SSH. También servirá como contraseña para los usuarios: root, bitcoin y pi.

*Los servicios Bitcoin y Lightning estarán corriendo en el background (como Daemons) bajo el usuario "bitcoin" por medidas de seguridad. Este usuario no tiene permisos de Administrador y no podrá hacer cambios a la configuración del sístema.*

Después deberás ingresar la Contraseña B. Esta se utiliza para la interfaz RPC de bitcoin y para acceder a algunas aplicaciones como RTL, Specter o Blockexplorer:

![SSH3b](pictures/ssh3b-password.png)

*Las contraseñas C y D serán requeridas después. Van a ser necesarias para configurar la billetera Lightning LND.*

A continuación el proceso tomará un poco más de tiempo; la pantalla arrojará un montón de mensajes rápidos. Solo espera hasta que termine:

![SSH4](pictures/ssh4-scripts.png)

### Obteniendo la Cadena de Bloques (Blockchain)

*Si ya cuentas con una copia de la Blockchain en tu disco duro, (por ejemplo, en tu computadora personal o la de un amigo) cuentas con la opción de confiar en esa información y saltarte hasta [el siguiente paso](#Instalando-Lightning). Si empezaste con disco duro vacío, te aparecerán los siguientes diálogos:*

Si conectaste un disco duro nuevo al Raspiblitz, te va a preguntar si estás de acuerdo en formatearlo.

<img src="pictures/ssh4-formatHDD.png" alt="format-HDD" width="366">

*Tu disco duro será formateado usando el sístema estándar de Linux EXT4. Si quieres utilizar el formato experimental [BTRFS](FAQ.md#why-use-btrfs-on-raspiblitz) que el Raspiblitz soporta desde la versión v1.4, necesitarás iniciar el proceso con una memoria adicional de 32GB conectado al segundo puerto USB3 del RaspberryPi. Así desbloquearás este logro secreto.*

Despues del formateo obtendrás una copia de la cadena de bloques; Raspiblitz ofrece las siguientes opciones:

<img src="pictures/ssh5-blockchain2.png" alt="blockchain-options" width="551">

Las opciones, y cuando usar cada una, serán explicadas brevemente a continuación:

#### 1. SYNC - Autovalidación de bloques

Si cuentas con el nuevo RaspberryPi 4 (con SSD y mínimo 2GB de RAM) esta es la mejor manera de validar la blockchain. Tomará al rededor de 2 o 3 días sincronizar y validarla directamente desde la red de bitcoin. Esta es la opción mejor conocida como `No te confíes, verifícalo`. 

*Para el modelo más viejo RaspberryPi 3, esto no es recomendable. Un Raspberrypi 3 tiene poco poder de CPU y la validación persona-a-persona de la cadena de bloques puede tardar hasta varias semanas. Por eso es mejor utilizar una copia de la cadena de bloques previamente lista y validada mediante la opcion COPY.*

#### 2. COPY - Copia la blockchain desde tu computadora, laptop, o el Raspiblitz de un amigo a través de tu red local.

Primero necesitas descargar y validar la blockchain en tu computadora o laptop. Puedes instalar bitcoin-core (0.18.1 o superior) desde [bitcoin.org](https://bitcoin.org/en/download) y dejarlo correr hasta que la blockchain se sincronice y se valide por completo. (necesitarás alrededor de 320 GB).

Después puedes usar la opción COPY para copiar la blockchain hacia tu Raspiblitz. Puedes hacer esto mediante el comando SCP (transferencia de archivo SSH) siguiendo las instrucciones en pantalla.

Es recomendable mantener bitcoin-core y la información de la blockchain actualizada tanto como sea posible en tu computadora/laptop en caso de que necesites montar de nuevo otro Raspiblitz.

Para más detalles: [Tengo una copia completa de la blockchain en otra computadora. ¿Cómo se lo paso a mi Raspiblitz?](FAQ.md#i-have-the-full-blockchain-on-another-computer-how-do-i-copy-it-to-the-raspiblitz)

### Configurar Lightning

Para entonces, Lightning ya está instalado y listo para recibir tu configuración si te aparece la siguiente pantalla:

![SSH7](pictures/ssh7-lndinit.png)

Ahora puedes decidir si quieres una billetera nueva o si quieres recuperar una vieja desde algún Raspiblitz (o nodo) que tuvieras antes.

#### Configurando una billetera NUEVA

Esta es la opción default si comienzas con un Raspiblitz por primera vez.

![SSH8](pictures/ssh8-wallet.png)

Raspiblitz te preguntará configurar tu contraseña para desbloquear la billetera. Utiliza la CONTRASEÑA C. Confirma ingresándola una segunda vez. 

LND ahora generará una Frase Semilla nueva (lista de palabras) para ti.

![SSH8](pictures/ssh8-walletb.png)

ESCRIBE TUS LISTA DE PALABRAS antes de que continúes. Sin ellas, disminuyes las posibilidades de recuperar tus fondos en caso de fallas de hardware u otras razones. Si solo se trata de probar y experimentar con el Raspiblitz, por lo menos toma una foto con tu smartphone, por si acaso. Si piensas mantener tu nodo corriendo, guarda la lista de palabras FUERA DE LÍNEA (esto significa, no fotos, no copia de word, no copia en dropbox, google drive, mensaje de whatsapp, y por el estilo) y en un lugar seguro. Puedes utilizar el [RaspiBlitz Password Sheet (PDF)](https://github.com/rootzoll/raspiblitz/raw/v1.4/home.admin/assets/RaspiBlitzRecoverySheet.pdf) para esto.

#### Recupera una billetera VIEJA

Escoge esta opción si ya cuentas con un viejo Raspiblitz o nodo que desees recuperar. Tienes tres opciones:

![SSH7](pictures/ssh7-lndrecover.png)

El Raspiblitz ejecutando el comando de creación de billetera LND:

##### LNDRESCUE LND tar.gz-Backupfile (MEJOR OPCIÓN) 

Escoge esta opción si cuentas con una copia de respaldo de la información LND en un archivo del tipo tar.gz llamado 'lnd-rescue'. Recuperará tus fondos on-chain y abrirá los canales que ya tenías disponibles. Tienes que asegurarte de que realmente sea la más reciente copia de la inormación LND; de otro modo, podrías perder la liquidez de los canales.

*Si tienes un archivo tar.gz que comienza con 'raspiblitz', ese es el archivo de migración. Ese archivo también incluye tu vieja billetera LND que has importado poco antes durante el proceso... mira más detalles abajo.*

##### SEED+SCB Palabras Semilla & archivo channel.backup (SEGUNDA MEJOR OPCIÓN) 

La siguiente mejor opción es si cuentas con tu archivo channel.backup y tu lista de palabras semilla. Esta es la mejor oportunidad que tienes para recuperar tus fondos on-chain que tenías para canales abiertos y en línea. Ten en cuenta que los canales van a cerrarse antes de hacer la recuperación de fondos.

##### ONLY SEED Únicamente Palabras Semilla (RESPALDO)

Si únicamente cuentas con tu lista de palabras (RaspiBlitz 1.1 o más viejas) puedes intentar al menos recuperar tus fondos on-chain. Recuperar los fondos de los canales es poco probable en este escenario.

### Configuración LND final

El sistema ahora verificará que la billetera se haya iniciado correctamente y te pedirá desbloquearla con la CONTRASEÑA C.

![SSH9c](pictures/ssh9c-unlock.png)

*La billetera LND necesita desbloquearse cada que enciendes o reinicias tu Raspiblitz.*

El Raspiblitz ahora realizará una configuración final. Instalará herramientas, moverá archivos SWAP al disco duro, activará cortafuegos, entre otras cosas. Verás un montón de texto a través de la pantalla mientras esto sucede:

![SSH9b](pictures/ssh9b-reboot.png)

La configuración básica está lista... pero aún faltan algunos detalles previos a que comiences a disfrutar tu Raspiblitz. Presiona 'OK' para reiniciar. Tu sesión en la terminal se desconectará y el RaspberryPi se reiniciará.

### Primer arranque: sincronización y escaneo.

Después del reinicio, tomará un pequeño tiempo para que los servicios arranquen. Espera hasta que la pantalla te solicite desbloquear la billetera LND. Deberás conectarte al Raspiblitz mediante SSH como al inicio del tutorial (revisa la pantalla LCD) pero esta vez, y de ahora en adelante, te solicitará tu CONTRASEÑA A.

Después de iniciar sesión, LND te va a pedir (como en cada arranque/reinicio) desbloquear la billetera. Utiliza la CONTRASEÑA C:

![SSH9c](pictures/ssh9c-unlock.png)

Durante la primera vez tendrás un periodo de espera más largo, (más o menos 10 minutos hasta 2 o 3 días, si has mantenido apagado tu Raspiblitz o si es la primera vez que lo inicias) pero no te preocupes. Déjalo correr hasta que esté listo.

![SSH9d1](pictures/ssh9d-sync.png)

*Incluso puedes cerrar la terminal y apagar tu laptop o computadora y volver a hacer inicio de sesión SSH para ver cómo van las cosas. Cuando la pantalla con fondo azul se vaya, aparecerá el informe del estado de tu nodo.*

Para entender porque está tomando tanto tiempo, se debe a dos cosas:

1. Sincronización de la blockchain.

La copia de la blockchain en tu disco duro no está completamente actualizada. Dependiendo de cuanto tiempo te tomó transferir la información hacia la Raspiblitz, existirá un retraso de un par de horas; quizá un par de días. Así que ahora la Raspiblitz necesita ponerse al corriente con el resto de la red hasta que alcance la sincronía del 100%. Incluso si parece congelado a 99.8%, aún requiere tiempo de espera. Avanzar un simple 1% podría tomar hasta cuatro horas (dependiendo de la velocidad de la red) así que mejor se paciente.

2. Escaneo Lightning

Si la sincronía de la blockchain está en progreso, LND comenzará a recopilar la información necesaria. El escaneo lightning toma 1 hora aproximadamente, pero puede tardar más si recuperaste una vieja billetera desde las palabras semilla.

* [¿Por qué mi sincronización está tomando demasiado?](FAQ.md#why-is-my-final-sync-taking-so-long)

Una vez que todo está listo, debería aparecer el informe de estado de la Raspiblitz en la pantalla LCD como se mira a continuación:

![SSH9dz](pictures/ssh9z-ready.png)

### Menú principal

Si haces login SSH en tu Raspiblitz (o si todavía estás con la sesión activa) podrás ver el Menú Principal (Main Menu):

![SSH9e1](pictures/mainmenu.png)

Todas las opciones del menú se explican a continuación.

*A partir de este punto tu Raspiblitz ya está listo para jugar.*

Si necesitas una idea básica de como las cosas funcionan, sería más o menos:

* Depositar fondos on-chain
* Abrir canales
* Realizar pagos y cobros

Si prefieres utilizar una interfaz de navegador en lugar de la terminal SSH, ve a la opción `SERVICES` y activa el servicio `RTL Webinterface` o el servicio `THUNDERHUB` y después de un reinicio verás las opciones `RTL` o `Thunderhub` en el menú principal. Al seleccionar cualquiera, te mostrará a continuación la información necesaria para comenzar a utilizarlos.

Que te diviertas en la red Lightning :D

*Por cierto, siempre es grato ver fotos de Raspiblitzes nuevos participando en la red. Si montas uno nuevo etiqueta en twitter a @rootzoll. También hay una [Página de donación Raspiblitz](https://tallyco.in/s/r5lx23/), puedes probar tu nuevo nodo lightning mandándonos una propina :D*

* [¿Cómo puedo obtener ayuda extra?](#support)

### Documentación de características

Las siguientes son características disponibles a través del menú SSH de la Raspiblitz. Cada uno ofrece algúnas formas básicas de funcionamiento y respaldo. A veces es mejor realizar operaciones complicadas utilizando las aplicaciones y scripts en tu nodo mediantes el uso de [APIs](#interface--apis) aprovechando que ahora cuentas con un nodo Bitcoin y Lightning en tu RaspiBlitz.

Vamos a ver el menú SSH principal a detalle:

#### INFO: Información de estado de la Raspiblitz

Esta es la información que se muestra en la pantalla LCD. Es útil para checarlo mediante SSH cuando estás lejos de tu Raspiblitz o por si quieres consultar tu información rápidamente o hacer una captura de pantalla. 

![SSH9dz](pictures/ssh9z-ready.png)

*No se actualiza todo el tiempo; es para una sola consulta.*

* [¿Por qué mi dirección IP de bitcoin aparece en color rojo?](FAQ.md#why-is-my-bitcoin-ip-on-the-display-red)
* [¿Por qué la dirección de mi nodo aparece en color rojo?](FAQ.md#why-is-my-node-address-on-the-display-red)
* [¿Por qué la dirección de mi nodo aparece en color amarillo?](FAQ.md#why-is-my-node-address-on-the-display-yellow-not-green)

#### LIGHTNING: Administración básica de nodo

En la opción `LIGHTNING` encontrarás los comandos básicos para administrar tu nodo. Son los más sencillos de utilizar para ir aprendiendo sobre la marcha. Para un control más avanzado, echa un vistazo a la opción 'SERVICES'.

##### FUNDING: Deposita fondos a tu billetera on-chain.

Antes de que puedas abrir canales, necesitas tener algunas monedas en tu billetera LND. Utiliza esta opción para generar una dirección de cobro.

*Recuerda: Raspiblitz y LND se encuentran todavía en fase de desarrollo. Si depositas fondos en tu nodo es porque reconoces el riesgo de perderlos. Así que utiliza cantidades pequeñas que no te incomoda arriesgar. También, es una buena práctica para la privacidad [hacer coinjoin con tus monedas](https://bitcoin-only.com/#privacy) antes de mandarlas a una billetera LND.*

Puedes depositar en más de una ocasión. LND siempre va a generar direcciones de cobro distintas, pero todos los depósitos que recibas llegarán a la misma billetera LND.

##### CONNECT: Conectarse a algún compañero (Peer)

Antes de abrir algún canal, necesitas conectar con el compañero usando su dirección pública.

Abrir un canal con un compañero es opcional. Mantener conectado a compañeros confiables permite mantenerte en sincronía con la información recopilada en la blockchain. Ayudará a tu nodo a encontrar mejores rutas para completar transacciones satisfactoriamente.

##### CHANNEL: Abre un canal con algún compañero

Para abrir un canal de pagos, puedes utilizar esta opción.

Encuentra nodos interesantes para abrir canales a través de directorios como [1ML.com](https://1ml.com/), o únete al canal de Telegram de Raspiblitz para conocer más usuarios y abrir canales con algúno de ellos: https://t.me/raspiblitz (inglés) https://t.me/raspiblitz_es (español)

Ten en cuenta que el canal queda público y disponible para formar parte de la infraestructura de la red. Si tu intención es abrir un canal privado, debes abrir el canal mediante el comando de línea utilizando la opción `-private`. Sin embargo, un canal privado no puede formar ser considerado para enrutar transacciones de otros usuarios de la red. 

*El siguiente es un script shell bastante básico. Para obtener más control, prueba con el servicio (opción `SERVICIOS`) RTL webinterface o conecta tu nodo a una aplicación para smartphone (opción `CONNECT` y luego `MOBILE`).*

##### SEND: Paga una factura/Orden de pago

Paga una factura mediante la red Lightning.

*El siguiente es un script shell bastante básico. Para obtener más control, prueba con el servicio (opción `SERVICIOS`) RTL webinterface o conecta tu nodo a una aplicación para smartphone (opción `CONNECT` y luego `MOBILE`).*

Si buscas algo interesante para pagar a través de lightning ... ¿por qué no... [donar algunos satoshis para el mantenimiento de Raspiblitz?](https://tallyco.in/s/r5lx23/)? ¡Gracias! :)

##### RECEIVE: Crear Factura/Recibo de pago

Genera un recibo u orden de pago para recibir una transferencia a través de la red Lightning.

*El siguiente es un script shell bastante básico. Para obtener más control, prueba con el servicio (opción `SERVICIOS`) RTL webinterface o conecta tu nodo a una aplicación para smartphone (opción `CONNECT` y luego `MOBILE`).*

#### lnbalance: Detalle de balances de la billetera

<img src="pictures/bonus-lnbalance.png" alt="bonus-lnbalance" width="600">

#### lnchannels: Lista de tus canales lightning

<img src="pictures/bonus-lnchannels.png" alt="bonus-lnchannels" width="600">

#### lnfwdreport: Reporte de tus ganancias por enrutar pagos

Tu nodo puede funcionar como "Nodo Enrutador" y cobrar una comisión por las transacciones enrutadas a través de tus canales. Otros usuarios podrían seleccionar tu nodo y tus canales como parte de su ruta para realizar una transferencia. Este menú ofrece un reporte de las ganancias según el periodo de tiempo que desees consultar.

Recuerda: ganar comisiones por enrutar transacciones no sucede automáticamente; requiere un poco de esfuerzo y dedicación. Puede ser díficil construir una reputación atractiva para que la gente se anime a abrir canales hacia tu nodo o para escoger tu nodo como hub enrutador de transferencias. Checa tutoriales en internet del tipo "lndmanage" para darte una idea de como analizar y mejorar el mantenimiento de nodo y canales.

##### NAME: Cambia el nombre de tu Nodo

Aquí puedes cambiar el nombre de tu nodo para que el resto de la red te identifique. La red guarda tus nombres de nodo pasados; no es lo mismo el alias o nombre de nodo que la dirección pública de tu nodo. 

##### CLOSE ALL: Cierra todos los canales activos

*La opción está disponible solo si tienes canales activos.*

Con esta opción puedes cerrar los canales y recuperar los fondos con los que abriste tus canales.

Puedes escoger la opcion force-close sobre canales donde tu compañero ya no se encuentra al alcance. Recuerda que cuando eliges esta opción, podría tomar mucho más tiempo para que tus fondos vuelvan a estar disponible en tu billetera on-chain.

##### CASHOUT: Retira los fondos de tu billetera on-chain.

Úsalo si quieres retirar los fondos de tu nodo. Recuerda que para retirarlos todos, tienes que cerrar los canales activos primero.

#### SETTINGS: Opciones básicas de Raspiblitz

Aquí encontrarás las opciónes básicas para tu RaspiBlitz:

![MainMenu-Settings](pictures/settings.png)

Activa y desactiva opciones con la barra de espacio del teclado y después elije `OK` para activar los cambios. A continuación más detalles sobre cada opción:

##### Correr nodo con Tor

Puedes correr tu nodo Bitcoin y Lightning; así como otras apps y servicios, reemplazando tu IP tradicional con una dirección .onion. Recomendable para mantener tus servicios de forma privada.

![tor1](pictures/tor1.png)

Correr tu nodo como servicio Tor tiene los siguientes beneficios:

* No das a conocer tu IP pública por lo que es más complicado revelar tu nombre real y locación.
* Haces túnel a través del NAT de tu router y vuelve accesible Bitcoin y Lightning para todos los otros nodos Tor.
* Usando una dirección Tor es posible moverte a otra IPv4 distinta sin comprometer las funciones de tus canales.

Pero también puede provocar algunos efectos secundarios:

* Algunas aplicaciones para celular todavía no soportan los servicios Tor.
* Otros nodos corriendo con IP pública regular no podrán dar contigo a menos que tu lo hagas primero hacia ellos.

Para probarlo, marca la casilla. Puedes desactivarlo y volver a la normalidad más adelante.

##### Pantalla táctil (experimental)

Tu Raspiblitz tiene un menú táctil listo para andar. Puedes activar esta opción; pero se encuentra aún en desarrollo.

![RTL](pictures/touchscreen.png)

Te dará cuatro botones al lado derecho de la pantalla.

- Info 
- Node - muestra el id del nodo/uri como un código QR (necesario para abrir canales desde aplicaciones móviles)
- Recibo - Crea un recibo en código QR para recibir transferencias vía lightning.
- Off - Apaga o reinicia tu RaspiBlitz

##### LCD Rotate

Para rotar 180 grados la pantalla del nodo. Útil para carcasas especiales o si piensas montarlo en algún mobiliario o muro. 

##### Autopiloto para canales

El autopiloto para canales de LND ofrece una automatización para manejar tus fondos y abrir canales con otros nodos en la red. 

Es útil si quieres comenzar a utilizar la red Lightning sin complicaciones, en especial si no quieres lidiar con toda la parte técnica.
Es posible que una vez que te acostumbres al mantenimiento de nodo y canales, ya no sea necesario utilizar el autopiloto.

Ten en cuenta que al activar el autopiloto, tendrás que reiniciar el nodo. Más información en: [Improvement request #1953](https://github.com/rootzoll/raspiblitz/issues/1953)

##### Accept Keysend

Keysend es una opción para que LND te permita aceptar pagos sin necesidad de crear una factura. Útil para tener tu wallet de donaciones y propinas. También es necesario para utilizar funciones experimentales de mensajería sobre la Red Lightning. (mira aplicaciones móviles como SendMany).

##### Testnet

Resulta conveniente aprender y hacer pruebas en ambiente de trabajo tipo "caja de arena". Raspiblitz permite esto mediante la opción "Testnet".
Tu ambiente de trabajo se renueva cada vez que cambias entre Testnet y Mainnet (blockchain, canales y wallets) lo que es conveniente y seguro.
Nota, sin embargo, que cambiando el ambiente de trabajo requiere volver a sincronizar la blockchain (tanto para Testnet como Mainnet) y puede tomar tiempo. Por decir algo, si activas pro primera vez Testnet, deber[as esperar a la sincronización completa de la blockchain Testnet; lo cual podría tomar varias horas. También, si vuelves a Mainnet, deberás ponerte al corriente con la última actualización de la blockchain.

Desde luego, sería menos arriesgado y más divertido si se pudiera contar con dos nodos; uno para pruebas y otro para producción. Así puedes mantener uno "oficial" corriendo y hacer pruebas alocadas con el segundo. 

Una vez en el ambiente de trabajo "TESTNET" puedes adquirir Bitcoin de la Testnet (bitcoin de a mentiras) y empezar a jugar con las monedas!
Puedes obtener bitcoin para Testnet en alguno de los siguientes sitios:
* https://coinfaucet.eu/en/btc-testnet/
* https://testnet-faucet.mempool.co/
* https://kuttler.eu/en/bitcoin/btc/faucet/
* https://faucet.lightning.community/

Puedes aprender más sobre Testnet en el siguiente enlace: https://kuttler.eu/code/bitcoin-testnet-blockchain-size-in-2020/
Que te diviertas.

IMPORTANTE: Actualkente BTCPayServer no está soportado en la red Testnet (RPC connection error messages). Por lo menos, hasta que se resuelva el siguiente problema: [issue #1724](https://github.com/rootzoll/raspiblitz/issues/1724). Mientras tanto, puedes intentar con: [jugar con BTCPayServer en TESTNET](https://testnet.demo.btcpayserver.org)

##### Circuitbreaker (Cortafuegos para LND)

Not everybody is acting friendly in the Lightning network. Circuitbreaker is a background service you cann activate that acts similar to a firewall to protect your now better. For details see: https://github.com/lightningequipment/circuitbreaker/blob/master/README.md

##### LND Auto-Unlock

The RaspiBlitz will automatically unlock the LND wallet upon every start.

This feature is based on https://github.com/Stadicus/guides/blob/master/raspibolt/raspibolt_6A_auto-unlock.md

It can be activated under "Services" -> "Auto-unlock LND". We recommend that it be turned on, when DynamicDNS is used. If there is a public IP change on your router, LND restarts automatically, and without Auto-Unlock it will stay inactive/unreachable until you manually unlock it.

* [When using Auto-Unlock, how much security do I lose?](FAQ.md#when-using-auto-unlock-how-much-security-do-i-lose)

##### StaticChannelBackup on DropBox

See [below on this README](README.md#backup-for-on-chain---channel-funds) for your Backup options to secure your funds against loss. Storing the encrypted Static Channel Backup file to your Dropbox account is an easy and secure way to do this.

##### StaticChannelBackup on USB Drive

You can connect a small extra USB drive to your RaspiBlitz (choose a small one up to 32GB - don't use second HDD or SSD here, that would drain too much power from the RaspiBlitz). On that USB drive your latest StaticChannelBackup will be stored - just in case your HDD gets an error.

##### ZeroTier 

With ZeroTier you can add your RaspiBlitz to a software defined network - see for details: https://en.wikipedia.org/wiki/ZeroTier

#### SERVICES: Activate/Deactivate Services

The RaspiBlitz offers further Services, Apps and configuration (scroll down to see all options in the RaspiBlitz):

![MainMenu-Services](pictures/services.png)

Activate/Deactivate service selection with the space bar and then select 'OK' to trigger Install/Uninstall. You can find more details about those options below (top to bottom):

##### Electrum Rust Server

Enables a user to run his own Electrum server on the RaspiBlitz. The server indexes the entire Bitcoin blockchain saved locally on your HDD/SSD, and the resulting index enables fast queries for any given user wallet, allowing the user to keep real-time track of his balances and his transaction history using the [Electrum wallet](https://electrum.org).

Since Electrum Rust Server runs on the user's own machine, there is no need for the wallet to communicate with external Electrum servers, thus preserving the privacy of addresses and balances.

By contrast, if you use your Trezor Hardware Wallet with the trezor.io wallet, it will tell their third party server your public keys - connecting it with your IP. Now you can use your Trezor with the Electrum Wallet, just talking to your own Electrum Server, preserving your privacy.

Learn how you can use Electrum with your own Server over Tor:

<a href="https://www.youtube.com/watch?v=AiosKK_TA7w" target="_blank"><img src="pictures/video-electrs.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=AiosKK_TA7w

[More Details on Service](https://github.com/romanz/electrs)

After install, you will see a new `ELECTRS` option in the SSH main menu - it will give you all the information you need to start using it.

##### RTL Webinterface

The RTL Webinterface is an LND Control Dashboard you can run in your browser with a nice GUI - it offers much more control over your Lightning node than the RaspiBlitz SSH menus. It's recommended to give it a try.

![RTL](pictures/RTL-dashboard.png)

Get all the details on how to mannage your channels with RTL in this video:

<a href="https://www.youtube.com/watch?v=pESO_Pm0v10" target="_blank"><img src="pictures/video-rtl.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=pESO_Pm0v10

Read an Intro-Tutorial to RTL: https://medium.com/@suheb.khan/how-to-ride-the-lightning-447af999dcd2

Feedback is welcome by the RTL programmer: https://github.com/ShahanaFarooqui/RTL

After install, you will see a new `RTL` option in the SSH main menu - it will give you all the information you need to start using it.

##### ThunderHub

A Lightning Node Manager WebUI - similar to RTL. 

[Details on Service](https://www.thunderhub.io)

After install, you will see a new `THUB` option in the SSH main menu - it will give you all the information you need to start using it.

##### Lightning Terminal (LIT) with loop, pool & faraday

Lightning Terminal (LiT) is a browser-based interface for managing channel liquidity. It bundles the former single tools called loop, pool & faraday with an easy to use browser interface.

![LIT](pictures/lit.png)

[Details on Service](https://github.com/lightninglabs/lightning-terminal#lightning-terminal-lit)

After install, you will see a new `LIT` option in the SSH main menu - it will give you all the information you need to start using it.

##### BTCPayServer

[BTCPay Server](https://github.com/btcpayserver) is a self-hosted, open-source cryptocurrency payment processor. It's secure, private, censorship-resistant and free.

![BTCPAY](pictures/btcpay.png)

Find all details on how to use the BTCPay Server on your RaspiBlitz in this great tutorial: https://coincharge.io/en/raspiblitz-btcpay-server/

After install, you will see a new `BTCPAY` option in the SSH main menu - it will give you all the information you need to start using it.

##### LNbits

LNbits is a very simple server that sits on top of your Lightning Wallet.

![LNBITS](pictures/lnbits.png)

It can be used together with IP2Tor to provide:
- Lightning Paper Vouchers (Plugin: LNURLw)
- Merchant Onboarding (Plugin: TPOS)

<a href="https://www.youtube.com/watch?v=0Bt3tHULAnw" target="_blank"><img src="pictures/video-vouchers.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=0Bt3tHULAnw

You can also develop your own extensions on it.

[Details on Service](https://github.com/arcbtc/lnbits/blob/master/README.md)

After install, you will see a new `LNBITS` option in the SSH main menu - it will give you all the information you need to start using it.

##### BTC-RPC-Explorer

BTC-RPC-Explorer is a blockchain explorer website you can run on your own RaspiBlitz. See an example running on: https://btc-explorer.com

![EXPLORER](pictures/blockexplorer.png)

[Details on Service](https://github.com/janoside/btc-rpc-explorer)

After install, you will see a new `EXPLORE` option in the SSH main menu - it will give you all the information you need to start using it.

##### Cryptoadvance Specter

Bitcoin Core has a very powerful command line interface and a wonderful daemon. Using pre-signed bitcoin transactions (PSBT) and [Hardware Wallet Interface](https://github.com/bitcoin-core/HWI) (HWI), it can also work with hardware wallets. At the moment it is very Linux-focused. The same applies to multi-signature setups.

The goal of SpecterDesktop is to make a convenient and user-friendly GUI around Bitcoin Core, focusing on multi-signature setups with airgapped hardware wallets like Trezor, Ledger, COLDCARD or the Specter-DIY.

![SPECTER](pictures/specter.jpg)

After install, you will see a new `SPECTER` option in the SSH main menu - it will give you all the information you need to start using it.

As an alternative to runninf Specter on directly on the RaspiBlitz, there is a Specter Desktop version that runs on your laptop. Here is a [guide to connect the specter laptop app] (https://d11n.net/connect-specter-desktor-with-raspiblitz.html) to your RaspiBlitz Bitcoin fullnode.

##### Mempool Explorer

![MEMPOOL](pictures/mempool.png)

Mempool is the fully featured visualizer, explorer, and API service running on mempool.space

[Details on Service](https://github.com/mempool/mempool)

After install, you will see a new `MEMPOOL` option in the SSH main menu - it will give you all the information you need to start using it.

##### JoinMarket

JoinMarket is software to create a special kind of bitcoin transaction called a CoinJoin transaction. Its aim is to improve the confidentiality and privacy of bitcoin transactions.

<a href="https://www.youtube.com/watch?v=uGHRjilMhwY" target="_blank"><img src="pictures/video-joinmarket.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=uGHRjilMhwY

A CoinJoin transaction requires other people to take part. The right resources (coins) have to be in the right place, at the right time, in the right quantity. This isn't a software or tech problem, it's an economic problem. JoinMarket works by creating a new kind of market that would allocate these resources in the best way.

For more details see [here](https://github.com/JoinMarket-Org/joinmarket-clientserver).

After install, you will see a new `JMARKET` option in the SSH main menu - it will give you all the information you need to start using it.

##### Balance of Satoshi

Balance of Satoshi gives you enhanced commands for working with LND balances.

[Details on Service](https://github.com/alexbosworth/balanceofsatoshis/blob/master/README.md)

After install, you will see a new `BOS` option in the SSH main menu - it will give you all the information you need to start using it.

##### Sphinx Relay Server

The Sphinx App allows chat over the Lightning Network and ties into the idea of [Podcasting 2.0](https://u.today/father-of-podcasting-integrates-bitcoin-lightning-into-his-app). To use the mobile app with your own RaspiBlitz you need to install the [Sphinx Relay Server](https://github.com/stakwork/sphinx-relay/blob/master/README.md).

![SPHINX](https://github.com/stakwork/sphinx-relay/raw/master/public/relay.jpg)

After install, you will see a new `SPHINX` option in the SSH main menu - it will give you all the information you need to start using it.

##### PyBlock

![PYBLOCK](pictures/pyblock.png)

https://github.com/curly60e/pyblock/blob/master/README.md

##### Channel Tools (chantools)

This tool provides helper functions that can be used to rescue funds locked in lnd channels in case lnd itself cannot run properly anymore.

https://github.com/curly60e/pyblock/blob/master/README.md

##### Download Bitcoin Whitepaper

Extract the original Bitcoin Whitepaper as PDF directly from the blockchain of your node.

#### SYSTEM: Monitoring & Configuration

![SYSTEM](pictures/system.png)

#### CONNECT: Connect Apps & Credentials

This feature should support connecting your RaspiBlitz to a mobile wallets or other apps.

![CONNECT](pictures/connect.png)

##### MOBILE: Mobile Wallet Apps (Smartphone)

At the moment, the following mobile wallets are supported:

* [Zeus (iOS/Android)](https://github.com/ZeusLN/zeus)
* [Fully Noded (iOS over Tor)](https://apps.apple.com/us/app/fully-noded/id1436425586)
* [SendMany (Android)](https://github.com/fusion44/sendmany/blob/master/README.md)
* [Sphinx Chat App (iOS/Android)](https://sphinx.chat/)

Mobile wallets work as a remote control app for your RaspiBlitz. First you need to install the apps on your phone - a QR code with the links to the app stores are displayed. Then you need to `pair` them with your RaspiBlitz - also via a QR code displayed on the LCD. If you run your RaspiBlitz without an LCD, there is the fallback option to display that QR code on the terminal as ASCII code (which might involve lowering your terminal's font size).

##### BTCPAY: Get the connection string for the BTCPay Server

To connect the payment processing BTCPay server to your Lightning node you find here the needed Connection string.

##### bitcoinRPC

If apps need access to the Bitcoin RPC service you can find this here.

##### BISQ: Use your node with BISQ

Here you can activate a hidden service for your bitcoin node so that it can be used for the decentral exchange called BISQ.

##### EXPORT: Macaroons and TLS.cert

If you want to access your LND APIs (to connect apps and additional services) you need credential files that grant access (Macaroons & the TLS cert).

*Macaroons: Access Tokens that allow certain command executions on the LND node.*
*TLS: Certificate to secure/encrypt communication with the LND node.*

In this menu, you can reset, re-sync, or export them as a file or string so that you can import them to apps and additional services.

Here are the following export options to get the Macaroon and TLS files to be used in other apps and wallets:

###### SSH Download

SCP is a SSH like command to transfer files. If we're able to SSH into the RaspiBlitz, also the SCP to transfer the files should work. If you choose this option, RaspiBlitz will print prepared SCP commands you can copy+paste to run in a second terminal.

This method is recommended to export to:
* [Zap Desktop Wallet](https://github.com/LN-Zap/zap-desktop)

###### Browser download

Opens an ad-hoc webserver so that you can download the files in your local network through the browser.

*This is the least secure way to transfer those files - everybody in your local network has access to those file during download. Remember with the Admin-Macaroon somebody could takeover your node and spend all your funds. Just use as last fallback.*

###### Hex-String

The Macaroons and TLS.cert files can be copy+pasted as Hex-Strings from RaspiBlitz to any other app that supports that format. If you choose this option, RaspiBlitz will print all the files for you as Hex-String to do so.

This method is recommended to export to:
* [Joule Browser Wallet](https://lightningjoule.com)

#### SUBSCRIBE: Subscription Services

The RaspiBlitz offers now also Subscriptions .. those are free or paid third-party services.

![MainMenu-Services](pictures/subscriptions.png)

Under `LIST my Subscriptions` you will always find the list of all your active subscriptions, to get more details or to `CANCEL` them.

At the moment, the following subscription services are available:

##### IP2TOR (paid)

IP2TOR is a tunnel service where you can run your RaspiBlitz anonymously behind TOR but you rent a port on a clearnet IP thru which you can make services of your RaspiBlitz easy reachable for everybody on the internet. You don't need to care about your local router or firewall settings. You can pay this service also directly thru Lightning from your RaspiBlitz as subscription.

At first you select what service of your RaspiBlitz you like to tunnel thru a IP2TOR bridge. 

You will get a list of available IP2TOR bridge offerings. Select `OK` on an IP2TOR bridge offering and you will see more details on it, such as how many satoshis the subscription will cost you - your node should be funded and have channels open at this point.

Then you get a list of available IP2TOR bridge offerings. By selecting `OK` on a IP2TOR bridge offering you can get more details on it and you will also see how many satoshis the subscription will cost you - your node should be funded and you should have channels open at this point.

If you choose `AGREE` on the details of a IP2TOR bridge offering the RaspiBlitz tries for you to setup the IP2TOR bridge. If everything worked you will find now the subscription under `MAINMENU` > `SUBSCRIBE` > `LIST My Subscriptions` where you can cancel it again.

To try out the IP2TOR tunnel choose in `MAINMENU` the extra menu point of the Service you choose the bridge for and it should give you now an updated URL or try calling the API on the IP and Port that is displayed under the details of the subscription in the `LIST My Subscriptions` section.

##### HTTPS with LetsEncrypt (free)

If you want a Webservice like BTCPay Server or LNbits available to the outside internet (like with IP2TOR) people expect you to offer HTTPS address so that the communication between the client and your RaspiBlitz is encrypted. You could use the self-signed HTTPS certificate that RaspiBlitzis offering you, but this will give users Security Warnings in their browser and is not very user friendly. That's where you can use a LetsEncrypt Subscription to get a free valid HTTPS certificate that is excepted without warning from almost all common browsers. 

Because you also need a domain name for that you will need to open a free account on [DuckDNS.org](https://www.duckdns.org) ... further options might be added in the future.

When you create a new LetsEncrypt subscription, you will be asked for your subdomain on DuckDNS and the Auth-Token of your DuckDNS account. Then RaspiBlitz tries to setup everything for you. If everything worked, you will find the subscription under `MAINMENU` > `SUBSCRIBE` > `LIST My Subscriptions`, where you can cancel it at any time if you wish.

To try out the IP2TOR tunnel, go into `MAINMENU` and the extra menu point of the Service you want to use the bridge for. It should give you an updated URL to call your service.

#### PASSWORD: Change Passwords

Change your passwords for security.

#### REPAIR: Options to test, repair and reset your RaspiBlitz

The `REPAIR` menu gives you options to check and reset your RaspiBlitz.

![RepairMenu](pictures/repairmenu.png)

The options are explained in detail below:

##### SOFTWARE: Run Software Tests (DebugReport)

This will print out a lot of information that can be used to find software problems.

Use this if you want to report a software problem with your RaspiBlitz, so that others can have a look and help you better.

##### BACKUP-LND: Backup your LND data (Rescue-File)

This stops your RaspiBlitz and creates an LND-Rescue ZIP file that you can download via SCP to your laptop. This can be used to move your LND id, wallet & channels to another RaspiBlitz.

*NOTICE: If you start your RaspiBlitz after this backup again the backup is outdated and using it can risk losing your channel funds.*

##### MIGRATION: Migrate Blitz Data to new Hardware

This stops your RaspiBlitz and creates a Migration ZIP file you can download/export per SCP to your laptop. This contains all important data of your RaspiBlitz including LND, your Blitz configuration and also data from your installed apps. Can be used to migrate your RaspiBlitz to a new hardware - for example if you want to replace the HDD with a SSD. How to import a Migration File [see here](README.md#import-a-migration-file).

*NOTICE: If you start your RaspiBlitz after exporting the migration file again it is outdated and using it can risk losing your channel funds.*

##### COPY-SOURCE: Offer your Blockchain to another RaspiBlitz for Setup

To expedite the setup process, you can connect another RaspiBlitz and copy over your blockchain data to it. Your RaspiBlitz will be `offline` during that process and it can take between 4 to 6 hours.

Make sure both RaspiBlitzes are connected to the same local network. During setup with the new RaspiBlitz, choose the `COPY` option to get the blockchain data and then select the source computer `RASPIBLITZ`. Now you can activate the `COPY-SOURCE` option, enter the given IP of the new RaspiBlitz and its Password A (not yours) .. then the process should start.

##### RESET-CHAIN: Delete Blockchain and Re-Download

Use this option if your blockchain data got corrupted. It will keep your LND data. You can even keep your channels open. Just keep in mind that your Lightning node will appear offline to the network until you have re-downloaded the blockchain.

##### RESET-LND: Delete LND data & start new node/wallet

*THIS WILL DELETE ALL YOUR LND DATA AND CHANNEL FUNDS.
Use this only if you have closed all channels and removed all funds.*

Use this option if you want to start with a fresh LND node id & wallet.

##### RESET-HDD: Delete HDD data but keep blockchain

*THIS WILL DELETE ALL YOUR LND DATA AND CHANNEL FUNDS.
Use this only if you have closed all channels and removed all funds.*

Use this if you want to setup a fresh RaspiBlitz but don't want to re-download the blockchain.

##### RESET-ALL: Delete HDD completely & start fresh

*THIS WILL DELETE ALL YOUR LND DATA AND CHANNEL FUNDS.
Use this only if you have closed all channels and removed all funds.*

Use this if you want to setup a fresh RaspiBlitz with an empty HDD.

##### DELETE-ELEC: Delete Electrum Index

If you had Electrum installed, you can use this option to make sure also the space consuming electrum index gets deleted to free up space.

##### DELETE-INDEX: Delete Bitcoin TX-Index

If you had the Bitcoin Transaction Index activated you can use this option to make sure that this extra space consuming index gets deleted as well to free up space.

#### UPDATE: Check/Prepare RaspiBlitz Update

The `UPDATE` menu gives you options to update your RaspiBlitz

![UpdateMenu](pictures/update.png)

The options are explained in detail:

*Please note that the RaspiBlitz does not support Auto-Update, to ensure that there is no remote control of your node from a central server.*

##### RELEASE: Update RaspiBlitz to a new Version

This is common way to update your RaspiBlitz. Choose this option to prepare your RaspiBlitz for a new SD card image containing the new version release.

##### PATCH: Patch RaspiBlitz code

With Patching you have now an easy way to sync your RaspiBlitz code/scripts with the official RaspiBlitz GitHub Repo or even your own forked GitHub Repo. This is an option for people that report bugs and we like to offer them a quick script update (patch) between RaspiBlitz releases or for people who want to develolp on the RaspiBlitz and sync code between their IDE, forked GitHub and their RaspiBlitz.

##### LND: Interim LND Update

Sometimes there is a new LND release that has some breaking changes that once you updated the LND database cannot be reversed (like the update from 0.9.2 to 0.10.0). Then RaspiBlitz offers you an optional update ... this is where you then can update LND.

If you choose this you get the option to do this `VERIFIED` that means it offers you the optional LND update we tested the RaspiBlitz with or `RECKLESS` which will just grab the latest LND release from the GitHub releases page (also Release Candidates) and install it with no further guarantees and verification checks - this is for people that run nodes to test new releases and how they work with existing RaspiBlitz apps.

##### BITCOIN: Interim Bitcoin Update

Like with LND you have the possiblity to upadte the bitcoin core version here.

#### REBOOT: Reboot RaspiBlitz

A safe way to restart the RaspiBlitz ... have you tried turning it off and on again?

#### OFF: PowerOff RaspiBlitz

A safe way to shutdown the RaspiBlitz.

#### X: Console Terminal

Closes the SSH main menu and exits to the terminal - where the user can make use of the CLI clients `bitcoin-cli` & `lncli` directly.

With the command `raspiblitz`, it's possible to return to the main menu.

## Import a Migration File

As mentioned above you can export a Migration File from your RaspiBlitz with MAINMENU > REPAIR > MIGRATION and store it on your laptop.

A Migration file contains all the important data from your RaspiBlitz, like your LND data, Bitcoin Wallet, raspiblitz.config, Tor/SSH keys .. and also installed apps. You can use this to migrate your RaspiBlitz to new hardware.

If you want to import it again to a new RaspiBlitz (for example with an updated HDD/SSD), you can choose the `MIGRATION` option on the first setup dialog after the Hardware test (where you normally choose between Bitcoin & Litecoin).

![SSH0](pictures/ssh0-welcome2.png)

If you start MIGRATION you will need to format your HDD/SSD in the next step.

![MIGRATION1](pictures/migration1.png)

Normally you choose here the EXT4 format. But you also have the option to choose the BTRFS format which is an experimental feature under RaspiBlitz - see [FAQ for details on BTRFS](FAQ.md#why-use-btrfs-on-raspiblitz).

Then you will be asked to upload the Migration Zip file to the RaspiBlitz. Follow the instructions shown to you.

Then you need to get a copy of the blockchain data again for your RaspiBlitz.

![MIGRATION2](pictures/migration2.png)

You have the two options: [SYNC](README.md#1-sync---selfvalidate-all-blocks) and [COPY](README.md#2-copy---copy-from-laptop-or-another-raspiblitz-over-local-network), as mentioned in the normal setup.

RaspiBlitz will reboot and start the normal recovery process to install all the services defined by the raspiblitz.config from your Migration File.

Then the blockchain needs to sync up and you should be back to normal.

## Make a RaspiBlitz out of your Umbrel or MyNode

Another kind of migration is when you already run an full node with the Umbrel or myNode software and you like to change it to RaspiBlitz without closing channels. You basically have all the hardware needed and just need to change software. You dont need the [LCD from the shopping list](#amazon-shopping-list-buy-parts--build-it-yourself) - RaspiBlitz can also run without an LCD.

*NOTE: This migration is still experimental. You will still use the terminal to setup & manage your RaspiBlitz. If that is too technical for you please wait for the RaspiBlitz v1.8, which will introduce a WebUI for your browser that make the migration to RaspiBlitz familiar like with your old node user experiences.*

Before you start migration:
* if you have on-chain funds on your old node - make sure to have the backup seed words
* if you have lightning channels open on your old node - make sure to have downloaded the latest Static Channel Backup file to your laptop

Also be aware that at the moment RaspiBlitz can only transfer your blockchain and LND wallet data (including channels) over to RaspiBlitz. Any data/pairing of additional apps cannot be transfered and may get lost.

Instructions for Migration:
* shutdown your old node
* remove the sd card
* [download the latest Raspiblitz sd card image & flash it to your sd card](#downloading-the-software)
* if you like to use a HDMI monitor for status & progress, create a empty file called `hdmi` (withot any ending) on the sd card while connected to your laptop 
* [insert sd card, boot up & login per SSH](#boot-your-raspiblitz)

Now RaspiBlitz should show you that old data from your node was detected and offer you todo the migration.

* If you continue it will prepare the data & reboot.
* The RaspiBlitz recover/update modus is starting - that will take a while and finally reboot.
* Login per SSH as before and reset the passwords (`FINAL RECOVERY LOGIN` on LCD). Then a final reboot will happen.
* Login per SSH with your new password A & unlock LND wallet with password C. Now blockchain needs to catch up and then your RaspiBlitz should be ready and show you (under INFO) your on-chain & channel balance.

If you dont have an LCD or HDMI monitor connected it might be a bit difficult to see what state your RaspiBlitz is in. Just (re-)try to login per SSH again after the reboots (might always take some time until it reacts). 

## Interface / APIs

To develop your own scripts/apps and connect other services/apps to your RaspiBlitz, you have multiple interfaces/APIs available:

### Bitcoin

* `bitcoin-cli` command line interface on the terminal
* `bitcoind` running on port 8333 (public)
* `JSON-RPC` running on port 8332 (local) [DOC](https://en.bitcoin.it/wiki/API_reference_%28JSON-RPC%29)

### LND-Lightning

* `lncli` command line interface on the terminal [DOC](https://api.lightning.community/)
* `lnd` running on port 9735 (public)
* `gRPC` running on port 10009 (public) [DOC](https://api.lightning.community/)
* `REST` running on port 8080 (public) [DOC](https://api.lightning.community/rest/index.html)

If you activate Tor, then your LND gRPC & REST APIs will also be reachable publicly as a Hidden Service.

### Backup for On-Chain- & Channel-Funds

Since LND v0.6 (and RaspiBlitz v1.2), a feature called Static-Channel-Backups is available. Within RaspiBlitz this is used when a `channel.backup` file is mentioned.

At this point in time, it is the best way to backup and protect your channel funds on RaspiBlitz - so it's recommended to make use of it.

To recover your funds this way, you will need two things:
- the 24-word seed
- the latest `channel.backup` file

You should have written down the word seed during wallet setup; keep it at a safe (offline) location. The `channel.backup` is stored on the HDD and updated by LND every time a new channel is opened or closed. The latest version of this file is needed to recover all your funds. In case your HDD gets damaged, RaspiBlitz always keeps a copy of the latest version of the `channel.backup` file on the SD card within the sub-directories of: `/home/admin/.lnd/data/chain/`.

If you want to get one step further in securing your funds against total fall-out of the RaspiBlitz (gets completely damaged, stolen or lost) then you can additionally set up an off-location or cloud backup of the `channel.backup` file. The file itself is encrypted by your word seed - so it's OK to store the file to untrusted third parties for backup (if you want). 

This video explains in detail how you can set further back Static Channel information:

<a href="https://www.youtube.com/watch?v=5wi6l9jRVQs" target="_blank"><img src="pictures/video-backup.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=5wi6l9jRVQs

The following options are also explained here shortly:

#### A) DropBox Backup Target

Activate the StaticChannelBackup to DropBox in the `SETTINGS` menu of your RaspiBlitz. It will ask you for the Dropbox-Authtoken. This is how you can get this token:

Go to your web browser, do the following:

1. Go to https://www.dropbox.com/developers/apps/create and sign in.

1. Choose **Create App**.

    ![Dropbox API 1](https://github.com/rootzoll/raspiblitz/raw/v1.6/pictures/dropbox-1.png)

    Choose the 'Scoped Access' & 'App Folder' and set a unique name - for example `LNDbackup` with a random number behind it. Agree to Terms of Service and click 'Create App'.

1. Set **Permissions**.

    ![Dropbox API 2](https://github.com/rootzoll/raspiblitz/raw/v1.6/pictures/dropbox-2.png)

    Its important first to select the `Permissions` tab and activate the `files.content.write` permission. Dont forget to `Submit` the change before continue.

1. Generate **OAUth2 Token**.

    ![Dropbox API 3](https://github.com/rootzoll/raspiblitz/raw/v1.6/pictures/dropbox-3.png)

    Now go back to the 'Settings' tab and under 'OAuth2' click the 'Generate' button. You will now see a long string of letters and numbers appear. This is your **Dropbox-Authtoken**. Make sure to copy the complete token string .. there might be more if you scroll to the right in the token field. 

To test it, try opening or closing a channel, and then check if you can find a copy of `channel.backup` in your Dropbox. You can check the background-script logs to see details on errors: `sudo journalctl -f -u background`

#### B) SCP Backup Target

*You can also backup the SCB to your own server, but this needs manual setup:*

In the `/mnt/hdd/raspiblitz.conf` the parameter `scpBackupTarget='[USER]@[SERVER]:[DIRPATH-WITHOUT-ENDING-/]'` can be set to activate this feature. On that remote server the public key of the RaspiBlitz root user needs to be part of the authorized keys - so that no password is needed for the background script to make the backup.

The script `/home/admin/config.scripts/internet.sshpubkey.sh` helps on initalization (init); it will show and transfer ssh-pubkey to a remote server.

To test it, try opening or closing a channel, and then check if you can find a copy of `channel.backup` on your remote server. You can check the background-script logs to see details on errors: `sudo journalctl -f -u background`

#### C) Local Backup Target (USB Thumbdrive)

*You can also backup the SCB to another local drive, e.g. a USB stick:*

You can use a small USB thumb drive (everything over 120MB is fine). Please don't use a second HDD/SSD for this because that might drain too much power and could hurt the security of your data more then it helps.

To activate this feature, go to `MAINMENU` > `SETTINGS` > `StaticChannelBackup on USB Drive` and follow the instructions.

To test it, try opening or closing a channel, and then check if you can find a copy of `channel.backup` in the specified location. You can check the background-script logs to see details on errors: `sudo journalctl -f -u background`

## Updating RaspiBlitz to new Version

If you have a RaspiBlitz older than version v1.0, please [see here](FAQ.md).

If you have a RaspiBlitz v1.2 or higher - just follow the `UPDATE` option from the main menu (choose `RELEASE` if asked) and follow the instructions - see the process in detail in the following video.

<a href="https://www.youtube.com/watch?v=Xvn0WQfHUdI" target="_blank"><img src="pictures/video-update.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=Xvn0WQfHUdI

If you have a RaspiBlitz v1.0 or v1.1 or higher do the following:

* Main menu > OFF
* Remove power
* Remove SD card

Now download the new RaspiBlitz SD card image and write it to your SD card. Yes, you simply overwrite the old one, it's OK! The RaspiBlitz stores all your personal data on the HDD. See details about latest SD card image [here](#installing-the-software).

*If you have done manual changes to the system (installed packages, added scripts, etc), you might need to do some preparations before overwriting your SD card - see [FAQ](FAQ.md#why-do-i-need-to-re-burn-my-sd-card-for-an-update).*

If done successfully, simply put the SD card into the RaspiBlitz and power on again. Then follow the instructions on the display ... and don't worry, you don't need to re-download the blockchain again. It is worth noting here that your SSH password will be reset to `raspiblitz`. You will be promted to change this once the update is finished.

* [Why do I need to re-burn my SD card for an update?](FAQ.md#why-do-i-need-to-re-burn-my-sd-card-for-an-update)

## Build the SD Card Image

A ready-to-use SD card image of RaspiBlitz is provided by us for download, to get everybody started quickly (see above). But if you want to build that image yourself - here is a quick guide:

* Get a latest RaspiOS 64-bit: [DOWNLOAD](https://downloads.raspberrypi.org/raspios_arm64/images).
* Write the image to an SD card: [TUTORIAL](https://www.raspberrypi.org/documentation/installation/installing-images/README.md).
* Add a file called `ssh` to the root of the SD card when mounted on your laptop to enable SSH login.
* Start the card on a Raspi and login via SSH with `ssh pi@[IP-OF-YOUR-RASPI]`. Password is `raspberry`.

Now you are ready to start the SD card build script (check the code to see if the installation and config are OK for you). Copy the following command into your terminal and execute:

`wget https://raw.githubusercontent.com/rootzoll/raspiblitz/v1.7/build_sdcard.sh && sudo bash build_sdcard.sh`

As you can see from the URL, you can find the build script in this Git repo under `build_sdcard.sh`. You can check what gets installed and configured in detail. Feel free to post improvements as pull requests.

The whole build process takes a while. At the end the LCD drivers get installed and a reboot is needed. A user `admin` is created during the process. Remember the default password is now `raspiblitz`. You can login per SSH again - this time use admin: `ssh admin@[IP-OF-YOUR-RASPI]`. The install dialog of the RaspiBlitz schould automatically start. If you do not want to continue with the installation at this moment and use this sd card as a template for setting up multiple RaspiBlitzes, click `Cancel` and run `/home/admin/XXprepareRelease.sh`. Once you see the LCD going white and the activity LED of the pi starts going dark, you can unplug power and remove the SD card. You have now built your own RaspiBlitz SD card image.

*Note: If you plan to use your self-build sd card as a MASTER copy and distribute it: Use a smaller 8GB card for that. This way it's ensured that it will fit on every 16 GB card recommended for RaspiBlitz later on.*

* [Can I run RaspiBlitz on other computers than RaspberryPi?](FAQ.md#can-i-run-raspiblitz-on-other-computers-than-raspberrypi)
* [How can I build an SD card other than the master branch?](FAQ.md#how-can-i-build-an-sd-card-other-then-the-master-branch)
* [How can I build an SD card from my forked GitHub Repo?](FAQ.md#how-can-i-build-an-sd-card-from-my-forked-github-repo)

## FAQ

Here is a short selection of the very frequently asked questions:

* [How to backup my Lightning Node?](FAQ.md#how-to-backup-my-lightning-node)
* [How can I recover my coins from a failing RaspiBlitz?](FAQ.md#how-can-i-recover-my-coins-from-a-failing-raspiblitz)
* [Are those "Under-Voltage detected" warnings a problem?](FAQ.md#are-those-under-voltage-detected-warnings-a-problem)
* [Can I run RaspiBlitz on computer boards other than RaspberryPi?](FAQ.md#can-i-run-raspiblitz-on-other-computers-than-raspberrypi)

Do you still have more questions? Check the [RaspiBlitz-FAQ-Archive](FAQ.md).

## Community Development

Everybody is welcome to join, improve, and extend the RaspiBlitz - it's a work in progress. [Check the issues](https://github.com/rootzoll/raspiblitz/issues) if you wanna help out or add new ideas. You find the scripts used for RaspiBlitz interactions on the device at `/home/admin` or in this Git repo's subfolder `home.admin`.

To start your Deep Dive into the RaspiBlitz project, the following YouTube video (July 2020) is recommended: [https://www.youtube.com/watch?v=QXUGg45CWLo](https://www.youtube.com/watch?v=QXUGg45CWLo)

Get all details on "How to contribute to RaspiBlitz Development" on this video:

<a href="https://www.youtube.com/watch?v=ZVtZepV3OfM" target="_blank"><img src="pictures/video-contrib.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=ZVtZepV3OfM

Also get inspired for a deep-dive with the original "[RaspiBolt](https://stadicus.github.io/RaspiBolt/)" tutorial on how to build a lightning node on the RaspberryPi, the base work on which the RaspiBlitz was developed - so much thx to Stadicus :)

Join me on twitter [@rootzoll](https://twitter.com/rootzoll), visit us at an upcoming [#lightninghackday](https://twitter.com/hashtag/LightningHackday?src=hash) or check by one of our bitcoin meetups in Berlin ... every 1st Thursday evening a month at the room77 bar - feel free to buy me a beer with lightning there :)

* [How can I get further help/support?](#support)
