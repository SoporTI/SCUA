En una lección anterior, hablamos sobre el peligro
de desconectar un dispositivo USB sin expulsarlo o desmontarlo
de la computadora. Tal vez hayas visto
esta clase de mensajes de error cuando el sistema te avisa
que debes expulsar con seguridad esta memoria flash. ¿Por qué tenemos que hacer esto? Cuando copiamos archivos a una memoria flash
y vemos que el archivo se copió correctamente, ¿por qué no podemos simplemente desconectar
la unidad sin desmontarla o sin tocar el botón de expulsión en el SO? Resulta que es posible que los datos
no se hayan terminado de copiar. No es que nos grite por diversión. Cuando leemos o escribimos algo en una unidad,
en realidad primero ponemos eso en un búfer o memoria caché. Un búfer de datos es una región de la RAM
que se usa para almacenar datos temporalmente mientras se los está desplazando. Entonces, cuando copias algo de tu SO
a tu unidad USB, primero se copia en un búfer de datos
porque la RAM trabaja más rápido que los discos duros. Si no desmontas correctamente un sistema de archivos
y no le das tiempo suficiente a tu búfer para que termine de mover los datos,
corres el riesgo de corrupción de datos. La corrupción de datos
podría suceder por muchas razones, aparte de la eliminación insegura de una unidad de disco. Supongamos que estás trabajando en tu computadora
y se cortó la corriente en el edificio, lo que hace que tu computadora
se apague de repente. Este tipo de bloqueo
también provoca corrupción de datos. Las fallas del sistema o los errores de software
también puede provocar corrupción de datos. El sistema de archivos NTFS
tiene algunas características avanzadas integradas que pueden ayudar a minimizar
el peligro de corrupción además de intentar una recuperación
cuando el sistema de archivos se daña. Una de estas características,
a través de un proceso llamado registro en diario, registra los cambios realizados en los metadatos de un archivo
en un archivo llamado "registro NTFS". Al registrar estos cambios,
NTFS crea un historial de las medidas tomadas. Esto significa que puede mirar el registro
para ver cuál debería ser el estado actual del sistema. Si un bloqueo o un error provocan la corrupción,
el sistema de archivos puede iniciar el proceso de recuperación que usará ese registro
para asegurarse de que el sistema está en un estado coherente. Además del registro en diario, NTFS y Windows implementan algo
llamado recuperación automática. Como puedes suponer por el nombre,
el mecanismo de recuperación automática hace modificaciones en problemas menores y corrupciones
en el disco automáticamente, en segundo plano. Hace esto mientras Windows se está ejecutando,
por lo que no es necesario reiniciar. Si deseas comprobar el estado del proceso
de recuperación automática en tu computadora, puedes abrir un símbolo de sistema como administrador
y usar la herramienta fsutil, así. Fsutil repair query,
y quiero consultar mi disco C. Por último, cuando las cosas se ponen muy mal y hay una corrupción seria o catastrófica del disco,
como sectores defectuosos, fallas de disco y más,
puedes recurrir a la utilidad chkdsk de NTFS. Gracias a las características de recuperación
incorporadas en NTFS no siempre es necesario ejecutar chkdsk. Pero está disponible en caso de emergencia. Para ejecutar chkdsk manualmente,
puedes abrir un símbolo de sistema como administrador y escribir chkdsk en la línea de comandos. De forma predeterminada,
chkdsk se ejecutará en modo de solo lectura. Te daré un informe
sobre la salud del disco, pero no hará modificaciones
o reparaciones en él. Puedes indicarle a chkdsk que repare
cualquier problema que encuentre con el indicador /F. También puedes especificar
la unidad que quieres verificar, así: chkdsk /F. Voy a revisar mi unidad portátil,
que está en D. Sin embargo, no tendrás que ejecutar chkdsk
manualmente muchas veces. Si el sistema operativo detecta
que algunos datos se corrompieron o que el disco tiene un sector con fallas, configurará un bit en un archivo de metadatos en el volumen
que indica que hay corrupción. Cuando el sistema se inicie,
la utilidad chkdsk comprobará este bit. Si está configurado, se ejecutará
y tratará de reparar la corrupción reconstruyendo los bits dañados del sistema de archivos
desde el registro NTFS. Como puedes ver, el sistema de archivos NTFS de Windows
tiene implementadas medidas y funciones bastante sólidas para recuperar tus particiones
y evitar que la corrupción las dañe. A continuación, veamos cómo puedes realizar reparaciones
en el sistema de archivos en Linux.