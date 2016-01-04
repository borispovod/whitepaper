

#Crypti: Libro Blanco

### Fundación Crypti

#### **v2.1**

#### 31 de diciembre, 2015

__Escrito por__

* Boris Povod
* Max Kordek
* Olivier Beddows
* Mike Doty
* William Canevari
* Stas Oskin
* Matthew DC

__Traducido por__

* Fernando Sanz

# Indice de contenidos

1. Introducción
	1. Qué es Crypti
	2. Transfondo técnico
	3. Factores clave de innovación
	4. Componentes de Crypti
2. Clientes
	1. Crypti (Cliente liviano)
	2. Crypti: Delegate & Developer Edition (Cliente completo)
	3. Cliente _Mobile_
3. Consenso
	1. Delegados
	2. Comisión de red
	3. Peer-to-Peer
4. Características Fundamentales
	1. Nombres de usuario
	2. Contactos
	3. Multi-firmas
5. Aplicaciones Descentralizadas
	1. Máquina Virtual
	2. Dapps
	3. Desarrollo de Dapps
	4. Computación de las Dapps
	5. Consenso sobre las Dapps
	6. Nodos Maestros
	7. Almacenamiento
	8. Depositos / Extracciones
	9. Tokens
6. Fuentes


### 1. Introducción
#### __i. Qué es Crypti__
Crypti es una plataforma de última generación que permite el desarrollo y distribución de aplicaciones descentralizadas basadas en JavaScript usando un ecosistema amistoso y completo en características. 
Con Crypti, los desarrolladores pueden crear, publicar, distribuír y monetizar sus aplicaciones desde una sistema propio basado en cryptomoneda que utiliza blockchains a medida, contratos inteligentes, almacenamiento distribuído, y nodos computadores; todo desde con una única solución de la industria.

#### __ii. Trasfondo Técnico__

