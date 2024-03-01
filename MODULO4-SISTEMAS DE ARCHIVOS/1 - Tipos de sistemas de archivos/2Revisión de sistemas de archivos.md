Tal vez recuerdes que presentamos
el concepto de un sistema de archivos en el curso Fundamentos de soporte técnico. Veamos un repaso. Un sistema de archivos sirve para rastrear archivos
y su almacenamiento en un disco. Sin un sistema de archivos, el sistema operativo
no sabría cómo organizar los archivos. Cuando tienes un disco nuevo
o cualquier tipo de dispositivo de almacenamiento, como una unidad USB,
necesitas agregarle un sistema de archivos. Hay muchos sistemas de archivos por ahí,
pero los dos de los que hablaremos en este curso se recomiendan como sistemas de archivos
predeterminados para Windows y Linux. Para Windows,
usamos el sistema de archivos NTFS; para Linux, se recomienda usar ext4. Los sistemas de archivos tienen
diferentes compatibilidades con distintos SO. La mayor parte del tiempo, el soporte inter-SO
es mínimo en el mejor de los casos. Supongamos que tienes una unidad USB
que está usando un sistema de archivos NTFS. Tanto Windows como Ubuntu (Linux)
pueden leer y escribir en la unidad USB. Pero si tienes una unidad USB ext4,
solo funcionará en Ubuntu y no en Windows, al menos sin ayuda
de herramientas externas. Es bastante probable que te encuentres en esta situación
en una función de soporte de TI. Supongamos que tienes algunos archivos importantes
en ese mismo USB que quieres copiar a tus SO Windows, Linux y Mac OS.
¿Qué harías entonces? Esta es una situación bastante común. Tendrías que reformatear
o limpiar la unidad USB y agregar un sistema de archivos
que sea compatible con los tres sistemas operativos. Por suerte, hay sistemas de archivos como FAT32
que admiten lectura y escritura de datos
en los tres sistemas operativos principales. FAT32 tiene algunas deficiencias, sin embargo. No admite archivos
cuyo tamaño supere los 4 GB y el tamaño del sistema de archivos
no puede superar los 32 GB. Esto podría ser suficiente para un pequeño USB,
pero no es muy bueno para nada más. Puedes ver más información sobre FAT32
en la lectura complementaria. Esto todavía plantea la pregunta:
¿y si quisieras poder compartir archivos entre múltiples sistemas operativos sin tener que lidiar
con las limitaciones del sistema de archivos? No te preocupes, cuenta con nosotros. En el próximo curso
sobre administración de sistemas y servicios de infraestructura de TI,
vamos a analizar otro tipo de sistema de archivos llamado sistemas de archivos de red
que resuelve exactamente este problema. Muy bien, ahora que tuviste un rápido repaso
sobre los sistemas de archivos, vamos a dedicar las siguientes lecciones
a analizar cómo configurarlos.