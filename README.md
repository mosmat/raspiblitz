![RaspiBlitz](pictures/raspilogo_tile_400px.png)

*Construye tu propio nodo para Bitcoin y red Lightning.*

`Versión 1.7.0 con lnd 0.12.1 y bitcoin 0.21.0 (o litecoin 0.18.1)`

![RaspiBlitz](pictures/raspiblitz.jpg)

**El Raspiblitz es un nodo para Bitcoin y Lightning del tipo hágalo-usted-mismo. Funciona corriendo LND al mismo tiempo que un Nodo-Completo de Bitcoin usando un RaspberryPi (con 1TB SSD de almacenamiento) y una cómoda pantalla para fácil instalación y monitoreo.**

Raspiblitz está orientado principalmente a aprender a correr un nodo descentralizado desde casa -porque, como dice el dicho: "si no es tu nodo, entonces no son tus reglas"-. Descubre y contribuye al desarrollo del ecosistema de la Red Lightning formando parte de ella. Puedes llevarlo a cabo mediante un [taller](WORKSHOP.md) o como un proyecto personal para el fin de semana.

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

El Raspiblitz está optimizado para ser montado durante la duración de una conferencia o un taller-repentina (Mira los detalles en [tutorial para talleres](WORKSHOP.md)). Si se trata de montar una copia de la cadena de bloques actualizada, es posible tener un nodo listo en 2 a 3 horas; la mayor parte de la duración de la instalación se trata de tener paciencia.

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

