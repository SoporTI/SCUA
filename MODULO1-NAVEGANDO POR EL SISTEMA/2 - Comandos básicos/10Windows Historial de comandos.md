> [!TIP]  
> [Ver video](https://youtu.be/gJu6rDOTKh8)

Retomando donde quedamos en el último video,
digamos que queremos crear un par de directorios,
`my_cool_folder2` y `my_cool_folder3`. Podríamos escribir
`mkdir my_cool_folder2` y luego volver a escribir `mkdir my_cool_folder3`, pero en lugar de eso, vamos a usar
otra función genial de PowerShell llamada "history" (historial).

Cada vez que ingresas un comando,
se guarda en la memoria y se agrega a un archivo especial. Puedes revisar los comandos que usaste anteriormente
con el comando `history`. Ahora estoy mostrando una lista de comandos
que ingresé anteriormente.

Esta información por sí sola no es muy útil. En cambio, hay un uso mejor de `history` que,
rápidamente, nos permite desplazarnos por estos comandos
y volver a usarlos. Podemos desplazarnos a través de estos comandos
con las teclas arriba o abajo de nuestro teclado.

Voy a subir por la lista de comandos utilizados y debería ver que ya tengo
`mkdir my_cool_folder`. En lugar de escribir todo esto
para crear una nueva carpeta, solo voy a agregar
el número 2 a mi comando. ¡Boom! Se crea un nuevo archivo
sin tener que escribir todo de nuevo. Genial, ¿verdad?

Incluso puedes buscar a través la lista de comandos
utilizados anteriormente con el atajo Ctrl-R de `history`. Desde aquí puedes empezar a escribir fragmentos del comando que quieres buscar
y te mostrará coincidencias. Busquemos la palabra "folder". Debería ver los comandos `mkdir`
que estuve usando antes. Muy ingenioso.

Si estás usando
una versión anterior de PowerShell, tal vez no tenga la función Ctrl-R. En tal caso, puedes escribir el símbolo #
seguido por alguna parte de tu antiguo comando, y luego usar tab completion
para ir pasando los elementos del historial.

La función `history`,
junto con tab completion y get-help, serán tus mejores amigos
mientras trabajes en PowerShell. Mantenlos cerca
y conócelos muy bien.

Hm... Nuestra shell se ve
un poco desordenada. Es un poco difícil ver dónde estoy,
así que vamos a limpiarla un poco. Podemos hacer eso con el comando `clear`. Esto no borra tu historial,
tan solo borra la salida en tu pantalla. Se ve un poco mejor.
