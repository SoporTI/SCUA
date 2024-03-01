Tal vez te diste cuenta de que, cuando estuvimos
mirando los permisos en la GUI antes, hay una casilla de verificación en la lista de permisos
para permisos especiales. Los permisos que estuvimos mirando
y estableciendo hasta aquí se llaman permisos simples. Los permisos simples son, en realidad,
conjuntos de permisos especiales o específicos. Por ejemplo,
cuando estableces el permiso de lectura en un archivo, en realidad estás estableciendo
múltiples permisos especiales. Veamos la lista
de permisos especiales disponibles. Voy a hacer clic en la pestaña Advanced (Opciones avanzadas)
debajo de mi configuración de permisos. Cuando hago clic en un nombre de usuario
y luego voy a los permisos avanzados, puedo ver una lista de todos los permisos especiales
habilitados en ese archivo. Cuando seleccionamos un permiso básico,
como el de lectura, en realidad estamos habilitando los permisos especiales
List folder / read data (Mostrar carpeta/leer datos), Read attributes (Leer atributos), Read extended attributes (Leer atributos
extendidos), Read permissions (Leer permisos) y Synchronize (Sincronizar),
que son solo permisos optimizados. Puedes modificar estos permisos como lo harías
con cualquier otro permiso básico. Siéntete libre de leer más
sobre los diferentes tipos de permisos especiales en las lecturas suplementarias
que incluí después de este video. En la mayoría de los casos,
los permisos simples serán todo lo que necesites. Pero a veces,
necesitas crear un archivo o una carpeta
que no sigue un patrón simple. Veamos un ejemplo
en esta CLI. Para ver los permisos especiales
de un archivo en la CLI, tan solo usaremos
el comando ICACLs como antes. Veamos un ejemplo más interesante
que mi carpeta Escritorio: icacls C:/windows/Temp. Este directorio se usa para conservar archivos temporales
para todos los usuarios del sistema. Nos gustaría que todos en el sistema
puedan crear archivos y carpetas aquí. Tal vez pienses que deberíamos usar
modificar o control total para esto, pero no queremos que los usuarios
puedan eliminar los archivos de los demás. Vamos a ver algunos de los DACL
asignados a esta carpeta y a entender cómo hacer esto. En primer lugar, las cuentas de administradores locales
y de sistemas operativos de la computadora tienen permisos completos sobre esta carpeta
y todos los archivos y carpetas dentro de ella. Vemos un nuevo descriptor, IO, que
indica que esta DACL es "solo heredar". Eso significa que será heredada, pero que no se aplica a este contenedor
C:\Windows\Temp. El grupo de usuarios incluye todas las cuentas de usuarios
en la máquina local. Vamos a permitir a los usuarios WD,
o "crear archivos/escribir datos", AD, o "crear carpetas y anexar datos"
y S para "sincronizar". Puedes ver en la próxima lectura suplementaria
que estos permisos especiales se incluyen
en el permiso simple modificado. A diferencia de la modificación de un permiso simple, no estamos otorgando a los usuarios
la capacidad para borrar archivos o carpetas. Sin embargo, queremos que los usuarios puedan eliminar
sus propios archivos y carpetas. ¿Cómo podemos hacer eso? Si ves "creator owner" (propietario creador)
es un usuario especial que representa al propietario de cualquier archivo
al que se aplique la DACL. En este directorio, y en todos los subdirectorios,
quien sea propietario de un archivo o carpeta tiene el control total de ellos. Bien, voy a crear una carpeta y un archivo en C:\Windows\Temp y ver qué DACL se les aplican. Usemos lo que aprendimos
sobre redireccionamiento de salida para registrar la salida de ICACLs
en este archivo. Entonces: icacls, ejemplo para C:\Windows\Temp\example. Luego vamos a utilizar nuestro operador de redireccionamiento
de salida para que nos dé icacls.txt. Bien, ahora veamos el archivo
que creamos para ver la salida de ICACLs. Genial, creé los archivos,
así que tengo el control total de ellos. Y todas las demás DACL que vimos
en C: \Windows\Temp se heredaron. Puedes ver que usar los especiales.
permisos en las DACL de NTFS puede ser complicado, pero también puede permitirte
crear conjuntos de permisos realmente poderosos y personalizados de acuerdo con tus necesidades exactas.