Crypti está escrito en Node.js[[1]](http://nodejs.org) en el backend, y HTML5 y CSS3 en el frontend. Trabaja asincrónicamente y permite el proceso rápido de las funciones tal como las transacciones de la red. La base de datos usa SQLite para habilitar el uso de consultas complejas.

#### __iii. Factores clave de innovación__

Crypti es la primera solución de aplicaciones descentralizadas escrita completamente en Node.js. Esto abre el ecosistema de Crypti a miles de actuales desarrollador sin la necesidad de habilidades adicionales. Cualquier desarrollador web que ya esté familiarizado con JavaScript y Node.js puede entrar de inmediato y comenzar a crear aplicaciones descentralizadas desde el primer dia.

Nuestra meta principal con Crypti era crear un sistema plug and play completo que permita a los desarrolladores hacer todo, desde el diseño, desarrollo, publicación, y monetización, desde una única plataforma descentralizada. En el ecosistema de Crypti, los desarrolladores pueden rápidamente implementar sus aplicaciones de JavaScript en los Nodos de Almacenamiento y Crypti Hosting, ser listados en el Dapp Store de Crypti, y tener acceso inmediato a los Nodos de Computos de Crypti para la ejecución del código. Todo ésto respaldado por la integridad y seguridad que otorga la funcionalidad de consenso del sidechain de Crypti.

Para completar el círculo, todas estas funcionalidades de nube, son ejecutadas por los usuarios y delegados de Crypti, quienes reciben su paga a través de un sistema de pagos integrado (o por la red misma en el caso de los delegados) y en XCR (La cryptomoneda propia de Crypti) o en BTC. Verdaderamente es una herramienta única para el desarrollo de aplicaciones con tecnología de vanguardia, con costos razonables y un paradigma innovador.


#### __iv. Componentes Crypti:__

1.	Hosting P2P descentralizado para dapps
2.	Almacenamiento P2P descentralizado para dapps
3.	Cómputos descentralizados
4.	Consenso en sidechain para cada dapp
5.	Interfaces API de Crypti y Bitcoin
6.	Herramientas de desarrollo: crypti-cli / Toolkit

### 2. Clientes
#### __i. Crypti (Cliente liviano)__

El cliente liviano es generalmente usado por los usuarios regulares para acceder a sus cuentas de Crypti.

Está disponible para Windows y Mac OS. No conlleva instalación, ya que utiliza tecnologías web modernas. No actúa como nodo en la red, porque solo se conecta a otros peers que estén online via conexión http. Esto trae varias ventajas.

El usuario no tiene que descargar el blockchain, lo que reduce considerablemente el tamaño de la aplicación. Tampoco hace broadcast de las claves secretas a través de la red, todos los datos son firmados localmente en el dispositivo del usuario.
Permite hacer todos los tipos de transacciones disponibles. 

Si el usuario desea servir un nodo delegado, puede registrar una cuenta de delegado con el cliente liviano. Pero no es posible correr un delegado desde el mismo, ej.: crear nuevos bloques. Para ello necesitará el cliente completo.

Los usuarios de las dapps tambien pueden usar el cliente liviano para acceder a sus dapps instaladas. La API de Dapps y de peers están disponibles para los desarrolladores.
Gracias a éstas es posible crear rápida y facilmente dapps en JavaScript con nw.js[[2]](https://github.com/nwjs/nw.js) ó Electron[[3]](https://github.com/atom/electron).

El cliente completo sin embargo es la mejor ópción para usuarios avanzaos, delegados y desarrolladores. Está disponible para Windows, Mac OS y GNU/Linux. Sin embargo sólo en el cliente de Linux es posible ser delegado. Los usuarios del cliente liviano se pueden conectar a los clientes completos para acceder a la red.

Tambien puede usarse para hacer llamadas al API, siempre que esté permitido por el propietario del cliente completo. Todos los usuarios del cliente completo descargan el blockchain desde otros usuarios a través de una conexión P2P.

#### __2ii. Crypti: Delegate & Developer Edition (Cliente completo)__


El cliente completo sin embargo es la mejor ópción para usuarios avanzaos, delegados y desarrolladores. Está disponible para Windows, Mac OS y GNU/Linux. Sin embargo sólo en el cliente de Linux es posible ser delegado. Los usuarios del cliente liviano se pueden conectar a éstos clientes completos para acceder a la red.

Tambien puede usarse para hacer llamadas al API, siempre que esté permitido por el propietario del cliente completo. Todos los usuarios del cliente completo descargan el blockchain desde otros usuarios a través de una conexión P2P.

#### __2iii. Cliente *Mobile*__

El cliente *mobile* permite al usuario acceder a su cuenta Crypti en cualquier lado. Estará disponible tanto para IOS y Android y destacada en el app store de Apple y Google Play.

La infraestructura de backend para el cliente móvil, espejará aquellas del cliente de escritorio. El cambio real viene en forma de adiciones y mejoras a la interfaz de usuario que permitirán una experiencia a medida en dispositivos móviles.

La aplicación fue diseñada a medida para proveer una interfaz familiar y fácil de usar, muy parecida a las apps de Bitcoin o Home Banking que son utilizadas a diario masivamente.

Permitirá también lanzar todas tus Dapps favoritas desde la propia aplicación. En el futuro, planeamos integrar funcionalidades específicas de los dispositivos como la habilidad de utilizar la huella dactilar o escaneo de retina para sumar seguridad a la cuenta de usaurio.

### 3. Consenso

Crypti se basa en el mecanismo de consenso denominado DPoS[[4]](http://wiki.bitshares.org/index.php/BitShares) (Delegated Proof of Stake ó Prueba de Participación delegada). Este método de consenso fue creado originalmente por el equipo de BitShares.

DPoS se basa en delegados creando bloques. Los mismos son cuentas confiables, elegidas para ser "Delegados Activos". Las 101 cuentas de delegado con la mayor cantidad de votos crean los bloques. Las restantes cuentas de delegados se denominan “Standby Delegates” o "Delegados en espera", y pueden avanzar hacial al listado de top 101 si reciben los votos suficientes de otros usuarios Crypti. Todos los usuarios tienen disponibles 101 votos para introducir a sus delegados favoritos en la lista de top 101. El peso de cada uno de los 101 votos es proporcional al monto de XCR que el usuario posee en el *wallet* desde el cual emite los mismos. Este monto total se muestra en el listado de delegados como “Approval” o "Aprobación", y se lista como porcentaje de los 100 millones de XCR disponibles con respecto a los votos de cada delegado.

La promoción de los delegados a la lista de top 101, o su remoción hacia la lista de espera se concreta al momento de completar el ciclo de generacion del bloque 101. Cada ciclo de 101 bloques es creado por el top 101 de delegados de forma aleatoria. El timpo entre bloques de de 10 segundos. 

Los bloques nuevos se emiten a la red y se agregan al blockchain.
Luego de 6 a 10 confirmaciones, un bloque, junto con sus transacciones, puede ser considerado como confirmado. Un ciclo completo de generación de 101 bloques toma aproximadamente 16 minutos.

En DPoS, pueden ocurrir *forks* (derivaciones), pero el fork mas largo gana. Los delegados deben estar online todo el tiempo y tener suficiente tiempo de *uptime*. Este tiempo es considerado para catalogar la fiabilidad de cada nodo, tras anotar cada vez que un nodo pierde un bloque que le fue asignado. Los usuario votan el top 101 de delgados basados en unos cuantos factores, siendo uno de estos el principal para tomar una determinación. Si un delegado queda debajo de cierta puntuación, los usuarios pueden quitarle los votos debido al bajo rendimiento.

#### __i. Delegados__

La función de los delegados es descrita en la sección anterior, titulada "Consenso".

Un usuario debe registrar una cuenta de delegado para poder serlo. Esto se logra desde la interfaz de usuario tanto del cliente liviano como el completo. Ten en cuenta que la generación de bloques solo es posible en el cliente completo, lo que significa que es posible crear una cuenta de delegado en ambos *wallets* pero solo en el completo se pueden realizar las tareas de delegado. El numero de cuenta y nombre de usuario serán los mismos luego de la registración como delegado. Todas las cuentas Crypti pueden ser votadas como delegados.

Los nuevos delegados, empiezan como delegados "en espera". Los mismos comienzan con un porcentaje de aprobación de 0 (cero) y necesitarán juntar votos de la comunidad Crypti para poder avanzar hacia la lista de los 101 más votados y convertirse efectivamente en un delegado activo.
La generación de bloques se realizas por los 101 más votados únicamente.
Mientras estés en estado de espera, no generarás ningún bloque.

#### __ii. Comisiones de la red__

Todas las transacciones válidas de la red deben ser procesadas. Los delegados las procesan y las alojan en nuevos bloques. Para que ésto funcione, los delegados reciben una comisión. Todas las transacciones deben contener algun tipo de comisión, esto es una medida para evitar el spam.

La comisión por defecto de la red para hacer una transacción de XCR es del 0.1%. Por ejemplo, una transacción de 100 XCR incluye un adicional de 0.1 XCR totalizando una transacción de 100.1 XCR.

__La siguiente es una lista de comisiones para distintas transacciones:__

* 0.1% del monto para depósitos.
* .5 XCR por el registro de una segunda frase de seguridad
* .100 XCR por el registro de un nombre de usuario
* .100 XCR por registrarse como delegado
* .1 XCR para agregar un contacto
* .500 XCR para registrar una Dapp
* .5 XCR por miembro para registrar un grupo multi-firma.

Los delegados reciben las comisiones de todas las transacciones del último ciclo de bloques (101 bloques).

Las comisiones son repartidas de forma equitativa entre todos los delegados que crearon un bloque en ese ciclo. Los que no pudieron crear un bloque que le fue asignado durante el ciclo, no reciben su paga.

#### __iii. P2P__

Utilizamos una red P2P estándar[[5]](https://en.wikipedia.org/wiki/Peer-to-peer), que trabaja sobre el protocolo HTTP, y JSON como formato de intercambio de datos. El módulo P2P captura la siguiente información de cada "peer":

Versión
OSIP
Puerto

### 4. Características fundamentales

#### __i. Nombres de usuario__

Crypti allows users to register usernames. Which act as an alias to your account. Other users can send transactions to this username and the linked account will then receive it. This eliminates the need to remember long account addresses.

The network fee for username registration is 100 XCR. Usernames may contain the following characters:

* Traditional Alphabet (Upper & Lower Case): A-Z, a-z
* Numbers: 0-9
* Special Characters: !, @, $, &, and __.__
* Each username is unique. 
* The length is currently limited to 16 characters. 

Currently, it is not possible to remove a username from your account.

#### __ii. Contacts__
Crypti allows users to maintain a contact or friends list. This feature can be used to store frequently used accounts, but can also be used as a reputation system. If an account has many confirmed contacts, it may be considered more reputable than one without.

Contacts work like followers on Twitter. A user is added to the contact list, which will then show as a pending contact request in the user's wallet. Regardless of whether or not the other user accepts the request, they will be shown in the contact list. Once the other user accepts the request, the requester will be added to his contact list as well. Both parties now have a new confirmed contact.

The network fee for adding a new contact or accepting an incoming request is 1 XCR.

#### __iii. Multi-signatures__
Crypti allows users to create a multi-signature group. A multi-signature group consists of several Crypti users, called group members. Transactions from multi-signature groups can be configured to require some or all signatories for approval.

*To achieve this a **M of N* multi-signature architecture is implemented. All members of a multi-signature group (N) are added, up to a maximum of 16 signatories, and then the required number (M) of signatures needed to approve a transaction is specified.

M must be greater than 1 and less than or equal than N. N is the number of members of the multi-signature group.

Once you initiate a transaction from the multi-signature group, all members will see this pending transaction and decide whether to approve or ignore it. Once the required number of confirmations has been collected, the group will allow the transaction and submit it to the blockchain.

The owners of a multi-signature group may change the rules of the group at any time with the approval of at least M of the signatories.

### 5. Decentralized Applications
#### __i. Virtual Machine__

The Crypti Virtual Machine is a safe Node.js VM. It can run untrusted JavaScript code. Which is a fork of Node.js that uses an API to connect to Crypti and connect Crypti to the VM. The Crypti VM is like the standard Node.js except that it disallows low level operations. For security, Crypti uses Seccomp[[6]](https://en.wikipedia.org/wiki/Seccomp). This is a sandbox mechanism implemented in the Linux kernel.

Developers can choose from a large library of NPM modules and use all of the power of JavaScript asynchronous programming[[7]](http://npmjs.org). The intent is for the global JavaScript community to be able to build within Crypti on top of established and accessible code.

#### __ii. Dapps__
A dapp is a decentralized application[[8]](https://github.com/DavidJohnstonCEO/DecentralizedApplications/blob/master/README.md) written in Node.js and JavaScript. It works with the Crypti VM using either the Crypti or soon the Bitcoin consensus algorithm. The Crypti VM is a scalable Node.js application that allows Node.js and JavaScript developers to write dapps. With current web technologies (HTML5/CSS3/JavaScript) the developer is able to create a powerful UI. Dapps can use custom Node.js packages from NPM (the Node.js package manager).

Regular users can launch the dapps on a Linux *Crypti: Delegate & Developer Edition* client or via the regular Crypti lite client on Windows or Mac OS.



*Dapp Use Cases*

#### __iii. Dapps Development__

Developers write dapps in JavaScript which allows the use of the full ecosystem of Node.js packages powered by NPM. The Crypti VM is integrated with the Crypti API. This API interfaces with the Crypti Blockchain and even with the Bitcoin blockchain. Each dapp runs in the Crypti VM, which removes many possible attack vectors and thus makes it much safer for the end user to start dapps on their local machine. The Crypt API is accessible by the dapp.

To make the dapp development as easy as possible the Crypti Foundation released crypti-cli, a command line interface which creates your own testnet and dapp environment by answering a few simple questions. Additionally we prepared a Dapp Toolkit, which gives developers a reference implementation of the most important dapp functionalities, and serves as a solid foundation upon which they can start building their decentralized applications.

Many libraries have been written to provide the full Crypti API functionality for developers “straight out of the box”. 

This API includes:

* Consensus API
* Crypti API
* Bitcoin API
* Database API

To open a dapp, the format:  
`http://ip:port/dapps/<dapp_id/username>`
is used.

#### __iv. Dapps Computation__

The Crypti Foundation is developing a system that allows for billing of CPU time. Where the Crypti VM uses its API to track how much CPU time is used to run a dapp. As a result, owners of nodes can run dapp master nodes in return for XCR or BTC payments.

The purpose of Crypti is to create a unique ecosystem, of which computation is one part. In the future, Crypti will have a submission manager to submit dapps to candidate nodes offering their service to run dapps and select the nodes meeting the specified resource requirements offering the best combination of price and performance. The node owners will earn revenue from providing computation, memory, storage and other resources.

This is referred to as Dapps Billing. You can compare it to the Heroku platform for  deploying applications.

#### __v. Dapps Consensus__
Each Dapp has its own unique private side chain which operates in synchronization with the Crypti block time and current block height.

Dapp sidechains are managed by a group of up to 101 master nodes, each of which have block generation enabled specifically for an individual dapp. The primary role of each master node is to process transactions and signify the validity of each block generated on the sidechain.

The signing of blocks by a master node against a given dapp is restricted by the dapp owners. Whom then approve individual Crypti accounts as master nodes, which then are allowed to forge on the Dapp’s side chain.

Sidechain consensus is maintained among the 101 master nodes using the same Delegated Proof-of-Stake (DPOS) method used to secure the Crypti blockchain. This allows individual master nodes to collect fees from each transaction as reward for securing the dapp's side chain.

The motivations behind this form of consensus are to prevent unnecessary enlargement of the Crypti blockchain and to retain individual sidechain autonomy, while at the same time, ensuring the integrity of each side chain is constantly upheld.

It should be noted as an optional alternative in the soon future, Crypti dapps can instead be secured by the Bitcoin blockchain using this same method.

#### __vi. Dapps Master Nodes__
Dapp master nodes are Crypti nodes with an installed dapp and with block generation enabled specifically for that dapp. Dapp owners need to approve individual Crypti accounts to be permitted to be a master node. The nodes process transactions and generate new blocks which are then secured by the Crypti Blockchain, making them the core of the dapp system.

#### __vii. Dapps Storage__
It is possible to host the dapps on decentralized peer-to-peer storage networks. The developers can also store data used by the dapps on those networks. There are already a few developed systems on the market and we are testing with our dapp platform. The nodes which host the dapps or store data will receive a fee for this service. The first decentralized storage solution we support is Sia10. Dapps are stored as a zip package, including the installation packages in Node.js which information are saved in the the package.json file.

As an alternative it is also possible to store dapps using existing centralized solutions, the first will be: GitHub. Allowing developers to host a given dapp’s source code and related assets within a GitHub hosted repository.

Once the dapps platform has had chance to mature, developers will be able to update dapps from their associated multi-signature dapp accounts. These multi-signature accounts will require M signatures before any changes can be applied to their associated dapps, according to the dapp’s individual multi-signature settings.




#### __viii. Dapps Deposits / Withdrawals__
Developers can use either XCR or BTC in their dapps11. Users of a dapp may deposit or withdraw funds from any given dapp. When XCR or BTC are sent to a dapp address, the funds appear in the dapp account. The funds will then become available for use within the dapp. This works the same way for BTC deposits as it does with XCR. BTC is sent to a special dapp address and then appears in the dapp Bitcoin wallet.

Dapp accounts are a special type of account created by the owner of a dapp. All deposited XCR or BTC will be stored in the associated addresses. For security reasons, only the use of multi-signature dapp accounts with trusted signers is recommended.

Withdrawals from dapps are processed by master nodes. When a withdrawal request is sent, the dapp master node processes it and moves the funds to the specified withdrawal address in the Crypti or Bitcoin blockchain.

#### __ix. Dapps Tokens__
Developers may implement custom tokens in their dapps, and use these tokens as the main currencies within their dapps. These tokens may be used in the same way as XCR or BTC, but the tokens cannot be moved directly from one dapp sidechain to another dapp sidechain. They must only move via the Crypti main chain.


### 6. Sources

* [1] Node.js Organization. [https://nodejs.org](https://nodejs.org)
* [2][https://github.com/nwjs/nw.js]
* [3][https://github.com/atom/electron]
* [4]Bitshares DPoS. [http://wiki.bitshares.org/index.php/BitShares]
* [5][https://en.wikipedia.org/wiki/Peer-to-peer]
* [6][https://en.wikipedia.org/wiki/Seccomp]
* [7][http://npmjs.org]
* [8]David Johnston. Decentralized Applications. [https://github.com/DavidJohnstonCEO/DecentralizedApplications/blob/master/README.md]
* [9] Factom. Merkle tree. [https://github.com/FactomProject/FactomDocs/blob/master/Factom_Whitepaper.pdf]
* [10]Sia. A decentralized storage solution. [http://siacoin.com]
* [11]Sidechains. Deposit/withdrawal sidechain. [https://www.blockstream.com/sidechains.pdf]
