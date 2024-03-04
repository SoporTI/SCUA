> [!TIP]  
> [Ver video](https://youtu.be/kHfH_4J16kE)

En esta lección, vamos a hablar
de una parte importante de la computación, que hace que trabajar
en soporte de TI sea un poco más fácil. En realidad, les hace las cosas mucho más fáciles
a casi todos. Imagina esto:
estás en camino a una reunión importante. Estuviste ensayando para esta presentación
toda la semana y ahora estás listo para mostrarles
lo que tienes a los peces gordos. Pero espera, la presentación con diapositivas, ¿dónde está? No está en tu laptop. ¿Dónde podría estar? Resulta que olvidaste tu única copia
en tu equipo de escritorio, en casa; es demasiado tarde ahora para dar la vuelta y tomarla,
así que te sientas allí temiendo lo inevitable. Pero espera un minuto, de repente recuerdas
que tienes una conexión remota configurada desde tu laptop a tu equipo de escritorio. Usas esta conexión para acceder
a la computadora de casa y como si estuvieras sentado allí, puedes tomar el archivo de tu equipo de escritorio
y copiarlo a tu laptop. Luego,
procedes con una presentación increíble. Pensemos en otra situación. Compraste una computadora en una tienda
y tienes muchos problemas con ella. La tienda tiene una sección de soporte técnico,
que puede ayudarte con los problemas, pero es tarde y la tienda está cerrada. Realmente necesitas solucionar
el problema de tu computadora. Entonces, ¿cuáles son tus opciones? Por suerte, la tienda ofrece
soporte técnico 24/7 en línea. Ahora, en lugar de preocuparte hasta que la tienda física
abra de nuevo, puedes acceder a un técnico en línea y lograr que te ayude con tu problema
a través de una conexión remota. La conexión remota simplifica muchísimo
el trabajo de soporte de TI porque nos permite gestionar múltiples máquinas
desde cualquier parte del mundo. En esta lección, vamos a aprender
acerca de la conexión remota. En realidad, ya estuviste usándola
a lo largo de este curso. Estuvimos usando la conexión de escritorio remoto de Chrome
para acceder a nuestros Qwiklabs de Windows, junto con SSH, o Secure Shell,
para acceder en forma segura a nuestro Qwiklabs de Linux. Pero en esta lección vamos a ir un poco más a fondo
y hablaremos sobre cómo funciona la conexión remota y los diferentes métodos
para conectarse de forma remota a una máquina. SSH o Secure Shell es un protocolo implementado
por otros programas para acceder, de forma segura, a una computadora desde otra. En los ejercicios de Qwiklabs, estuviste usando
el cliente SSH de Google Cloud Console para acceder a las instancias de VM de Linux. Para usar SSH, necesitas tener un cliente SSH instalado
en la computadora desde la que te estás conectando, junto con un servidor SSH en la computadora
a la que estás tratando de conectarte. Ten en cuenta que cuando decimos servidor SSH, no queremos decir
otra máquina física que entregue datos. Un servidor SSH es solo software. En la máquina remota, el servidor SSH
se ejecuta como un proceso en segundo plano. Comprueba constantemente si un cliente
está tratando de conectarse a ella, entonces autenticará su solicitud. El programa más popular para usar SSH
en Linux es el programa OpenSSH. Lo usaremos en esta lección, pero todavía no hablaremos
sobre cómo instalarlo. Volveremos a eso en el próximo curso,
Administración de sistemas y servicios de infraestructura de TI. Lo mismo ocurre con Windows. Hablaremos sobre cómo usar SSH
desde una máquina de Windows usando el popular programa de código abierto PuTTY. Por ahora, solo hablemos de qué ocurre
cuando usas SSH. Te vamos a mostrar un ejemplo
de cómo hacer SSH en una máquina remota. Ya tenemos un cliente SSH
instalado en esta máquina, pero no te preocupes, vamos a hablar
de los diferentes clientes SSH y su instalación en el próximo curso del programa,
Administración de sistemas y servicios de infraestructura de TI. Lo primero es lo primero: para acceder a una máquina remota
tenemos que tener una cuenta en esa computadora. También necesitamos el nombre de host
o la dirección IP de esa computadora. Vamos a probar esto. Entonces: ssh cindy@ dirección IP. Recibimos este mensaje. La autenticidad del host, y por lo tanto la dirección IP,
no se puede establecer. Este mensaje solo dice que nunca
nos hemos conectado a esta máquina antes, y que nuestro cliente SSH no puede verificar
que nos estemos conectando a la máquina que queremos conectarnos. Pero podemos verificar
que esta es la máquina correcta. Sigamos adelante y escribamos "yes". Ahora, este host se guarda en la computadora
como un host conocido, por eso no volveremos a recibir este mensaje
cuando intentemos acceder a ella. Bien, ahora que estamos conectados
a través de SSH, cualquiera de los comandos de texto que escribamos
se envían de forma segura al servidor SSH. Desde aquí, incluso puedes iniciar una aplicación
que te permita ver una GUI en lugar de trabajar directamente en la shell. Puedes leer más sobre cómo hacerlo
en la lectura complementaria. Podemos conectar SSH usando contraseñas,
como viste antes. Esta forma de autenticar un equipo remoto
es bastante común, pero no es muy segura. La alternativa es usar
una clave de autenticación SSH. Las claves SSH vienen en un juego de dos claves
llamadas claves privadas y públicas. Puedes pensar en ellas como
llaves físicas reales para una caja fuerte especial. Puedes usar una llave para cerrar la caja fuerte,
pero no la abrirá. La otra llave, entonces, solo puede
abrir la caja fuerte, pero no cerrarla. Así es, básicamente, cómo funcionan
las claves públicas y privadas. Puedes bloquear algo con una clave pública, pero solo puedes desbloquearlo
con una clave privada y viceversa. Esto asegura que lo que sea que haya
en la caja fuerte, esté disponible solo para quienes tengan
ambas claves, la pública y la privada. Aprenderás sobre los detalles técnicos
de claves públicas y privadas en nuestro curso de seguridad informática. No te preocupes si esto no tiene sentido
en este momento, ya lo tendrá. Y así es cómo funciona SSH. No da mucho miedo, ¿verdad? Otra forma en la que puedes conectarte de forma segura
a una máquina remota es a través de una VPN. Una VPN es una red privada virtual. Te permite conectarte
a una red privada, como la red de tu trabajo, a través de Internet. Piensa en ello como un SSH más sofisticado,
con mucha más configuración. Te permite acceder a recursos,
como servidores de archivos compartidos y dispositivos de red,
como si te conectaras a la red de tu trabajo. Alerta de spoiler: también vamos a mencionar
los detalles técnicos por detrás de VPN en el curso de seguridad informática. Hemos visto mucho sobre las conexiones remotas
y cómo funcionan. Veremos más sobre los programas populares
de conexión remota para Windows y Linux y cómo configurarlos
en el curso de administración de sistemas.