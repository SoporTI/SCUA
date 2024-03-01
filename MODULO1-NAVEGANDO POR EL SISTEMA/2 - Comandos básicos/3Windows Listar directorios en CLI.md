Es importante saber que hay un par de interfaces de línea de comandos, o CLI, disponibles en Windows. La primera se llama símbolo del sistema o `command.exe`. La segunda es PowerShell o `powershell.exe`.

El símbolo del sistema existe desde hace mucho tiempo. Es muy similar al símbolo del sistema que se usaba en MS DOS. Como PowerShell admite casi todos los mismos comandos que el Símbolo del sistema y muchos, muchos más, vamos a usar PowerShell para los ejercicios en este módulo.

Quiero señalar que muchos de los comandos de PowerShell que usamos en realidad son alias para comandos comunes en otras shells. Un alias es algo así como un apodo para un comando.

El primer comando que usaremos es para listar archivos y directorios. Comencemos listando los directorios en la raíz de nuestra unidad C:. La unidad C: es donde está instalado el sistema operativo Windows.

Para acceder a la CLI de PowerShell, simplemente busca PowerShell en tu lista de aplicaciones. Desde aquí, podemos seguir adelante e iniciar el programa PowerShell.

Vamos a utilizar el comando `ls` o "listar directorios" y darle la ruta de acceso que queremos mirar. La ruta no es realmente parte del comando, pero es un parámetro de comando. Puedes pensar en los parámetros como un valor que está asociado con un comando.

Ahora puedes ver todos los directorios en la raíz de tu unidad C:. Es posible que solo veas unos pocos directorios o un montón de ellos. Todo depende del uso que se le dé a tu computadora.

La carpeta raíz de la unidad C: es lo que llamamos un directorio superior y los contenidos en el interior se consideran directorios secundarios. A medida que sigas trabajando con los sistemas operativos, encontrarás términos que, al principio, pueden parecer un poco extraños, pero en realidad tienen mucho sentido. Superior y secundario son términos comunes que representan relaciones jerárquicas en los SO.

Si tengo una carpeta llamada Dogs y una segunda carpeta anidada dentro de aquella, llamada Corgi, Dogs sería el directorio superior y Corgi, el directorio secundario.

Veamos algunos de los directorios secundarios comunes en esta carpeta.
- `Program Files (x86)` (Archivos de programa [x86]). Estos directorios contienen la mayor parte de las aplicaciones y otros programas que se instalan en Windows.
- `Users` (Usuarios). Esto contiene los directorios del perfil de usuario o directorios principales. Cada usuario que accede a esta máquina Windows obtendrá su propio directorio aquí.
- `Windows`. Aquí es donde está instalado el sistema operativo Windows.

Si abrimos un PowerShell y ejecutamos `Get-Help ls`, veremos el texto que describe los parámetros del comando `ls`. Esto nos dará un breve resumen de los parámetros de los comandos. Pero si quieres ver ayuda más detallada, prueba `Get-Help ls -Full`. Ahora puedes ver una descripción de cada uno de los parámetros y algunos ejemplos de cómo usar el comando.

¿Y si quisiéramos ver todos los archivos ocultos en este directorio? Bueno, podemos usar otro parámetro útil para el comando `ls`, `-Force`. El parámetro `-Force` mostrará archivos ocultos y del sistema que normalmente no se listan solo con `ls`. Ahora puedes ver algunos archivos y directorios importantes como `Recycle Bin` (Papelera de reciclaje). Aquí es donde reside la papelera de reciclaje. Cuando mueves archivos a la papelera de reciclaje, se mueven a este directorio en lugar de borrarse inmediatamente.
- `ProgramData`. Este directorio contiene muchas cosas diferentes. En general, se usa para almacenar datos de programas que están instalados en `Program Files` (Archivos de programa).

Muy bien, ahora que sabes cómo mirar el sistema de archivos en Windows, veamos este proceso en Linux.
