Muy bien, ahora que aprendimos
a listar, crear y mover archivos en directorios,
vamos a empezar a eliminarlos.

En la GUI de Windows,
si deseas eliminar un archivo o carpeta, haces clic derecho y Delete (Eliminar). El archivo termina en la papelera de reciclaje,
la que puedes encontrar en tu escritorio. Si deseas restaurar un archivo aquí,
podrías hacer clic derecho y Restore (Restaurar). Si vacías tu papelera por algún motivo,
no podrás recuperar esos archivos.

En PowerShell, el comando para eliminar
archivos y directorios es `rm`, o "eliminar". Ten cuidado al usar `rm`
porque no utiliza la papelera de reciclaje. Una vez que los archivos y directorios se eliminan,
se han ido para siempre.

Vamos a eliminar un archivo llamado `text1.txt`
en mi directorio principal. Vamos a ver... Ahí está. Voy a eliminarlo. Ya no está. El comando `rm` podría parecer un arma peligrosa
en las manos equivocadas. Por suerte, hay medidas de seguridad
implementadas que solo habilitan esta capacidad a los usuarios
que tienen autorización para usarla. Hablaremos más sobre los permisos de archivo
en una lección diferente. Pero veamos rápidamente
a qué me refiero.

Vamos a eliminar un archivo llamado
`important_system_file`. Recibo un mensaje de error que dice
que no tengo permiso para borrar este archivo. En ciertos casos, como este,
es porque está marcado como archivo del sistema. En otros casos,
podría ser porque no tengo permisos suficientes en el sistema de archivos para eliminarlo. Tengo los permisos correctos esta vez,
pero ya que es un archivo importante, PowerShell quiere asegurarse
de que quise hacer esto. Si repito el comando con el parámetro `-Force`,
`rm` seguirá adelante y eliminará el archivo. Vamos a verlo. `-Force`, Y puedes ver que el archivo ya no está.

Si el archivo pertenece a otra persona,
o si no soy administrador, entonces podría no tener los permisos correctos
para eliminar el archivo. En ese caso, necesitaré acceder a una cuenta administrativa
para eliminar el archivo.

Está bien, vamos a tratar de eliminar
un directorio con `rm` a continuación. Aquí vamos. Aquí hay otro lugar donde PowerShell
nos va a preguntar si realmente queremos hacer esto. Como esto está en un directorio,
contiene otros archivos. Y no usamos el parámetro `-Recurse`. Vemos un aviso que nos pide que confirmemos
si realmente queremos eliminar el directorio y todo su contenido. Podemos decir Yes (Sí) o Yes to All (Sí a todo) para continuar. También podemos cancelar este comando
y volver a ejecutarlo con el parámetro `-Recurse`. De esa manera, PowerShell sabe
que entendemos las consecuencias de lo que estamos haciendo. Sigamos adelante y cancelemos esto
y volvamos a intentarlo. `-Recurse`. Sí, ya no está. Y ese es el comando `rm`
en pocas palabras. Una vez más,
debido a la naturaleza de este comando, debes tener mucho cuidado
al eliminar archivos o directorios.
