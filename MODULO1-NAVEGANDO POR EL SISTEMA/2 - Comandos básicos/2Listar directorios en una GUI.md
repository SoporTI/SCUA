> [!TIP]  
> [Ver video](https://youtu.be/1dT49m5Ms-A)

En los sistemas operativos, los archivos y carpetas o los directorios se organizan en un árbol de directorios jerárquico. Tienes un directorio principal que se ramifica y contiene otros directorios y archivos. A la ubicación de estos archivos y directorios la llamamos ruta de acceso.

La mayoría de las rutas de acceso en Windows se ven así: `C:\Users\cindy\Desktop`. En Windows, los sistemas de archivos se asignan a letras de unidad que se ven así: `C:`, o `D:`, o `X:`. Cada letra de unidad es un sistema de archivos. Recuerda que los sistemas de archivos se usan para rastrear los archivos en nuestra computadora. Cada sistema de archivos tiene un directorio raíz que es el superior para todos los demás directorios en ese sistema de archivos. El directorio raíz de `C:` se escribirá `C:\`, y el directorio raíz de `X:` se escribirá `X:\`.

Los subdirectorios están separados por barras inversas a diferencia de Linux, que utiliza barras comunes. Una ruta de acceso comienza en el directorio raíz de una unidad y sigue hasta el final de la ruta. Vamos a abrir esta PC y a navegar hacia nuestro directorio principal.

El directorio principal en un sistema Windows es la unidad en la que se almacena el sistema de archivos. En este caso, nuestro sistema de archivos se almacena en el disco local `C`. Desde aquí, voy a ir a Users (Usuarios), luego a mi carpeta de usuario, cindy, y por último a Desktop (Escritorio). Si nos fijamos en la parte superior, aquí, puedes ver la ruta de acceso en la que estoy. `Local disk\Users\cindy\Desktop` (Disco local\Usuarios\cindy\Escritorio). No fue tan difícil, ¿verdad?

Puedes ver aquí en nuestro directorio Desktop que tenemos algunas carpetas y archivos. Tenemos una carpeta llamada Puppy Pictures, una carpeta llamada Hawaii y un archivo llamado My Super Cool File. También hay algunos archivos aquí que no puedes ver. Los llamamos archivos ocultos. Están ocultos por algunas razones. Una es que no queremos que nadie vea o modifique accidentalmente estos archivos. Podrían ser archivos críticos del sistema o configuraciones o, peor aún, fotos vergonzosas tuyas en la escuela primaria con un corte de pelo tipo "mullet". Está bien, no eres la primera persona a la que le gusta llevar el cabello corto adelante y largo atrás.

Solo por diversión, veamos qué tipo de archivos ocultos tenemos aquí. Vamos a la parte superior y hacemos clic en `View` (Ver), luego marcamos la casilla de verificación `Hidden Items` (Elementos ocultos). Ahora podemos ver todos los archivos ocultos en nuestro sistema. Oh, interesante. Hay un archivo llamado `secret_file`. Por mucho que me gustaría curiosear, quien lo creó probablemente no quiere que veamos lo que hay dentro, así que vamos a dejarlo en paz.

Vamos a seguir adelante y revertir esta opción para no cambiar otra cosa accidentalmente. Bien, ¿y si quisiéramos ver información sobre un archivo? Bueno, para esto podemos hacer clic derecho y elegir `Properties` (Propiedades). Vamos a intentar esto con `My Super Cool File`.

En este cuadro de diálogo emergente podemos ver mucha información. Vamos a analizarlo. En la pestaña General podemos ver el nombre del archivo, el tipo de archivo, qué aplicaciones utilizamos para abrirlo y la ruta de acceso a la ubicación del archivo, que es `C\Users\cindy\Desktop`. Luego tenemos el tamaño del archivo y el tamaño en disco. Esto puede ser un poco confuso. El tamaño del archivo es, en realidad, la cantidad de datos que ocupa, pero el tamaño en disco es un poco diferente. No es algo que debas saber ahora mismo, pero si quieres aprender más al respecto, puedes consultar la siguiente lectura complementaria.

Muy bien, sigamos adelante. A continuación tienes marcas de tiempo de cuando el archivo fue creado, su última modificación y último acceso. Después de eso tenemos los atributos que podemos habilitar para nuestro archivo. Tenemos `Read-Only` (Solo lectura) y `Hidden` (Oculto). Puedes suponer que si marcas `Hidden` (Oculto), nuestro archivo estará oculto y solo será visible si habilitamos la función para mostrar elementos ocultos.

También hay algunas opciones avanzadas, pero no las veremos por ahora. También verás que hay algunas otras pestañas aquí, en la parte superior: `Security` (Seguridad), `Details` (Detalles) y `Previous Versions` (Versiones anteriores). Hablaremos más sobre la pestaña de seguridad en una lección posterior.

La pestaña `Details` (Detalles), básicamente, nos dice la información que acabamos de analizar sobre un archivo. La pestaña `Previous Versions` (Versiones anteriores) nos permite restaurar una versión anterior de un archivo por lo que si hiciste un cambio en un archivo y quieres revertir ese cambio, podrías volver a esa versión.

Para resumir el listado de directorios en la GUI de Windows, podemos ver la lista de archivos y carpetas de manera predeterminada aquí. Puedes cambiar la forma en que deseas verlos utilizando íconos o incluso una lista. Si deseas obtener más información sobre un archivo, puedes mirar sus propiedades. A continuación, veremos qué aspecto tiene toda esta información a través de la CLI de Windows.
