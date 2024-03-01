Para comenzar a interactuar con el disco, necesitamos montar el sistema de archivos
en el directorio. Podrías preguntarte
por qué no podemos hacer cd en /dev/sdb. Ese es el dispositivo de disco, ¿no? Lo es,
pero si intentamos hacer cd en /dev/sdb, así. obtenemos un error que dice
que el dispositivo no es un directorio, lo que es cierto. Para resolver esto,
necesitamos crear un directorio en nuestra computadora y luego montar el sistema de archivos
de nuestra unidad USB a este directorio. Detengámonos en la ubicación de nuestra partición
con sudo parted -l. Muy bien, puedo ver que la partición
a la que queremos acceder es /dev/sdb1. Ya creé un directorio
bajo el directorio raíz llamado my_usb. Vamos a intentarlo. Entonces: sudo mount /dev/sdb1 /my_usb/. Ahora, si vamos a my_usb,
podemos empezar a leer y escribir en el nuevo sistema de archivos. En realidad, no necesitamos montar explícitamente
un sistema de archivos con el comando mount. La mayoría de los sistemas operativos
hacen esto por nosotros automáticamente cuando conectamos un dispositivo, como una unidad USB. Los sistemas de archivos tienen que estar montados de una manera o de otra, porque tenemos que indicarle al SO
cómo interactuar con el dispositivo. También podemos desmontar el sistema de archivos
de manera similar usando el comando umount. Desmontar es lo contrario
de montar un disco. Así que ahora vamos a desmontar el sistema de archivos. Puedo usar sudo umount /my_usb, o sudo umount /dev/sdb1. Ambas servirán para desmontar un sistema de archivos. Cuando apagas tu computadora, los discos que se montaron manualmente
se desmontan automáticamente. En algunos casos,
como si estuviéramos usando una unidad USB, solo queremos desmontar el sistema de archivos
para la unidad USB sin apagar. Siempre asegúrate de desmontar un sistema de archivos
de una unidad antes de desconectarla físicamente. En el caso de una unidad USB, podemos encontrarnos con algunos errores interesantes
del sistema de archivos si no lo hacemos. Hablaremos más sobre esto
en la próxima lección. Además, ten en cuenta que cuando usamos el comando mount
para montar un sistema de archivos en un directorio, una vez que apagamos la computadora,
el punto de montaje desaparece. Sin embargo, podemos montar
permanentemente un disco si necesitáramos cargarlo automáticamente
cuando la computadora se inicia. Para ello, tenemos que modificar
un archivo llamado /etc/fstab. Si lo abrimos ahora, verás una lista de ID
de dispositivos únicos, sus puntos de montaje, qué tipo de sistema de archivos son,
más un poco de información adicional. Si queremos montar automáticamente
sistemas de archivos cuando la computadora se inicia, solo hay que agregar una entrada similar
a lo que se lista aquí. Vamos a seguir adelante y hacerlo muy rápido. El primer campo que necesitamos agregar
en /etc/fstab es el UUID o ID universal único de nuestra unidad USB. Para obtener el UUID de nuestros dispositivos,
podemos usar este comando: sudo blkid. Nos mostrará el UUID para los ID de dispositivo de bloqueo ID,
conocidos también como ID de dispositivo de almacenamiento. Y eso es todo. Vimos muchas tareas básicas
de administración de discos. Hasta ahora, particionamos un disco, le incorporamos
un sistema de archivos y lo montamos para su uso. Si tienes curiosidad y quieres conocer más
sobre el archivo /etc/fstab y sus opciones, puedes consultar
la siguiente lectura complementaria. De lo contrario, sigamos adelante