> [!TIP]  
> [Ver video](https://youtu.be/zk24bQ3yeb4)

En Linux, los procesos tienen
una relación principal/secundario. Esto significa que cada proceso que inicias
viene de otro proceso. Veamos este comando. El comando less sería el proceso principal
de nuestro proceso grep. Si todos los procesos provienen
de otro proceso, debe haber un proceso inicial
que comenzó todo esto, ¿verdad? Sí lo hay.
Cuando enciendes tu computadora, el kernel crea un proceso llamado init,
que tiene PID igual a 1. Init pone en marcha otros procesos que necesitamos
para que nuestra computadora funcione. Hay muchos más matices en la creación de procesos,
pero quería presentar el concepto de proceso principal,
ya que lo verás cuando empecemos a gestionar procesos. ¿Y qué ocurre cuando
hemos terminado con nuestros procesos? Cuando tus procesos completan su tarea,
en general, finalizarán automáticamente. Una vez que un proceso finaliza,
devolverá todos los recursos que estaba usando al kernel,
para que puedan ser utilizados para otro proceso. También puedes finalizar un proceso manualmente. Vamos a analizar cómo hacerlo
en una próxima lección.