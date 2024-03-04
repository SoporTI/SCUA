> [!TIP]  
> [Ver video](https://youtu.be/rNoGp2nfuxI)

Los paquetes de software suelen depender
de otras piezas de código para poder funcionar. Supongamos que estás instalando
un juego en tu computadora Windows. Quizás sea necesario que el programa deba hacer
algunos cálculos para permitir que la física del juego funcione correctamente y así reproducir los resultados
en forma de gráficos en la pantalla. Para realizar estas tareas, el juego podría depender
de un motor físico para hacer los cálculos y de una biblioteca de procesamiento
para mostrar los gráficos en la pantalla. Para que el juego funcione, tendrás que tener
todo ese software disponible para el juego. Confiar en otras piezas de software
para hacer que una aplicación funcione se llama "tener dependencias" ya que un bit de código
depende de otro para poder funcionar. En nuestro ejemplo, el juego depende
tanto del motor físico como de una biblioteca de procesamiento para poder ejecutarse. Pero un momento, ¿qué queremos decir
cuando nos referimos a una biblioteca? Puedes pensar en la biblioteca como una manera
de empaquetar un código útil que alguien más escribió. Este código está incluido
en una sola unidad. Los programas que desean utilizar
la funcionalidad que proporciona el código pueden beneficiarse de esto si es necesario. En Windows, estas bibliotecas compartidas se llaman
bibliotecas de enlace dinámico, o DLL para abreviar. Puedes encontrar más detalles
sobre bibliotecas de enlaces dinámicos en la siguiente lectura. Una característica súper útil de una DLL
es que la misma DLL puede ser utilizada por muchos programas diferentes. Esto significa que todo ese código compartido
no necesita cargarse en la memoria para cada aplicación que quiera usarlo,
por lo que se usa menos memoria en general. Por lo general, las aplicaciones de Windows
tienen muchas dependencias que se encuentran juntas
en un solo paquete de instalación, junto con algo llamado un archivo .msi
que le dice al instalador de Windows cómo reunir todos estos elementos. Esto significa que un paquete de instalación dado
tendrá todos los recursos y dependencias como las DLL,
allí en el paquete. El instalador de Windows también manejará
la gestión de esas dependencias y se asegurará de que estén disponibles
para el programa. En el pasado,
las cosas no siempre fueron tan buenas. Imagínate esta situación: Un reproductor de video que has estado usando
para reproducir películas en tu computadora utiliza gráficos DLL para reproducirlas
en tu pantalla. Acaba de salir un nuevo juego
que quieres jugar, así que también lo instalas. El juego viene con una nueva versión
de esa biblioteca de gráficos. Entonces el instalador del juego actualiza
la versión existente con la nueva DLL. De repente,
tu reproductor de video deja de funcionar. Resulta que el reproductor de video no sabe
cómo utilizar la nueva versión de la DLL, y entonces nos empezará a fastidiar. Sin embargo, en los modernos sistemas operativos de Windows,
el infierno de las DLL es un problema del pasado. Para solucionarlo, la mayoría de las bibliotecas compartidas
y los recursos en Windows son gestionados por algo llamado
ensamblados en paralelo o SxS. La mayoría de estas bibliotecas compartidas se guardan
en una carpeta en C:\Windows\WinSxS. Si una aplicación necesita utilizar
una biblioteca compartida para realizar una tarea, esa biblioteca se especificará
en algo llamado un manifiesto. Esto le dice a Windows que cargue la
biblioteca correspondiente de la carpeta SxS. El sistema SxS también admite el acceso
a múltiples versiones de la misma biblioteca compartida de forma automática. Así que cuando instalas software, no dejas sin soporte
a los programas que ya tienes. Además del manifiesto,
el sistema SSX y las dependencias crean paquetes combinados
junto con sus paquetes de instalación. Puedes utilizar un administrador de paquetes de Windows
para ayudar con la instalación y el mantenimiento de las librerías y otras dependencias
que tu software ya instalado necesita utilizar. Hablaremos de esto con más detalle
en nuestra lección sobre administradores de paquetes de Windows. Te daremos una vista previa mediante la funcionalidad de Windows
para la gestión de paquetes para PowerShell. Con el cmdlet de gestión de paquetes de Windows
llamado Find-Package, puedes localizar el software, junto con sus dependencias,
desde la línea de comandos. A propósito, un cmdlet es básicamente el nombre
que le damos a los comandos de Windows PowerShell que utilizan el formato verbo-sustantivo. Ya hemos usado muchos cmdlets
como get-help, select-string, etc. Hay cientos de cmdlets integrados a Windows
y hasta puedes escribir tus propios cmdlets. De acuerdo, volvamos a mi tarea actual. Supongamos que querías instalar
el paquete Sysinternals. Este es un conjunto de herramientas publicadas por Microsoft
que pueden ayudarte a solucionar todo tipo de problemas
en computadoras con Windows. Puedes descargar el paquete Sysinternals
del sitio web de Microsoft o podrías usar la funcionalidad
de gestión de paquetes. Primero tendremos que abrir un terminal PowerShell.
Para ello, escribimos PowerShell en el menú Inicio. Luego podremos intentar localizar el paquete de sysinternals
ejecutando el siguiente comando: Find-Package
sysinternals -IncludeDependencies. Un error. No se encontraron coincidencias. ¿Qué significa todo eso? Esta excepción se generó porque
el origen predeterminado de paquetes en PowerShell es la galería PowerShell,
que no contiene el paquete Sysinternals. Por suerte, todo lo que tenemos que hacer
es indicarle a PowerShell un lugar donde pueda encontrar
el paquete de Sysinternals. Y esto es un repositorio de paquetes
llamado Chocolatey. Profundizaremos más sobre Chocolatey
en el video sobre gestores de paquetes. Pero por ahora, solo debes saber que es un lugar donde podemos encontrar
todo tipo de paquetes de software de Windows. Entonces, antes de que podamos instalar algún paquete,
necesitamos agregar una fuente de paquetes que le indique a nuestra computadora dónde puede encontrar
los paquetes que queremos instalar. Ya que queremos usar Chocolatey
para encontrar nuestros paquetes, necesitamos agregarlo como una fuente de paquetes. Haremos esto con el comando
Register-PackageSource de PowerShell. Escribamos Register -PackageSource -Name chocolatey -ProviderName
Chocolatey -Location, .org/api/v2. Podemos verificar que ambas fuentes
del software están listas con el comando Get-PackageSource. Luego, intenta localizar nuestro paquete y sus dependencias de nuevo con Find-Package sysinternals -includeDependencies. ¡Excelente! Ahora que sabemos cuál es
el paquete que queremos, podemos utilizar un cmdlt llamado Install-Package
para instalar Sysinternals y sus dependencias correspondientes. Lo haremos en una lección posterior. Ahora es el momento de un refrigerio. Toda esta charla sobre Chocolatey mmmm.... ¡me dio hambre!