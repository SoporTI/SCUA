> [!TIP]  
> [Ver video](https://youtu.be/RTI8qguASBs)

La capacidad de hacer conexiones remotas
es igualmente útil en computadoras con Windows, pero no hay un cliente de OpenSSH
para el SO Windows, al menos no todavía. Aunque eso está cambiando. Microsoft anunció
que va a colaborar con el proyecto OpenSSH para ofrecer una integración con PowerShell. Puedes leer el texto completo de su declaración
en la lectura suplementaria que está incluida después de esta lección. Es genial saber que Windows,
finalmente, integrará un cliente OpenSSH en PowerShell. Mientras tanto, ¿qué debe hacer un especialista en soporte de TI
si quiere tener SSH en otra computadora? Bueno, hay hosts de aplicaciones externas
que pueden funcionar como clientes SSH en Windows. Veamos una de las herramientas más populares,
PuTTY. PuTTy es un software gratuito de código abierto
que puedes usar para hacer conexiones remotas a través de varios protocolos de red,
incluido SSH. Puedes visitar el sitio web de PuTTy
para descargar el paquete de software completo con el Instalador de Microsoft. Son los archivos .msi
de los que hablamos antes. O puedes elegir un ejecutable específico
que te brinda la funcionalidad que estás buscando, como PuTTY.exe. Hay un vínculo a la página de descargas de PuTTY
en la siguiente lectura suplementaria en caso de que quieras probarlo. Después de descargar
y de instalar PuTTY, puedes iniciarlo a través de la GUI. Aparecerá una ventana en la que verás
las opciones básicas para conectarte. Tome nota del nombre del host, el puerto
y las opciones de tipo de conexión. El puerto predeterminado es el 22, ya que es
el puerto predeterminado que usa el protocolo SSH, y el tipo de conexión se establece como SSH. Todo lo que necesitas hacer
es escribir el nombre del host o la dirección IP de la computadora
a la que quieres conectarte. Luego, haz clic en Open (Abrir)
para comenzar una nueva sesión de SSH. Y ahora me conecté a una computadora remota
por medio de SSHD. Ejecutar PuTTy desde la GUI
no es tu única opción. También puedes usarlo en la línea de comandos. Abre una ventana de PowerShell
y escribe el nombre de la aplicación, así. Luego, agrega la opción -ssh para indicar
que quieres conectarte a través de SSH. También podrías indicar el usuario y la dirección
en la forma de usuario@direcciónIP, especificando el puerto al final. En conjunto,
el comando se vería más o menos así. PuTTy también viene con una herramienta
llamada plink o enlace PuTTy, que se integra en la línea de comandos
una vez que se instala PuTTy. También puedes usar plink
para hacer conexiones SSH remotas. SSH puede ser muy útil,
en especial si quieres conectarte desde una computadora que ejecuta Windows a un sistema operativo basado en Linux
que se ejecuta de forma remota. Microsoft proporciona otra manera de conectarse
a otras computadoras con Windows llamada Protocolo de escritorio remoto, o RDP. También hay clientes de RDP
para Linux en OS 10, como RealVNC, y Microsoft RDP en Mac. Agregaremos algunos vínculos a estos clientes
en la lectura complementaria. RDP proporciona a los usuarios
una interfaz gráfica de usuario a computadoras remotas siempre que la computadora remota tenga habilitadas
las conexiones entrantes RDP. Un programa cliente llamado
cliente de Microsoft Terminal Services, o MSTSC.exe, se usa para crear conexiones RDP
a computadoras remotas. Para habilitar conexiones remotas
en tu computadora, abre el menú Inicio, haz clic derecho en This PC (Este equipo),
luego selecciona Properties (Propiedades). Desde ahí, selecciona Remote settings (Configuración remota). Y luego elige una opción desde la sección
Remote desktop (Escritorio remoto) del panel. Permitir que las personas se conecten
de manera remota con tu computadora conlleva ciertas implicaciones de seguridad. Solo debes dejar que usuarios
en quienes confías hagan esto. En general, en un entorno del sector,
este tipo de ajustes lo establece el administrador del sistema a cargo
de las computadoras de la empresa que se conectan a la red. Una vez que tengas conexiones permitidas
en la computadora remota y siempre que estés en la lista
de usuarios autorizados para acceder a ella, puedes usar el cliente
del Protocolo de escritorio remoto, MSTSC.exe, para conectarte a ella
desde cualquier otro lugar de la red. Puedes iniciar el cliente RDP
de varias maneras. Puede escribir mstsc en el cuadro de ejecución o buscar conexiones de escritorio remoto
en el menú Inicio. Una vez iniciado el cliente,
te pedirá el nombre o la dirección IP de la computadora
a la que quieres conectarte. El cliente Windows RDP también puede iniciarse
desde la línea de comandos o puedes especificar más parámetros,
como /admin, si quieres conectarte a la computadora remota
con las credenciales administrativas que tal vez ya usaste
con el cliente de Windows RDP en Qwiklabs. Pero si no lo hiciste,
incluimos un vínculo a la documentación de RDP en la lectura complementaria
en caso de que quieras aprender más.