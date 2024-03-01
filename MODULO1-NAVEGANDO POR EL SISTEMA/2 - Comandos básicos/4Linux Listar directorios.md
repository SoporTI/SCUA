En Linux, el directorio principal del que todos los demás derivan se llama directorio raíz. La ruta de acceso al directorio raíz se marca con una barra diagonal. Un ejemplo de una ruta de acceso en Linux que comienza desde el directorio raíz es `/home/cindy/Desktop`. Al igual que `c:\Users\cindy\Desktop` en Windows.

Sigamos adelante y veamos qué hay debajo del directorio raíz. Vamos a usar el comando `ls` o "listar contenidos del directorio". También debemos darle a este comando la ruta de acceso al directorio que queremos ver. Si no indicamos la ruta de acceso, de forma predeterminada nos mostrará el directorio actual en el que estamos. Entonces: `ls /`.

Muy bien, ahora podemos ver todos los directorios listados en el directorio raíz. Hay muchos directorios aquí y todos se usan para diferentes propósitos. No vamos a pasar por todos ellos, pero vamos a hablar de algunos de los más importantes.

- `/bin`: este directorio almacena nuestros binarios o programas esenciales. El comando `ls` que acabamos de usar es un programa y se encuentra aquí, en la carpeta `/bin`. Es muy similar a nuestro directorio de archivos de programa en Windows.
- `/etc`: esta carpeta almacena algunos importantes y hermosos archivos de configuración del sistema.
- `/home`: este es el directorio personal para usuarios. Contiene documentos del usuario, fotos, etc. También es similar a nuestro directorio de usuarios de Windows.
- `/proc`: este directorio contiene información sobre los procesos actualmente en ejecución. Hablaremos más sobre procesos en una próxima lección.
- `/usr`: el directorio de usuario no contiene, en realidad, nuestros archivos de usuario como nuestro directorio principal. Está destinado para el software instalado por el usuario.
- `/var`: aquí almacenamos nuestros registros del sistema y básicamente cualquier archivo que cambie constantemente.

El comando `ls` tiene un par de indicadores muy útiles que podemos usar también. De forma similar a los parámetros de comando de Windows, un indicador es una forma de especificar opciones adicionales para un comando. Por lo general, podemos especificar un indicador colocando un guión y luego la opción correspondiente. Esto varía dependiendo del programa, sin embargo. Cada comando tiene diferentes opciones de indicador. Puedes ver qué opciones están disponibles para un comando añadiendo el indicador `--help`. Veámoslo en acción.

Hay una cantidad increíble de texto, pero no te asustes. No tienes que memorizar estas opciones. Esto se utiliza principalmente como referencia. Por ahora, vayamos rápidamente a través del menú de ayuda. En la parte superior te indica en qué formato poner el comando. Y aquí te da una descripción de lo que hace el comando. Este enorme texto enumera las opciones que podemos utilizar. Nos dice qué indicadores de comando están disponibles y lo que hacen. El indicador `--help` es muy útil, incluso los usuarios experimentados del SO lo consultan de vez en cuando.

Otro método que puedes usar para obtener información sobre comandos es el comando `man`, de "manual". Se usa para mostrarnos páginas de manual. En Linux las llamamos "man pages". Para usar este comando, simplemente ejecuta `man`, y a continuación, el comando que deseas buscar. Vamos a buscar `man ls`. Y aquí tenemos la misma información que en `--help` con un poco más de detalle.

Bien, volvamos a usar el comando `ls`. Ahora mismo, no es muy fácil de leer. Hagamos nuestra lista de directorios más legible con el indicador `-l`, de "largo". Muestra información detallada sobre archivos y carpetas en el formato de una larga lista. Ahora podemos ver información adicional sobre nuestro directorio y los archivos y las carpetas en ellos. Al igual que "Mostrar propiedades" en Windows, el comando `ls` nos mostrará la información detallada del archivo.

Vamos a desglosar esta salida empezando desde la izquierda. La primera columna aquí son permisos de archivo. Nota al margen: vamos a hablar sobre permisos de archivo en una próxima lección. Bien, lo siguiente es el número de vínculos que tiene un archivo. Una vez más, analizaremos esto en más detalle en una lección posterior. A continuación, tenemos el propietario del archivo, luego el grupo al que pertenece el archivo. Los grupos son otra manera en la que podemos especificar el acceso; hablaremos de esto en otra lección también. Luego tenemos el tamaño del archivo. La marca de tiempo de la última modificación, y por último, el nombre del archivo o directorio.

El último indicador que analizaremos para el comando `ls` es `-a`, o la opción "todo". Esto nos muestra todos los archivos en el directorio, incluidos los archivos ocultos. Notarás que agregué dos indicadores diferentes juntos. Es lo mismo que `ls -l -a /`. Ambos funcionan exactamente de la misma manera. El orden del indicador determina en qué orden funcionará. En nuestro caso, no importa si hacemos una larga lista primero o si mostramos todos los archivos primero.

Mira cómo algunos archivos nuevos se hacen visibles cuando usamos estos indicadores. El indicador `-a` o "todo" muestra todos los archivos, incluidos los ocultos. Puedes ocultar un archivo o directorio colocando un punto adelante como el archivo que se ve aquí, `.i_am_hidden`.

Abarcamos mucho en este video, aprendimos cómo ver información detallada sobre archivos con el comando `ls`. También comenzamos a usar rutas de acceso en la computadora y aprendimos a obtener ayuda con comandos usando el indicador `--help` y las man pages. Hasta pudimos curiosear en nuestro sistema de archivos Linux.

Si te pareció que avancé muy rápido por algo de todo esto, solo vuelve a ver el video. Nos volveremos a ver en el siguiente, donde empezaremos a cambiar directorios en la GUI. Nos vemos.
