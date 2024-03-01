En Linux, los metadatos y los archivos se organizan
en una estructura llamada inodo. Los inodos son similares
a los registros MFT del NFTS de Windows. Almacenamos inodos en una tabla de inodos y nos ayudan a gestionar los archivos
en nuestro sistema de archivos. El inodo en sí no almacena
la fecha del archivo ni su nombre, pero almacena todo lo demás
sobre un archivo. En la última lección, aprendimos a crear
accesos directos de archivos, vínculos simbólicos y vínculos físicos en Windows. Pues en Linux tenemos el mismo concepto. A los accesos directos en Linux
los llamamos softlinks o symlinks. Funcionan de manera similar
a los vínculos simbólicos en Windows en cuanto a que solo apuntan a otro archivo. Los softlinks nos permiten enlazar a otro archivo
mediante un nombre de archivo. Son geniales para crear accesos directos
a otros archivos. El otro tipo de enlace que encontramos en Linux
son los hardlinks. De manera similar a Windows,
los hardlinks no apuntan a un archivo. En Linux, enlazan a otro inodo almacenado
en una tabla de inodos en el sistema de archivos. Básicamente, cuando estás creando un hardlink,
estás apuntando a una ubicación física en el disco o, más específicamente,
en el sistema de archivos. Pero si borraste un archivo de un hardlink,
todos los demás hardlinks seguirían funcionando. Veamos dónde se hace referencia
a los hardlinks. Si hiciéramos ls -l en este archivo,
important_file, notarás que el tercer campo
en los detalles, este campo en realidad indica
la cantidad de hardlinks que tiene un archivo. Cuando el recuento de hardlinks de un archivo
llega a cero, entonces el archivo se eliminó por completo
de la computadora. Para crear un softlink, podemos ejecutar el comando ln
con el indicador -s para "softlink". Entonces: ln -s important_file
important_file_softlink. Para crear un hardlink, podemos ejecutar el comando ln sin la -s,
para especificar un hardlink. Entonces:
ln important_file important_file_softlink. Ahora, si comprobamos ls -l important_file, veremos que el recuento de hardlinks
aumentó en una unidad. Los hardlinks son geniales si necesitas guardar el mismo archivo
en diferentes lugares, pero no quieres ocupar
nada de espacio adicional en el volumen. Esto es porque todos los hardlinks
apuntan al mismo espacio en el volumen. Podrías usar softlinks
para hacer lo mismo. Pero ¿y si moviste un archivo,
deshiciste el softlink y olvidaste todos los demás lugares
donde lo usaste? Todos los demás softlinks también quedarían deshechos
y limpiar todo puede llevarte cierto tiempo. Tal vez no tenga sentido para ti
crear tus propios softlinks o hardlinks ahora mismo, pero se utilizan en todo tu sistema,
por lo que debes estar al tanto de cómo funcionan.