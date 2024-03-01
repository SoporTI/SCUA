Ahora que aprendimos los conceptos básicos de la navegación de archivos y directorios, vamos a aprender cómo podemos visualizar y editar archivos, buscar texto dentro de archivos y más.

En la GUI de Windows, si queremos abrir un archivo y ver su contenido, podemos hacer doble clic en el archivo. Dependiendo del tipo de archivo, se abrirá en una aplicación predeterminada. En Windows, los archivos de texto se abren en una aplicación llamada Bloc de notas. Pero podemos cambiar esto si queremos. Para cambiar la aplicación predeterminada que abre archivos, haz clic derecho y luego clic en Properties (Propiedades). En Open with (Abrir con), podemos cambiar la aplicación a otro editor de texto, como WordPad.

La mayoría de los archivos con los que trataremos a lo largo de este curso serán archivos de texto y de configuración. Entonces, enfoquémonos en esos archivos en lugar de archivos de imágenes, música, etc.

Para ver el contenido de un archivo en PowerShell, simplemente usas el comando cat, que significa concatenar. Hagamos un intento. Esto volcará el contenido del archivo en nuestra shell. No es la mejor solución para un archivo ya que sigue escribiendo el contenido hasta mostrar el archivo completo.

Si queremos ver el contenido del archivo de a una página, podemos usar el comando more, así. El comando more obtendrá el contenido del archivo, pero hará una pausa una vez que llene la ventana del terminal. Ahora, podemos avanzar el texto a nuestro propio ritmo.

Cuando ejecutamos el comando more, pasamos a un programa separado de la shell. Esto significa que interactuamos con el programa more con teclas diferentes. La tecla Intro avanza el archivo una línea. Puedes usar esto si quieres moverte lentamente a través del archivo. El espacio avanza el archivo una página. Una página en este caso depende del tamaño de la ventana de tu terminal. Básicamente, more entregará suficiente contenido para llenar la ventana del terminal. La tecla "q" te permite salir de more y volver a tu shell. Si queremos dejar el comando more y volver a nuestra shell, podemos tocar la tecla "q". Aquí vamos.

Ahora, ¿y si solo queremos ver parte del archivo? Supongamos que queremos ver rápidamente cuáles son las primeras líneas del archivo de texto. No queremos abrir todo el archivo. En cambio, solo queremos ver un esbozo del documento. A esto se lo llama el encabezado del archivo. Para hacer esto, podemos volver a cat y agregar el parámetro -Head. Esto nos mostrará las primeras 10 líneas del archivo.

Ahora bien, ¿y si quisiéramos ver las últimas líneas o el final del archivo? Apuesto a que puedes suponer lo que vamos a hacer. Esto nos mostrará, de forma predeterminada, las últimas diez líneas del archivo. Una vez más, estos dos comandos aún no parecen tener ningún uso inmediato para ti. Veremos sus beneficios cuando trabajemos con registros, en una próxima lección.

Ahora, veamos cómo hacer estas mismas tareas en Linux.
