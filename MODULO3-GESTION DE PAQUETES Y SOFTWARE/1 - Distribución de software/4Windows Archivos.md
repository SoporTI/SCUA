> [!TIP]  
> [Ver video](https://youtu.be/DdQ0i11jJ6E)

Un tipo de paquete
del que todavía no hablamos no es en realidad un paquete,
es un archivo Un archivo se compone de uno o más archivos que están comprimidos
en un solo archivo. Los archivos de paquetes son básicamente el núcleo o los archivos de software de origen
que se comprimen en un archivo Cuando instalamos software
de un archivo fuente, se conoce como
instalación desde la fuente. Los tipos de archivos más populares
que verás  son .tar,.zip y .rar. Para instalar el software de un archivo,
primero debes extraer los contenidos de la carpeta
para que puedas ver los archivos que hay adentro. Después, dependiendo del tipo
de código en que fue escrito, debes usar
un método específico para instalarlo. No veremos cómo
instalar desde la fuente, debido a que cambia según el lenguaje
en el que fue escrito el software. Sin embargo, analizaremos cómo extraer
los contenidos de un archivo, que es algo que deberás hacer muchas veces
como especialista en soporte de TI. No es solo software lo que hay almacenado en un archivo,
cualquier elemento puede archivarse, como imágenes o archivos de música. Verás muchos elementos de este tipo en soporte de TI. Para complicar las cosas aún más, existen muchas maneras diferentes
de extraer estos tipos de archivo. Por suerte, hay herramientas muy populares.
en Windows para archivar y desarchivar diferentes tipos de archivos
como .rar .zip y tar. Esta es la herramienta de código abierto 7-zip. Ya está instalada en mi computadora. Si quieres descargarla tú mismo, incluí un vínculo
en la lectura complementaria. Hay un archivo en mi escritorio
llamado colors.zip. Extraigamos el contenido de esta carpeta
para que podamos ver los archivos en su interior. Sólo tengo que hacer clic derecho,
7-Zip, Extract Here (Extraer aquí). Parece que hay bastantes archivos
dentro de esta carpeta. Además de desarchivar archivos,
también puedes archivar carpetas. Voy a crear una nueva carpeta
llamada new_colors. Después, agregaré este nuevo archivo
blue.txt los viejos archivos con nombre de colores en esta carpeta. Luego voy a archivarlo
con 7-Zip y Add to Archive (Agregar a la carpeta). Hago clic en OK (Aceptar). Genial, ¿no? Ahora, si quisieras enviarle a alguien
un montón de archivos en un correo electrónico, no tienes que enviarlos uno por uno. En su lugar, puedes combinarlos todos
en un solo archivo y enviarlo. Si estás usando la versión 5.0 de PowerShell
o una versión más avanzada, en realidad puedes extraer y comprimir archivos
desde la línea de comando. Digamos que tienes un montón de archivos en una
carpeta llamada "CoolFiles" en tu escritorio, y te gustaría agregarla
a un nuevo archivo zip. Después de que hayas abierto
la interfaz de línea de comandos de PowerShell, puedes ejecutar este comando,
Compress-Archive -path CoolFiles, y luego vamos a crear un nuevo archivo en el escritorio
llamado CoolArchive.zip. Ahora, si revisamos nuestro escritorio, podrás verlo allí, CoolArchive.zip. Esto tomará todo lo del directorio CoolFiles
del escritorio y lo comprimirá en el archivo CoolArchives.zip