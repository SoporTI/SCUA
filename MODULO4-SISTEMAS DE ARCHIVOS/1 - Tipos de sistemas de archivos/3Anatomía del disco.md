Antes de que incorporemos un sistema de archivos a un disco,
vamos a hacer un resumen de los componentes del disco que te permiten almacenar
y recuperar archivos. Un disco de almacenamiento se puede dividir
en algo llamado particiones. Una partición es sólo una parte del disco
que puedes administrar. Cuando creas múltiples particiones,
te da la ilusión de estar dividiendo físicamente un disco
en discos separados. Para incorporar un sistema de archivos a un disco,
primero necesitas crear una partición. Por lo general, solo tenemos una sola partición
para nuestro sistema operativo, pero no es raro tener múltiples particiones
para diferentes usos. Supongamos que quieres tener
dos particiones en un disco, una para un SO Windows y otra para un SO Linux. En lugar de usar dos máquinas
para ambos sistemas operativos, solo puedes usar una máquina
y cambiar de SO en el inicio. También puedes incorporar diferentes sistemas de archivos
en diferentes particiones del mismo disco. Las particiones funcionan básicamente
como sus propios sub discos separados, pero todas usan el mismo disco físico. Algo para señalar es que cuando formateas un sistema de archivos
en una partición, se convierte en un volumen. A veces, volumen y partición
se usan erróneamente como sinónimos, pero queremos asegurarnos
de que entiendas esta distinción. El otro componente de un disco
es una tabla de particiones. Una tabla de particiones le indica al SO
cómo se particiona el disco. La tabla te indicará desde qué particiones
puedes dar inicio, cuánto espacio se asigna
a la partición, etc. Hay dos esquemas principales
de tablas de particiones en uso: MBR, o registro de arranque maestro,
y GPT, o tabla de particiones GUID. Estos esquemas deciden
cómo estructurar la información sobre particiones. MBR es una tabla de particiones tradicional,
y se usa principalmente en el SO Windows. MBR solo te permite tener volúmenes
de hasta 2 TB de tamaño. También usa algo llamado
particiones primarias. Solo puedes tener
cuatro particiones primarias en un disco. Si quieres agregar más,
tienes que tomar una partición primaria y convertirla en algo
que se conoce como partición extendida. Dentro de la partición extendida, puedes hacer algo llamado
partición lógica. Al principio cuesta entenderlo, pero es así como se creó
la tabla de particiones. MBR es un estándar antiguo
y lentamente va perdiendo terreno a manos del próximo esquema
de tabla de particiones del que hablaremos, GPT. GPT se está convirtiendo
en el nuevo estándar para discos. Puedes tener un volumen
cuyo tamaño supere los 2 TB y solo tiene un tipo de partición. Puedes hacer tantas particiones
como quieras en un disco. En una lección anterior,
conocimos un nuevo estándar de BIOS, llamado UEFI, que se convirtió en el BIOS predeterminado
para sistemas más nuevos. Para poder iniciar con UEFI,
tu disco tiene que usar la tabla de particiones GUID. Ahora que sabes lo que debes hacer
para realizar una partición, vamos a particionar un disco real. En las siguientes lecciones,
vamos a aprender a particionar y formatear una unidad USB para cada SO.