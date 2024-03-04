> [!TIP]  
> [Ver video](https://youtu.be/NT-4My292PA)

Para leer un archivo simple en bash, también podemos usar el comando cat que se usa para ver un documento. Vamos a ver el archivo important_document. El comando cat es similar al comando cat de Windows, ya que no hace un gran trabajo en la visualización de archivos de gran tamaño. En su lugar, usamos otro comando, less. Less hace algo similar a lo que hace more en Windows, pero tiene más funcionalidad.

Curiosidad: hay un comando de bash que se llama more, pero viene cayendo en desuso lentamente a raíz de less. Literalmente, es un caso de "menos es más". De manera similar a more, cuando usamos less pasamos a una shell interactiva.

Algunas de las teclas más comunes que usarás para navegar esta herramienta son las teclas arriba y abajo, y las teclas para retroceder y avanzar páginas.

- **g:** te lleva al principio de un archivo. Puedes ver ahora que estamos en el principio.
- **G mayúscula:** te lleva al final de un archivo de texto. Ahora estamos en el final.
- **Una barra y luego una búsqueda de palabra (/word_search):** te permite buscar una palabra o frase. Si escribo una barra y luego la palabra que quiero buscar, puedo examinar el archivo de texto en busca de palabras que coincidan con mi búsqueda.
- **q:** esto te permite salir de less y volver a tu shell, de modo similar a la tecla "q" en el comando more de Windows.

¿Ves como less ofrece funcionalidad como buscar dentro de un archivo? Less es una gran herramienta para ver archivos de cualquier tamaño. Sin duda terminarás usando este comando muy a menudo como especialista de soporte de TI.

Al igual que con cat en Windows y el parámetro -Head, podemos hacer lo mismo en Linux con un comando llamado head. Esto te mostrará, de manera predeterminada, las primeras diez líneas de un archivo.

¿Y si quisieras ver las últimas líneas de un archivo? Puedes usar un comando llamado tail. Esto te mostrará, de manera predeterminada, las últimas diez líneas de un archivo.
