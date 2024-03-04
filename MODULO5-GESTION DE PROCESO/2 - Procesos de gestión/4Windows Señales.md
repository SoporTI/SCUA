> [!TIP]  
> [Ver video](https://youtu.be/P4uVPadSwrg)

Imagina que estás empezando un videojuego
que se toma su tiempo para procesar sus gráficos. Decides que no quieres jugar más, lo que te deja con algunas opciones. Puedes esperar a que termine de cargar
y luego salir del juego desde el menú o puedes interrumpir el proceso por completo,
diciéndole que anule a nivel del sistema. Este es solo un ejemplo de un momento en el que,
tal vez, te gustaría cerrar un proceso antes de que se complete al 100%. Para indicarle a un proceso que se anule a nivel del sistema,
usamos algo llamado señal. Una señal es una forma de decirle un proceso
que algo acaba de ocurrir. Puedes generar una señal
con caracteres especiales en tu teclado y a través de otros procesos y software. Una de las señales más comunes
con las que te encontrarás se llama SIGINT, que significa "interrupción de la señal". Puedes enviar esta señal a un proceso en ejecución
con la combinación de teclas Ctrl + C. Digamos que inicias la herramienta DiskPart
que vimos cuando analizamos el formateo de particiones. Solo voy a abrir el símbolo del sistema
y luego iniciar DiskPart. Si decides que, en verdad,
no quieres formatear ningún disco, puedes mantener presionada la tecla Ctrl y presiona C al mismo tiempo para enviar
la señal SIGINT al proceso DiskPart. Verás que se cierra la ventana
en donde DiskPart se ejecutaba y el proceso termina. Hay algunas otras señales de Windows
que los procesos pueden enviar y recibir. Pero, a diferencia de Linux,
no hay una manera fácil para que un usuario final emita
comandos de señales arbitrarias. Si te interesa aprender más
sobre las señales de Windows, consulta el vínculo de referencia sobre señales
en la lectura complementaria.