[Qué otras opciones de carcasas existen?](FAQ.md#what-other-case-options-do-i-have)

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

|Método|Instalación de imágen de archivo|Recopilar la microtarjeta SD|
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

Al principio puedes elegir el tipo de instalación para tu Raspiblitz. Puede correr Bitcoin o Litecoin en la Red Lightning. Esto también aplica si estás importando el archivo de migración desde un Raspiblitz desactualizado. Lee más sobre la migración [más abajo](README.md#import-a-migration-file). La opción por defecto es Bitcoin. 

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

LND generará una Frase Semilla nueva (lista de palabras) para ti.

![SSH8](pictures/ssh8-walletb.png)

ESCRIBE TU LISTA DE PALABRAS antes de que continúes. Sin ellas, disminuyes las posibilidades de recuperar tus fondos en caso de fallas de hardware u otras razones. Si solo se trata de probar y experimentar con el Raspiblitz, por lo menos toma una foto con tu smartphone, por si acaso. Si piensas mantener tu nodo corriendo, guarda la lista de palabras FUERA DE LÍNEA (esto significa, no fotos, no copia de word, no copia en dropbox, google drive, mensaje de whatsapp, y por el estilo) y en un lugar seguro. Puedes utilizar el [RaspiBlitz Password Sheet (PDF)](https://github.com/rootzoll/raspiblitz/raw/v1.4/home.admin/assets/RaspiBlitzRecoverySheet.pdf) para esto.

#### Recupera una billetera VIEJA

Escoge esta opción si ya cuentas con un viejo Raspiblitz o nodo que desees recuperar. Tienes tres opciones:

![SSH7](pictures/ssh7-lndrecover.png)

El Raspiblitz ejecutando el comando de creación de billetera LND:

##### LNDRESCUE LND tar.gz-Backupfile (MEJOR OPCIÓN) 

Escoge esta opción si cuentas con una copia de respaldo de la información LND en un archivo del tipo tar.gz llamado 'lnd-rescue'. Recuperará tus fondos on-chain y abrirá los canales que ya tenías disponibles. Tienes que asegurarte de que realmente sea la más reciente copia de la inormación LND; de otro modo, podrías perder la liquidez de los canales.

*Si tienes un archivo tar.gz que comienza con 'raspiblitz', ese es el archivo de migración. Ese archivo también incluye tu vieja billetera LND que has importado poco antes durante el proceso... mira detalles más abajo.*

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

Resulta conveniente aprender y hacer pruebas en un ambiente de trabajo tipo "caja de arena". Raspiblitz permite esto mediante la opción "Testnet".
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

IMPORTANTE: Actualmente BTCPayServer no está soportado en la red Testnet (RPC connection error messages). Por lo menos, hasta que se resuelva el siguiente problema: [issue #1724](https://github.com/rootzoll/raspiblitz/issues/1724). Mientras tanto, puedes intentar con: [jugar con BTCPayServer en TESTNET](https://testnet.demo.btcpayserver.org)

##### Circuitbreaker (Cortafuegos para LND)

No todos pueden ser amistosos en la red Lightning. Circuitbreaker es un servicio de cortafuegos que actúe similar al de una computadora para proteger mejor tu equipo. Para detalles mira: https://github.com/lightningequipment/circuitbreaker/blob/master/README.md

##### LND Auto-Unlock

Desbloqueo automático del servicio LND del Raspiblitz.

Esta opción está basada en: https://github.com/Stadicus/guides/blob/master/raspibolt/raspibolt_6A_auto-unlock.md

Se puede activar en `SERVICIOS` -> `Auto-unlock LND`. Recomendamos que lo mantengas encendido si utilizas DynamicDNS. Cada que cambia el IP público de tu nodo, LND se reinicia automaticamente; sin el Auto-Unlock, el nodo se mantendría desactivado o fuera de alcance hasta que lo desbloquees manualmente.

* [¿Qué tan riesgoso es mantener Auto-Unlock encendido?](FAQ.md#when-using-auto-unlock-how-much-security-do-i-lose)

##### StaticChannelBackup en DropBox

Mira [más abajo](README.md#backup-for-on-chain---channel-funds) para saber las opciones de respaldo que tienes para proteger tus fondos. Puedes guardar un archivo encriptado de respaldo (Channel Backup) en tu Dropbox. 

##### StaticChannelBackup en una USB Drive

Puedes conectar una USB extra a tu Raspiblitz. (una pequeña de 32GB, puede funcionar; no es necesario conectar un segundo disco duro, eso estaría sobrecargando tu Raspiblitz) En esa memoria USB se guardará tu último archivo 'StaticChannelBackup'; para el caso en el que tu disco duro tenga algún error.

##### ZeroTier 

Con ZeroTier puedes agregar tu Raspiblitz a una red definida de aplicación. Para más detalles: https://es.wikipedia.org/wiki/ZeroTier

#### SERVICES: Activar y desactivar servicios

El Raspiblitz ofrece servicios extra, aplicaciones y configuraciones. Mira más abajo todas las opciones:

![Menú Principal](pictures/services.png)

Activa o desactiva servicios seleccionando la casilla con la barra espaciadora, después selecciona `OK` para instalar y/o desinstalar.

##### Electrum Rust Server

Permite correr en tu Raspiblitz un Servidor Rust para Electrum. El servidor indexa la blockchain completa en el disco duro; de modo que es más rápido dar con la información relacionada con determinada wallet, permitiendo al usuario mantener de forma privada y en tiempo real el detalle de sus balances e historial de transacciones. [Electrum wallet](https://electrum.org).

Esto es distinto a utilizar Electrum con la configuración por default; la diferencia es que no utilizas el servidor de ellos y en lugar utilizas el tuyo que se encuentra corriendo en tu Raspiblitz. Esto ayuda a mantener la privacidad y seguridad de tus cuentas. 

Imagina que utilizas tu hardware wallet Trezor con la aplicación y servidores de trezor.io. Esto confiaría la información que relaciona la dirección de tu bitcoin con la dirección IP de tu nodo. Utilizando el servidor Electrum Rust Server la comunicación es directa y privada entre tu nodo y tu Trezor.

Para aprender cómo utilizar el servidor como servicio Tor:

<a href="https://www.youtube.com/watch?v=AiosKK_TA7w" target="_blank"><img src="pictures/video-electrs.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=AiosKK_TA7w

[Más detalles del servicio (en inglés)](https://github.com/romanz/electrs)

Después de la instalación verás `ELECTRS` como opción en el menú principal por SSH; al seleccionarlo te dará la información necesaria para comenzar a usar Electrs enseguida.

##### RTL Webinterface

La interfaz RTL Webinterface es un puesto de mando al que accedes desde tu navegador; ofrece mucho más control sobre tu nodo que los menús principales de Raspiblitz. Se recomienda probarlo, vale la pena.

![RTL](pictures/RTL-dashboard.png)

Mira todos los detalles de RTL (en Inglés):

<a href="https://www.youtube.com/watch?v=pESO_Pm0v10" target="_blank"><img src="pictures/video-rtl.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=pESO_Pm0v10

Lectura tutorial sobre RTL: https://medium.com/@suheb.khan/how-to-ride-the-lightning-447af999dcd2

Para ofrecer comentarios sobre el desarrollo de RTL: https://github.com/ShahanaFarooqui/RTL

##### ThunderHub

Una interfaz web para controlar tu nodo; similar a RTL.

[Detalles del servicio (en Inglés)](https://www.thunderhub.io)

Después de la instalación, verás `THUB` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### Lightning Terminal (LIT) para utilizar loop, pool y faraday

Lightning Terminal (LiT) es una interfaz web para manejar la liquidez de tus canales. Hace paquete con las herramientas loop, pool y faraday.

![LIT](pictures/lit.png)

[Detalles del servicio (en Inglés)](https://github.com/lightninglabs/lightning-terminal#lightning-terminal-lit)

Después de la instalación, verás `LiT` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### BTCPayServer

[BTCPay Server (Inglés)](https://github.com/btcpayserver) es un procesador de pagos personal, open source y alojado en tu nodo. Útil para E-comercio y recibir pagos.

![BTCPAY](pictures/btcpay.png)

Mira los detalles de cómo se usa BTCPayServer en tu Raspiblitz en este tutorial (en Inglés): https://coincharge.io/en/raspiblitz-btcpay-server/

Después de la instalación, verás `BTCPayServer` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### LNbits

LNBits es un sencillo pero poderoso servidor para administración de cuentas y carteras lightning. Tiene plugins que permiten funciones para E-commerce, paywalls, o wallets para tus amigos y demostraciones educativas.

![LNBITS](pictures/lnbits.png)

Se puede usar en combinación con IP2TOR para poder ofrecer:
- Volantes Lightning (Plugin: LNURLw)
- Términal de venta para mercaderes (Plugin: TPOS)

<a href="https://www.youtube.com/watch?v=0Bt3tHULAnw" target="_blank"><img src="pictures/video-vouchers.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=0Bt3tHULAnw

También puedes crear plugins adicionales.

[Detalles del servicio (en Inglés)](https://github.com/arcbtc/lnbits/blob/master/README.md)

Después de la instalación, verás `LNBITS` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### BTC-RPC-Explorer

BTC-RPC-Explorer es un explorador de la blockchain que puedes utilizar con la información de tu nodo. Mira un ejemplo de su uso en: https://btc-explorer.com

![EXPLORER](pictures/blockexplorer.png)

[Detalles del servicio (en Inglés)](https://github.com/janoside/btc-rpc-explorer)

Después de la instalación, verás `EXPLORE` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### Cryptoadvance Specter

Bitcoin Core tiene una poderosa CLI y un grandioso daemon. Es posible hacer uso de transacciones pre firmadas (PSBT) utilizando una [Hardware Wallet](https://github.com/bitcoin-core/HWI) (HWI). Por el momento el soporte para esta función está concentrada sobre todo en el sistema operativo Linux.

El objetivo de SpecterDesktop es ofrecer cómodamente las capacidades que el Bitcoin Core tiene para ofrecer; con énfasis en las opciones multi-firma que utilizan las wallets hardware como Trezor, Ledger, ColdCard o el Specter-DIY.

![SPECTER](pictures/specter.jpg)

Después de la instalación, verás `SPECTER` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

Como una alternativa a usar SPecter directamente en tu Raspiblitz, hay una versión para aplicación de escritorio que permite usarlo en tu laptop. Aquí hay una guía (en Inglés)  con los detalles para conectar esa aplicación directamente con tu nodo: https://d11n.net/connect-specter-desktor-with-raspiblitz.html

##### Mempool Explorer

![MEMPOOL](pictures/mempool.png)

Mempool es un explorador y visualizador de la blockchain quer funciona con la información de tu nodo. Mira como funciona en https://mempool.space

[Detalles del servicio (en Inglés)](https://github.com/mempool/mempool)

Después de la instalación, verás `MEMPOOL` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### JoinMarket

JoinMarket es una herramienta para realizar transacciones que se conocen como CoinJoin. Su objetivo es otorgar confidencialidad y anonimato a las transacciones en bitcoin.

<a href="https://www.youtube.com/watch?v=uGHRjilMhwY" target="_blank"><img src="pictures/video-joinmarket.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=uGHRjilMhwY

Una transacción CoinJoin requiere la presencia de otros participantes. La cantidad exacta debe estar en el momento y tiempo exacto. Al tratarse de un problema económico, más que técnico, JoinMarket trabaja para crear un mercado que posiciona estos recursos de la mejor manera.

Para más detalles [mira (en Inglés)](https://github.com/JoinMarket-Org/joinmarket-clientserver).

Después de la instalación, verás `JMARKET` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### Balance of Satoshi

Balance of Satoshi te da comandos mejorados para trabajar con tu liquidez LND.

[Detalles del servicio (en Inglés)](https://github.com/alexbosworth/balanceofsatoshis/blob/master/README.md)

Después de la instalación, verás `BOS` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### Sphinx Relay Server

Sphinx App te permite chatear sobre la Lightning Network siguiendo la idea del [Podcasting 2.0](https://u.today/father-of-podcasting-integrates-bitcoin-lightning-into-his-app). Para usarlo con la aplicación para celular, necesitas instalar [Sphinx Relay Server](https://github.com/stakwork/sphinx-relay/blob/master/README.md).

![SPHINX](https://github.com/stakwork/sphinx-relay/raw/master/public/relay.jpg)

Después de la instalación, verás `SPHINX` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### PyBlock

PyBlock es un set de comandos para obtener datos útiles y curiosos sobre la blockchain.

![PYBLOCK](pictures/pyblock.png)

[Detalles del servicio (en Inglés)](https://github.com/curly60e/pyblock/blob/master/README.md)

Después de la instalación, verás `PYBLOCK` como opción en el menu principal por SSH; al seleccionarlo tendrás la información necesaria para comenzar a usarlo.

##### Channel Tools (chantools)

Chantools ofrece ayuda para rescatar fondos bloqueados en los canales LND en caso de que dejen de funcionar.

[Detalles del servicio (en Inglés)](https://github.com/curly60e/pyblock/blob/master/README.md)

##### Download Bitcoin Whitepaper

Extrae una copia del whitepaper original de bitcoin directamente desde tu nodo.

#### SYSTEM: Monitoring & Configuration

![SYSTEM](pictures/system.png)

#### CONNECT: Connect Apps & Credentials

Esta opción ofrece soporte para conectar tu Raspiblitz a distintas aplicaciones para celular.

![CONNECT](pictures/connect.png)

##### MOBILE: Mobile Wallet Apps (Smartphones)

Al momento, las siguientes aplicaciones wallet están soportadas por Raspiblitz:

* [Zeus (iOS/Android)](https://github.com/ZeusLN/zeus)
* [Fully Noded (iOS over Tor)](https://apps.apple.com/us/app/fully-noded/id1436425586)
* [SendMany (Android)](https://github.com/fusion44/sendmany/blob/master/README.md)
* [Sphinx Chat App (iOS/Android)](https://sphinx.chat/)

Las Wallets móviles trabajan como controles remotos para tu Raspiblitz. Primero necesitas instalar la aplicación en tu smartphone. Raspiblitz ofrece códigos QR con acceso directo a la tienda de aplicaciones. Después necesitas `pair` (enlazar la aplicación) con tu Raspiblitz, también mediante un código QR que Raspiblitz genera. Si no tienes pantalla LCD, el código QR se ofrece en código ASCII para escanearlo en la terminal. (Tendrás que alejar el zoom para ver el código completo)

##### BTCPAY: Obtiene la conexión string para BTCPay Server

Encontrarás aqui el código string para conectar con tu BTCPay Server

##### bitcoinRPC

Si algúna app necesita acceso al bitcoin core, aquí encontrarás los detalles.

##### BISQ: Use your node with BISQ

Aquí puedes conectar tu nodo con la aplicación Bisq para acceder a sus funciones bitcoin core.

##### EXPORT: Macaroons and TLS.cert

Si quieres tener acceso a las APIs de LND (para conectar otras apps o servicios) necesitaras las credenciales mediante los archivos Macaroons y  TLS cert.

*Macaroons: Las llaves que permitirán que ciertas funciones de LND se ejecuten.*
*TLS: Certificado para asegurar y encriptar la comunicación con tu nodo.*

En este menú puedes reiniciar, resincronizar, o exportar las credenciales para que puedas usarlas en otros servicios.

Aquí las opciones para que puedas conseguir los archivos de identificación:

###### SSH Download

Los comandos SCP y SSH para transferir los archivos. Raspiblitz te dará el comando para que lo copies y lo pegues en una terminal de tu computadora y se ejecute la transferencia.

Este método es recomendable para conectarse con:
* [Zap Desktop Wallet](https://github.com/LN-Zap/zap-desktop)

###### Browser download

Abre una ventana de explorador para iniciar la descarga de tu archivo.

*Este método es el menos seguro porque cualquier persona con acceso a tu red local podría tener acceso al archivo durante la descarga. Útilizalo únicamente como último recurso.*

###### Hex-String

Los archivos Macaroons y TLS.cert pueden ser copiados y pegados en formato Hex-String desde el Raspiblitz hacia otra app que soporte el formato. Al elegir esta opción, Raspiblitz te dará las instrucciones para copiar el código.

Método recomendable para conectarse con:
* [Joule Browser Wallet](https://lightningjoule.com)

#### SUBSCRIBE: Subscription Services

Raspiblitz algunos servicios provistos por tercer; algunos son de pago.

![MainMenu-Services](pictures/subscriptions.png)

Sobre `LIST my Subscriptions` podrás ver la lista de tus suscripciones. Podrás cancelarlos con `CANCEL` en cualquier momento.

Al momento, las siguientes suscripciones están disponibles:

##### IP2TOR (de paga)

IP2TOR es un servicio de túnel informático con el que puedes correr servicios TOR de tu Raspiblitz a través de un puerto IP de la clearnet. De este modo puedes estar al alcance de cualquiera sin necesidad de comprometer la información de tu acceso a internet. No es necesario que te preocupes por la configuración de tu firewall o enrutador. El servicio se puede pagar directamente a través de Lightning en una suscripción de renovación automática.

Primero eliges a cuál servicio te gustaría brindarle un túnel. 

Verás una lista de los servicios disponibles. Elige `OK` sobre alguna oferta y Raspiblitz se encargará de construir el túnel. Ten en cuenta que para entonces ya deberías tener canales activos para poder completar el pago de la suscripción.

Si seleccionas `AGREE` en los detalles de la suscripción IP2TOR, la instalación se completará enseguida. Si todo funcionó correctamente, podrás encontrar la información en `MAINMENU` > `SUBSCRIBE` > `LIST My Subscriptions` y en donde podrás cancelarla también.

Para probar IP2TOR escoge en  `MAINMENU` el menú extra con el servicio al cuál deseas suscribir un enlace; después deberías obtener un nuevo URL. Puedes usar las API con el IP y puerto que se muestran en los detalles de la sección `LIST My Subscriptions`.

##### HTTPS con LetsEncrypt (gratis)

Si quieres que un servicio como BTCPay o LNBits sean facilmente alcanzables en internet (como con IP2TOR) la gente esperará que tu página ofrezca servicio HTTPS para que la comunicación entre el cliente y tu Raspiblitz sea encriptada. Puedes utilizar certificados HTTPS autofirmados pero esto sonará las alertas de los navegadores con los que los usuarios acceden a tus servicio; la alerta de seguridad no es del todo amigable. Es aqui donde puedes utilizar un LetsEncrypt para obtener un válido y gratis certificado HTTPS que es válido y seguro para casi todos los tipos de navegadores.

Necesitarás un dominio, por lo que puedes utilizar uno de [DuckDNS.org](https://www.duckdns.org) ... más opciones estarán disponibles en el futuro.

Cuando te suscribes a un LetsEncrypt, te será requerido tu subdominio de duckdns y el Auth-Token de tu cuenta. Entonces Raspiblitz intentará dejar todo listo para tí. Si todo funcionó, encontrarás la suscripción yendo a `MAINMENU` > `SUBSCRIBE` > `LIST My Subscriptions`, en donde también podrás cancelarlo cuando desees.

Para probar el túnel, ve a  `MAINMENU` y selecciona el servicio para el cuál deseas conectarlo. Debería darte una URL actualizada cuando accedas de nuevo a tus servicios.

#### PASSWORD: Cambia las contraseñas

Para cambiar tus contraseñas de seguridad.

#### REPAIR: Opciones para resetear, respaldar y reparar tu Raspiblitz.

El menú `REPAIR` te da opciones con las que puedes respaldar y dar soporte a tu Raspiblitz.

![RepairMenu](pictures/repairmenu.png)

Las opciones se explican a detalle a continuación:

##### SOFTWARE: Para correr pruebas de estado (DebugReport)

Esto te dará la información necesaria para identificar problemas con el software.

Útilizalo para cuando necesites ayuda, su información hará que otros entiendan mejor lo que le causó problemas a tu nodo.

##### BACKUP-LND: Respalda tu información LND (Rescue-File)

Esta función detiene tu Raspiblitz y genera un archivo de rescate-LND que puedes descargar via SCP hacia tu laptop o computadora. Puede ser usado para llevar la información de tu nodo, wallet y canales a otro Raspiblitz nuevo.

*ATENCIÓN: Si echaste a andar tu Raspiblitz utilizando un archivo de respaldo y vuelves a utilizar ese mismo archivo (ahora desactualizado) después, correrás el riesgo de perder los fondos de tus canales.*

##### MIGRATION: Migra la información de tu Raspiblitz a nuevo hardware.

Esta función detiene tu Raspiblitz y genera un archivo de migración-LND que puedes descargar via SCP hacia tu laptop o computadora. Puede ser usado para llevar la información de tu nodo, wallet y canales a un nuevo hardware, por ejemplo, de un HDD a un SSD. Para saber más sobre el archivo de migración [mira aquí (en Inglés)](README.md#import-a-migration-file).

*ATENCIÓN: Si echaste a andar tu Raspiblitz utilizando un archivo de migración y vuelves a utilizar ese mismo archivo (ahora desactualizado) después, correrás el riesgo de perder los fondos de tus canales.*

##### COPY-SOURCE: Ofrece la información de la blockchain a otro Raspiblitz.

Para acelerar el proceso de instalación, puedes conectar la copia de la blockhain de Raspiblitz a otro. Durante la transferencia, el Raspiblitz estará `offline` y podría demorar de 4 a 6 horas.

Asegúrate de que ambos Raspiblitzes están conectados a la misma red local. Durante la instalación del nuevo Raspiblitz, selecciona `COPY` para obtener la copia y después selecciona la `RASPIBLITZ` de origen. Ahora podrás activar la opción `COPY-SOURCE`. Inicia sesión utilizando su información de usuario (no el de tu nodo) y entonces el proceso debería comenzar.

##### RESET-CHAIN: Borra la blockchain y la vuelve a descargar

Utiliza esta opción si la información de tu blockchain se corrompió. Mantendrá tu información LND, incluso mantendrá los canales abiertos. Solo ten en cuenta que tu nodo aparecerá fuera de línea hasta que toda la blockchain se descargue de nuevo.

##### RESET-LND: Elimina la información de tu LND y comienza una nueva wallet-nodo

*ESTA OPCIÓN ELIMINA TODA LA INFORMACIÓN LND SOBRE TUS FONDOS*
*Úsala solo si antes has cerrado los canales y retirado los fondos*

Usa esta opción si quieres empezar con una nueva wallet; con nueva identidad, nombre y lista de palabras semilla. 

##### RESET-HDD: Elimina la información de tu disco duro pero mantiene la blockchain

*ESTA OPCIÓN ELIMINA TODA LA INFORMACIÓN LND SOBRE TUS FONDOS*
*Úsala solo si antes has cerrado los canales y retirado los fondos*

Usa esta opción si quieres comenzar un nuevo Raspiblitz pero no quieres descargar de nuevo la blockchain

##### RESET-ALL: Elimina todo completamente y comienza desde cero

*ESTA OPCIÓN ELIMINA TODA LA INFORMACIÓN LND SOBRE TUS FONDOS*
*Úsala solo si antes has cerrado los canales y retirado los fondos*

Usa esta opción si quieres comenzar un nuevo Raspiblitz como si fuera la primera vez.

##### DELETE-ELEC: Elimina el índice Electrum

Si tenías Electrum instalado, puedes utilizar esta opción para eliminar la información restante y liberar espacio en tu disco.

##### DELETE-INDEX: Elimina el TX-Index de Bitcoin

Si tenías la opción TX-Index activada y quieres eliminar la información para liberar espacio en tu disco, esta es la opción.

#### UPDATE: Revisa actualizaciones para tu RaspiBlitz

El menu `UPDATE` te da distintas opciones para actualizar tu Raspiblitz:

![UpdateMenu](pictures/update.png)

Las opciones se explican a detalle a continuación:

*Por favor ten en cuenta que Raspiblitz no soporta la función de actualizaciones automáticas*

##### RELEASE: Actualiza a la más reciente versión de Raspiblitz.

Es la forma más común para actualizar tu Raspiblitz. Selecciona esta opción para preparar tu Raspiblitz para una nueva imagen para micromemoria SD que contenga la última versión.

##### PATCH: Parches para el código de Raspiblitz

Con los parches puedes actualizar los últimos scripts del Repo oficial de Raspiblitz en Github. Es una buena opción para gente que reporta errores y que quiere probar una solución rápida sin tener que esperar a la siguiente versión oficial. También funciona para personas que quieren utilizar sus propias versiones modificadas de Raspiblitz.

##### LND: Actualización LND intermedia

A veces el equipo de desarrollo de LND publica actualizaciones para su daemon. Algunas actualizaciones llegan a romper los canales; de este modo puedes actualizar cuando lo creas conveniente.

Para hacer esto, tendrás la opción `VERIFIED` que significa una actualización que ha sido probada en el Raspiblitz o la opción `RECKLESS` con el que vas a obtener la actualización directamente desde el repo de LND, aún para las versiones en prueba; esta última opción es más para personas que buscan probar aplicaciones nuevas de trabajo y experimentales.

##### BITCOIN: Actualización Bitcoin intermedia

Al igual que en la opción anterior, aquí podrás tener las opciones para actualizar el Bitcoin-Core.

#### REBOOT: Reinicia tu RaspiBlitz

Una forma segura de reiniciar tu Raspiblitz. "¿Ha intentado apagarlo y encenderlo de nuevo?"

#### OFF: Apagar tu RaspiBlitz

Una forma segura de apagar tu RaspiBlitz.

#### X: Consola terminal

Cierra el menú SSH y sale a la terminal donde el usuario puede hacer uso de comandos y clientes CLI como `bitcoin-cli` y `lncli` directamente.

Con el comando `raspiblitz`, es posible regresar al menú principal.

## Importa un archivo de migración

Como mencionamos anteriormente; puedes exportar un archivo de migración de tu Raspiblitz en MAINMENU > REPAIR > MIGRATION y transferirlo a tu laptotp o computadora.

Un archivo de migración contiene la información necesaria para instalar Raspiblitz en un nuevo hardware; contiene la información de LND, bitcoin wallet, raspiblitz.config, llaves Tor y SSH, así como alguna información de tus aplicaciones instaladas. 

Si quieres importar hacia una nueva Raspiblitz (por ejemplo, a una versión más actualizada) puedes escoger la opción `MIGRATION` durante las primeras pantallas de instalación, después de la prueba de hardware y cuando Raspiblitz te pregunta si vas a usar Bitcoin o Litecoin.

![SSH0](pictures/ssh0-welcome2.png)

Si comienzas una migración, necesitarás formatear tu disco duro en el siguiente paso.

![MIGRATION1](pictures/migration1.png)

Aquí normalmente escoges el formato EXT4. Pero también existe la opción BTRFS para cuando existen opciones experimentales para Raspiblitz. Mira [más detalles en el FAQ](FAQ.md#why-use-btrfs-on-raspiblitz).

Después podrás subir el archivo de migración a tu Raspiblitz. Sigue las instrucciones que se te muestran.

Después necesitarás obtener una copia de la blockchain.

![MIGRATION2](pictures/migration2.png)

Recuerda que tendrás las opciones: [SYNC](README.md#1-sync---selfvalidate-all-blocks) y [COPY](README.md#2-copy---copy-from-laptop-or-another-raspiblitz-over-local-network), igual que en la configuración inicial.

RaspiBlitz reiniciará y comenzará el proceso de restauración siguiendo la configuración de acuerdo con el archivo raspiblitz.config contenido en tu archivo de migración.

Después la blockchain se va a sincronizar y al final todo volverá a la normalidad.

## Haz un RaspiBlitz partiendo desde tu Umbrel o myNode

Otro tipo de migración es para cuando ya tienes un nodo corriendo con el software de Umbrel o myNode y quieres cambiarte a Raspiblitz sin cerrar tus canales. Básicamente tienes el hardware, por lo que solo necesitas cambiar el sistema operativo. No necesariamente necesitas la pantalla LCD, RaspiBlitz también fuede funcionar sin ella.

*NOTE: Esta migración todavía es experimental. Todavía tendrás que utilizar tu terminal para manejar tu Raspiblitz. Si eso es demasiado técnico para ti, espera a la versión 1.8 de Raspiblitz, que incluirá una interfaz web para tu navegador que hará que la migración sea más amigable para usuarios de otros nodos parecidos.*

Antes de que comiences la migración:
* si tienes fondos en tu viejo nodo, asegúrate de traer contigo tu lista de palabras semilla
* si tienes canales activos en tu nodo, asegúrate de traer contigo una copia del archivo de respaldo Static Channel Backup

También ten en cuenta que Raspiblitz únicamente podrá transferir al momento tu blockchain y la información de tu wallet LND (canales incluidos). La información de las aplicaciones y servicios extra no pueden ser transferidos y podrían perderse.

Intrucciones para migración.
* Apaga tu viejo nodo
* Retira la microtarjeta SD
* [descarga la más reciente versión de Raspiblitz y flashea la imagen](#downloading-the-software)
* Si lo que quieres es utilizar un monitor HDMI para revisar el estado y progreso, crea un archivo vacío llamado 
`hdmi` (sin ningúna extensión) en la microtarjeta SD cuando la tengas conectada a tu laptop o computadora.
* [Inserta la microtarjeta, enciéndelo e inicia sesión](#boot-your-raspiblitz)

Raspiblitz debería mostrarte la información detectada para ofrecer continuar con el proceso.

* Si continúas, Raspiblitz recuperará la información y después se reiniciará.
* El modo de recuperación de Raspiblitz estaría comenzando; demoraría un tiempo hasta que finalmente se reinicie.
* Inicia sesión y reestablece tus contraseñas  (`FINAL RECOVERY LOGIN` en el LCD). Después un último reinicio será necesario..
* Inicia sesión por SSH con tus nuevos datos y desbloquea la wallet LND con la contraseña C. La blockchain necesitará ponerse al corriente pero después tu Raspiblitz debería estar listo mostrarte en el menú INFO tu balance on-chain y de canales.

Si no tienes ningún monitor LCD o HDMI, puede que sea un poco cpomlicado conectarte a tu Raspiblitz para revisar el estado en el que se encuentra. Solo intenta hacer login SSH una vez más cada que se reinicie, a veces puede demorar un tiempo en reaccionar.

## Interface / APIs

Para desarrollar tus propios scripts y apps y conectarlos con servicios en tu Raspiblitz. Tienes múltiples interfaces API disponibles:

### Bitcoin

* `bitcoin-cli` interfaz de líneas de comando para bitcoin
* `bitcoind` corriendo en el puerto 8333 (público)
* `JSON-RPC` corriendo en el puerto 8332 (local) [DOC](https://en.bitcoin.it/wiki/API_reference_%28JSON-RPC%29)

### LND-Lightning

* `lncli` interfaz de líneas de copmando para LND [DOC](https://api.lightning.community/)
* `lnd` corriendo en el puerto9735 (público)
* `gRPC` corriendo en el puerto 10009 (público) [DOC](https://api.lightning.community/)
* `REST` corriendo en el puerto 8080 (público) [DOC](https://api.lightning.community/rest/index.html)

Si activas TOR, entonces tugRPC  LND y APIs REST APIs también podrán ser enlazados como servicios incógnito.

### Backup para la información On-Chain- y fondos en Canales

Desde la versión v0.6 de LND (y v1.2 de RaspiBlitz), una función llamada Static-Channel-Backups estará disponible. Dentro del Raspiblitz puede ser usado para obtener un archivo `channel.backup` como hemos mencionado anteriormente.

Es recomendable tener archivos de respaldo para proteger los fondos en tus canales y nodo. 

Para recuperar tus fondos de este modo, necesitarías dos cosas:
- la lista de 24 palabras semilla
- el último archivo `channel.backup`

Deberías tener escrita la lista de palabras semillas de cuando iniciaste tu wallet LND; mantenla a salvo (offline) y en un lugar seguro. El archivo `channel.backup` es almacenado en el disco duro y se actualiza por LND cada que un nuevo canal es abierto o cerrado. La más reciente versión es necesaria para recuperar tus fondos. En caso de que tu disco duro se dañe, Raspiblitz mantendrá una copia del último archivo `channel.backup` en la microtarjeta SD en el sub-directorio: `/home/admin/.lnd/data/chain/`.

So quieres ir un paso más allá aseguirando tus fondos ante una perdida total de tu Raspiblitz (que se descomponga por completo, te lo roben o lo pierdas) entonces puedes adicionalmente planificar un respaldo del archivo `channel.backup`. El archivo en sí está encriptado con tu contraseña, por lo que de seria relativamente seguro almacenarlo con algún tercero. 

Este video explica como funcionaría el proceso (en Inglés):

<a href="https://www.youtube.com/watch?v=5wi6l9jRVQs" target="_blank"><img src="pictures/video-backup.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=5wi6l9jRVQs

Las siguientes opciones se explican brevemente a continuación:

#### A) Respaldo con DropBox

Activa la opción StaticChannelBackup DropBox dentro de `SETTINGS` en el menú de tu RaspiBlitz. Te pedirá el token de autenticación de Dropbox, para obtenerlo realiza lo siguiente:

Ve a tu navegador:

1. Abre la dirección https://www.dropbox.com/developers/apps/create inicia sesión o crea una cuenta nueva.

1. Selecciona **Create App**.

    ![Dropbox API 1](https://github.com/rootzoll/raspiblitz/raw/v1.6/pictures/dropbox-1.png)

    Selecciona entre 'Scoped Access' o 'App Folder' y elige un nombre fijo, por ejemplo `LNDbackup` con un número aleatorio adicional. Acepta los térmios y condiciones de uso y después selecciona 'Create App'.

1. Configura los **Permissions**.

    ![Dropbox API 2](https://github.com/rootzoll/raspiblitz/raw/v1.6/pictures/dropbox-2.png)

    Es importante que vayas a la pestaña `Permissions` y actives los permisos del `files.content.write`. No olvides dar `Submit` a los cambios antes de continuar.

1. Genera tu **OAUth2 Token**.

    ![Dropbox API 3](https://github.com/rootzoll/raspiblitz/raw/v1.6/pictures/dropbox-3.png)

    Ahora ve de vuelta a la pestaña 'Settings' debajo de 'OAuth2' y da click en el botón 'Generate'. Verás un largo código con números y letras; ese es tu **Dropbox-Authtoken**. Aségurate de copiarlo completamente, puede haber más texto si revisas más abajo. 

Para probarlo, intenta abrir o cerrar un canal. Después revisa si puedes encontrar una copia del archivo `channel.backup` en tu Dropbox. Puedes monitorear el registro de esta herramienta ingresando en la terminal el comando: `sudo journalctl -f -u background`

#### B) Respaldo manual SCP

*Puedes realizar un respaldo SCB hacia tu propia computadora o servidor, pero necesitarás hacerlo manualmente*

En el archivo de configuración `/mnt/hdd/raspiblitz.conf` el parámetro `scpBackupTarget='[USER]@[SERVER]:[DIRPATH-WITHOUT-ENDING-/]'` puede activar esta opción. En el servidor remoto necesitarás una copia de la llave del usuario root del Raspiblitz para que no haya necesidad de ingresar contraseñas y el script pueda funcionar como tarea de fondo.

El script `/home/admin/config.scripts/internet.sshpubkey.sh` ayuda con el arranque (init); te mostrará el proceso para hacer una copia de la llave-ssh al servidor externo.

Para probarlo, intenta abrir o cerrar un canal. Después revisa si puedes encontrar una copia del archivo `channel.backup` en tu servidor externo. Puedes monitorear el registro de esta herramienta ingresando en la terminal el comando: `sudo journalctl -f -u background`

#### C) Respaldo manuel en una memoria USB

*También puedes configurar la opción de respaldo utilizando una memoria USB:*

Cualquiera con capacidad de almacenamiento arriba de 120MB está bien. No utilices un segundo disco duro porque podría ocupar mucha energia y comprometer la seguridad y rendimiento de la Raspberry y el disco con la información importante de tus fondos y canales.

Para activar esta opción ve a `MAINMENU` > `SETTINGS` > `StaticChannelBackup on USB Drive` y sigue las instrucciones.

Para probarlo, intenta abrir o cerrar un canal. Después revisa si puedes encontrar una copia del archivo `channel.backup` en tu dirección de USB. Puedes monitorear el registro de esta herramienta ingresando en la terminal el comando: `sudo journalctl -f -u background`

## Actualizar el Raspiblitz a una nueva versión

Si tienes una versión de Raspiblitz anterior a la version 1.0, [mira aquí](FAQ.md).

Si tienes un Raspiblitz versión 1.2 o mayor; sólo sigue las instrucciones en la opción `UPDATE` desde el menú principal (escoge `RELEASE` si te pregunta) y sigue las instrucciones. Mira el proceso a detalle en el siguiente video (en Inglés).

<a href="https://www.youtube.com/watch?v=Xvn0WQfHUdI" target="_blank"><img src="pictures/video-update.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=Xvn0WQfHUdI

Si tienes un RaspiBlitz v1.0 o v1.1 o mayor, has lo siguiente:

* Ve a "Main menu" y selecciona "OFF"
* Retira el cable de la corriente de energía
* Retira la microtarjeta SD

Ahora descarga la nueva versión de Raspiblitz y flashea la imagen en la microtarjeta SD. Puedes sobre escribir la que ya tienes, pero sería recomendable conservar una segunda con la versión actual por si acaso. Mira los detalles sobre la última versión [aquí](#installing-the-software).

*Si hiciste cambios manuales al sistema (instalación de paqueterías, scripts nuevos, etc) quizás tengas que hacer unos preparativos previos a sobreescribir tu microtarjeta SD; para saber más, mira el [FAQ](FAQ.md#why-do-i-need-to-re-burn-my-sd-card-for-an-update).*

Si lo hiciste correctamente, simplemente coloca la microtarjeta SD de vuelta al Raspiblitz y enciéndelo de nuevo. Después sigue las instrucciones en la pantalla... pero no te preocupes, no será necesario volver a descargar y sincronizar la blockchain; pero es importante que tengas en cuenta que los datos de acceso por SSH serán reiniciados y necesitarás utilizar la contraseña y usuario `raspiblitz`. Más adelante en el proceso podrás renovar tus contraseñas.

* [¿Por qué necesito volver a flashear una microtarjeta SD para actualizar mi Raspiblitz?](FAQ.md#why-do-i-need-to-re-burn-my-sd-card-for-an-update)

## Construye una microtarjeta SD

Una microtarjeta SD con el archivo de imagen de RaspiBlitz lo ofrecemos nosotros para que lo descargues. Para echarlo a andar rápidamente, vuelve más arriba en la guía; pero si lo que quieres es construirla por ti mismo, aquí una breve guía:

* Consigue la última versión 64-bit de RaspiOS: [DESCARGA](https://downloads.raspberrypi.org/raspios_arm64/images).
* Flashea la imagen en una microtarjeta SD: [TUTORIAL](https://www.raspberrypi.org/documentation/installation/installing-images/README.md).
* Añade un archivo llamado `ssh` al root de la microtarjeta SD montándola en tu laptop para activar el login SSH. 
* Inicia la tarjeta en el RaspberryPi e inicia sesión via SSH con `ssh pi@[IP-DE-TU-RASPBERRY]`. La contraseña es `raspberry`.

Ahora estás listo para comenzar la construcción con el script para construcción de microtarjeta SD (revisa el código para que decidas si estás de acuerdo con la configuración). Copia el siguiente comando en tu terminal y ejecútalo:

`wget https://raw.githubusercontent.com/rootzoll/raspiblitz/v1.7/build_sdcard.sh && sudo bash build_sdcard.sh`

En el enlace podrás ver cómo esta construido el script `build_sdcard.sh`. Puedes revisar lo que hace y lo que será instalado. Siéntete libre de ofrecer recomendaciones y comentarios.

El proceso completo demora un tiempo. Al final, la instalación de drivers para la pantalla LCD y un reinicio serán necesarios. Un usuario `admin` Será creado durante el proceso. Recuerda que la contraseña default es ahora `raspiblitz`. Después puedes acceder haciendo login de nuevo, esta vez con los nuevos datos ingresando: `ssh admin@[DIRECCION-IP-DE-TU-RASPIBLITZ]`. El proceso de instalación debería comenzar de nuevo automáticamente. Si no quieres continuar con la instalación en este momento, puedes usar esa misma microtarjeta SD para configurar multiples Raspiblitzes. Da click en `Cancel` y corre `/home/admin/XXprepareRelease.sh`. Una vez que el LCD se muestra en blanco y el indicador LED del Pi se ha apagado, puedes desconectarla de la corriente y retirar la microtarjeta SD. Habrás construido tu propia imagen Raspiblitz en una microtarjeta SD.

*Nota: Si pretendes autoconstruir microtarjetas SD como copias maestras y distribuirlas, mejor que utilices pequeñas de 8GB. Eso asegurará de que será adecuada para cualquiera de 16GB recomendada por Raspiblitz en un futuro.*

* [¿Puedo usar Raspiblitz en otra computadora aparte de un RaspberryPi?](FAQ.md#can-i-run-raspiblitz-on-other-computers-than-raspberrypi)
* [¿Cómo puedo construir otra imagen para microtarjeta SD además de la del repo oficial?](FAQ.md#how-can-i-build-an-sd-card-other-then-the-master-branch)
* [¿Cómo puedo construir mi propia imagen para microtarjeta SD?](FAQ.md#how-can-i-build-an-sd-card-from-my-forked-github-repo)

## FAQ

Aquí una corta selección de las más recurrentes preguntas en el FAQ:

* [¿Cómo hago un respaldo de mi nodo lightning?](FAQ.md#how-to-backup-my-lightning-node)
* [¿Cómo puedo recuperar los fondos de un Raspiblitz con fallas?](FAQ.md#how-can-i-recover-my-coins-from-a-failing-raspiblitz)
* [¿Esas alertas de voltaje son peligrosas?](FAQ.md#are-those-under-voltage-detected-warnings-a-problem)
* [¿Puedo usar Raspiblitz en otra computadora aparte de un RaspberryPi?](FAQ.md#can-i-run-raspiblitz-on-other-computers-than-raspberrypi)

¿Todavía tienes más preguntas? Revisa el [Archivo FAQ Raspiblitz](FAQ.md).

## Comunidad de desarrolladores

Cualquiera es bienvenido a integrarse para mejorar y extender las capacidades de Raspiblitz; se trata de un trabajo en progreso. [Mira los issues](https://github.com/rootzoll/raspiblitz/issues) Si quieres ayudar o aportar nuevas. Encontrarás los scripts utilizados para las interacciones con Raspiblitz dentro del folder `/home/admin` o en el subfolder de este repo Git `home.admin`.

Para echar un vistazo al desarrollo de Raspiblitz, es recomendable ver este video. (En Inglés, Julio 2020): [https://www.youtube.com/watch?v=QXUGg45CWLo](https://www.youtube.com/watch?v=QXUGg45CWLo)

Mira todos los detalles en el video "Como contribuir al desarrollo de Raspiblitz (Inglés)":

<a href="https://www.youtube.com/watch?v=ZVtZepV3OfM" target="_blank"><img src="pictures/video-contrib.png" alt="Video Tutorial" width="400"></a><br>--watch--> https://www.youtube.com/watch?v=ZVtZepV3OfM

El proyecto original [RaspiBolt](https://stadicus.github.io/RaspiBolt/)" es un tutorial que enseña como construir un nodo lightning en un nodo de RaspberryPi; el trabajo base sobre el cuál Raspiblitz es desarrollado. Muchas gracias a Stadicus :)

Sígueme en twitter [@rootzoll](https://twitter.com/rootzoll), vísitanos en el siguiente [#lightninghackday](https://twitter.com/hashtag/LightningHackday?src=hash) o encuentranos en alguna de nuestras reuniones en Berlín cada primer jueves del mes en el bar room77. Siéntete libre de invitarme una cerveza usando lightning. :)

* [¿Cómo puedo obtener más ayuda?](#support)
