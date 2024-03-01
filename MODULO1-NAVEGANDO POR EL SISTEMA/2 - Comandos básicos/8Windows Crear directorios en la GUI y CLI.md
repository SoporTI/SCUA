Ahora que ya vimos cómo listar directorios y cambiar de directorio, vamos a aprender a agregar nuevos directorios. Podemos hacer esto en la GUI de una manera muy simple. Clic derecho, New (Nuevo), luego Folder (Carpeta), y ¡boom!, tenemos una nueva carpeta.

Ahora, ¿y si quisiéramos hacer esto en la CLI? En PowerShell, el comando para crear un nuevo directorio se llama `mkdir` o "crear directorio". Vamos a crear un nuevo directorio llamado `my_cool_folder` y ahí está. Eso fue fácil.

¿Y si quisiéramos usar espacios en el nombre de nuestra carpeta en lugar de guiones bajos? ¿Qué crees que pasaría si yo hiciera esto? `Mkdir my cool folder`. Eso es un error. `Mkdir` está intentando interpretar "cool" y "folder" como otros parámetros del comando `mkdir`. No entiende esas palabras como parámetros válidos.

Resulta que nuestra shell no interpreta los espacios como lo hacemos nosotros. Por lo tanto, debemos decirle explícitamente que el nombre de esta carpeta es una sola cosa. Podemos hacer esto de varias maneras. Podemos rodear el nombre con comillas, como: `mkdir 'my cool folder'`, o podemos marcar el espacio con un escape usando el acento grave: `mkdir my` cool` folder`.

El concepto de caracteres de escape es bastante común cuando manejamos código. Significa que el siguiente carácter después del acento grave debe tratarse literalmente. En nuestro ejemplo, al marcar el espacio con un escape, el shell comprende que el espacio después del acento grave es parte de nuestro nombre de archivo. Mientras que el acento grave es el carácter de escape en PowerShell, otros lenguajes de programación y shells pueden usar otro tipo de carácter de escape. Verás esto en el siguiente video.
