> [!TIP]  
> [Ver video](https://youtu.be/hR661bi-as4)

¿Alguna vez intentaste enviar
un archivo a un compañero de trabajo? ¿Qué métodos usas? ¿Lo adjuntas a un correo electrónico y lo envías,
o copias el archivo a una unidad USB y luego transfieres el archivo de esa manera? Hay muchas formas de transferir archivos. En esta lección, vamos a hablar de un método
que utiliza conexión remota. SCP, o copia segura, es un comando que puedes usar en Linux para copiar archivos
entre computadoras en una red. Utiliza SSH para transferir los datos. Al igual que harías SSH en una máquina,
puedes enviar un archivo de esa manera. Veámoslo en acción. Supongamos que quieres copiar un archivo
de nuestra computadora a otra computadora. Para ello, podemos ejecutar el comando SCP
con algunos indicadores. Entonces: scp, Desktop, myfile, a cindy@. En este comando, ejecutamos el comando scp
con la ruta del archivo que queremos transferir a la cuenta de usuario,
nombre de host y ruta desde donde queremos copiar el archivo. Ahora, nos solicita la información de acceso de la computadora
a la que queremos enviarle el archivo. Después de ingresar esto, podemos verificar
si el archivo se copió correctamente. Y ahí está. El comando scp es una herramienta súper útil
si necesitas copiar archivos hacia y desde las computadoras en una red. Puedes leer más sobre el comando
en la man page.