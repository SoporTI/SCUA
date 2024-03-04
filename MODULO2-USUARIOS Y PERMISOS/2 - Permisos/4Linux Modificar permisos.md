> [!TIP]  
> [Ver video](https://youtu.be/TtLEUFjyJ2M)

En Linux, cambiamos los permisos usando el comando chmod,
o "cambio de modo". Primero, elige el conjunto de permisos
que quieres cambiar. El propietario, marcado por una "u",
el grupo al que pertenece el archivo, marcado por una "g",
o los demás usuarios, marcado por una "o". Para agregar o eliminar permisos,
solo usa los símbolos + o - que indican
a quién afecta el permiso. Veamos algunos ejemplos Entonces: chmod u+x my_cool_file. Este comando indica
que queremos cambiar el permiso de my_cool_file otorgándole acceso ejecutable ("x")
al propietario ("u"). Puedes hacer lo mismo
si quisieras eliminar un permiso. Entonces: chmod u-x my_cool_file. En lugar de +, ponemos - Bastante fácil, ¿verdad? Si quisieras agregar múltiples permisos
a un archivo, podrías hacer algo como esto. Esto indica que queremos agregar
permisos de lectura y escritura para el propietario de my_cool_file. Y puedes hacer lo mismo
para múltiples conjuntos de permisos. Haces: chmod ugo+r my_cool_file. Ahora, esto dice que queremos agregar
permisos de lectura para nuestro propietario, para el grupo al que pertenece el archivo
y para todos los demás usuarios y grupos. Este formato de uso de rwx y ugo
para indicar permisos y usuarios en chmod
se conoce como formato simbólico. También podemos cambiar los permisos numéricamente,
lo que es mucho más rápido y más simple, y nos permite cambiar
todos los permisos a la vez. El equivalente numérico de rwx es
4 para lectura o "r", 2 para escritura o "w" y 1 para ejecución o "x". Para establecer permisos,
agregamos estos números a cada conjunto de permisos que queremos afectar. Veamos un ejemplo. El primer número 7,
es el permiso de nuestro propietario. El segundo número, 5, corresponde a los permisos
de nuestro grupo, y el tercer número, 4, es el permiso para todos los demás usuarios. Espera un minuto,
¿de dónde salieron 5 y 7? Recuerda, tienes que agregar
los permisos juntos. Si sumas 4, 2 y 1, obtienes rwx,
que es igual a 7. Así que nuestro permiso de propietario puede leer,
escribir y ejecutar este archivo. ¿Puedes adivinar qué significaría 5? Correcto. 4 + 1 = lectura y ejecución. Ahora, puedes ver cómo el formato numérico
es más rápido que el formato simbólico. En lugar de ejecutar algo como esto, podemos ejecutar chmod 754 my_cool_file
para actualizarlos a todos. De cualquier manera, puedes modificar los permisos
usando el formato simbólico o el numérico. Solo elige lo que te resulte más fácil. También puedes modificar el propietario
y el grupo de un archivo. El comando chown o "modificar propietario"
te permite cambiar el propietario de un archivo. Sigamos adelante
y cambiemos el propietario a Devan. Increíble. Y Devan es el propietario de este archivo. Para cambiar el grupo al que el archivo pertenece,
puedes usar el comando chgrp o "modificar grupo". Increíble. Ahora, best_group_ever
es el propietario del grupo para este archivo. Te puede llevar un tiempo dominar
la lectura y modificación de permisos. Puedes practicar cambiando los permisos en algunos archivos
hasta que lo logres. Los permisos son un fundamento esencial
de la seguridad informática y los usarás durante tu carrera
como especialista en soporte de TI.