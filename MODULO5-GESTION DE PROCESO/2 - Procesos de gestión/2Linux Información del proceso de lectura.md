> [!TIP]  
> [Ver video](https://youtu.be/K4cGRhflMBM)

Muy bien, ahora hablemos sobre cómo ver los procesos
que se ejecutan en nuestro sistema en Linux. Usaremos el comando ps.
Sigamos adelante, ejecutémoslo con el indicador -x
y veamos qué ocurre. Esto te muestra una instantánea de los procesos
actualmente en ejecución en tu sistema. Al principio, la salida de ps
puede resultar abrumadora, pero no te preocupes,
te enseñaremos a leerla. Vamos a empezar de derecha a izquierda, aquí. P-I-D o PID es el ID del proceso. Recuerda que los procesos
obtienen un ID exclusivo cuando se inician. TTY, este es el terminal
asociado al proceso. No hablaremos de este campo, pero puedes leer más sobre esto en las man pages vinculadas
justo después de este video. STAT, este es el estado del proceso. Si ves una R aquí significa que el proceso
está en ejecución o esperando para ejecutarse. Otro estado común que verás es T, para "detenido", lo que significa que un proceso
fue suspendido. Otro que podrías ver es una S,
para "sueño interrumpible", es decir, la tarea está esperando
que se complete un evento antes de reanudarse. Puedes leer más sobre los otros tipos
de estados de proceso en las man pages. TIME: este es el tiempo total de CPU
que duró el proceso. Y por último, COMMAND: este es el nombre del comando
que estamos ejecutando. Bien, ahora vamos a ingresar
al modo difícil. Ejecuta este comando, ps -ef. El indicador "e" se utiliza para obtener todos los procesos,
incluso los ejecutados por otros usuarios. El indicador -f significa "full"
y te muestra todos los detalles sobre un proceso. Mira eso, tenemos más procesos
y aún más detalles de procesos. Vamos a analizarlo. UID es el ID de usuario de la persona
que inició el proceso. PID es el ID de proceso
y PPID es el ID del proceso principal que analizamos en la lección anterior,
cuando iniciamos el proceso. C es el número de procesos secundarios
que tiene este proceso. STIME es la hora de inicio del proceso. TTY es el terminal asociado
al proceso. TIME es el tiempo total de CPU
que duró el proceso. y CMD o "command" es el nombre del comando
que estamos ejecutando. ¿Y si quisiéramos buscar algo
a través de esta salida? Está muy desordenada en este momento. ¿Se te ocurre una manera en que podamos ver
si un proceso se está ejecutando? Correcto, con el comando grep.
Te dije que lo íbamos a usar todo el tiempo. Esto nos dará una lista de procesos
que tienen el nombre Chrome en ellos. Hay otra manera de ver
información del proceso, recuerda que, en Linux, todo tiene un archivo,
incluso los procesos. Para ver los archivos que corresponden a los procesos
podemos mirar en el directorio /proc. Hay muchos directorios aquí
para cada proceso en ejecución. Si miraras dentro de uno de los subdirectorios,
te dará mucha más información acerca del proceso. Veamos un archivo de proceso de muestra
para PID 1805. Esto nos dice mucha más información
sobre estados de proceso que lo que vimos en PS. Si bien es interesante
mirar el directorio /proc, no es muy práctico cuando necesitamos
solucionar problemas con los procesos. Por ahora, quedémonos con el comando ps -ef
para ver la información del proceso. Como ves, podemos aprender mucho
sobre los procesos que se ejecutan en nuestra máquina con solo teclear un poco. En una próxima lección, hablaremos sobre cómo usar
la información del proceso para nuestro beneficio cuando tenemos que averiguar qué procesos
están ocupando demasiados recursos. Por ahora, siéntete libre de aprender un poco más
sobre los procesos que estás ejecutando. Te estaré esperando en el siguiente video.