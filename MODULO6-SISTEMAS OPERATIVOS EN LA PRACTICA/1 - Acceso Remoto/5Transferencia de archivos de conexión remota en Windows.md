¿Cómo podemos compartir archivos y datos a través de la red
en una computadora con Windows? Da la casualidad de que el programa PuTTY
del que hablamos hace un par de lecciones
admite el protocolo SCP. El paquete PuTTY viene con una herramienta llamada
cliente de copia segura de PuTTy, o pscp.exe. Puedes usarla para copiar archivos de manera muy similar
al comando scp de Linux. Vamos a verlo. Pscp.exe, y voy a tomar
un archivo de mi escritorio, luego voy a copiarlo
a mi estación de trabajo Linux. Y luego voy a agregar la ubicación
desde donde quiero copiarlo. Ahora, si volvemos
a mi estación de trabajo Linux, Podemos ver que se copió. Usar PuTTY o scp para transferir archivos
puede llevar un poco de tiempo, en especial si necesitas transferir archivos
a varias máquinas. Como alternativa, Windows concibió
un mecanismo incorporado para compartir archivos mediante el concepto de carpetas compartidas. Las carpetas compartidas hacen más o menos
lo que su nombre sugiere. Le dices a Windows que quieres
compartir una carpeta con una persona o un grupo de personas;
luego, sueltas algunos archivos en ella. La persona con quien hayas compartido la carpeta
puede entonces acceder a esos archivos. Compartir carpetas en Windows es fácil. Tan solo haz clic derecho en la carpeta
que quieres compartir, luego pasa el mouse sobre la opción Share with (Compartir con),
luego selecciona Specific People (Personas específicas). Desde aquí,
puedes agregar los usuarios individuales o los grupos con los que quieres compartir la carpeta. Incluso hay una opción para agregar a todos
a los permisos de compartición, lo que podría ser conveniente,
pero no es muy seguro. Después de compartir la carpeta,
puedes acceder a ella desde otras computadoras. Comienza abriendo This PC (Este equipo),
luego ve a la pestaña Computer (Equipo). Desde aquí, puedes mapear la carpeta
directamente a tu computadora con la opción Map network drive (Conectar a unidad de red). Por último, en otra computadora, puedes ir directamente
a la carpeta desde el cuadro Ejecutar escribiendo un barra invertida,
el nombre de la computadora, otra barra invertida, el nombre de la carpeta asignada
como carpeta compartida. Quizás te interese saber que también
puedes compartir carpetas desde la línea de comandos, usando el comando net share. "net share" te permite hacer lo mismo
que el flujo de trabajo de intercambio de la GUI, y deberás especificar qué tipo de permisos
te gustaría otorgar a qué usuarios. Supongamos que querías otorgar a toda la gente en tu red
permisos completos a una carpeta llamada ShareMe. Podrías ejecutar este comando
desde una ventana de PowerShell de nivel superior o de administrador: net share ShareMe, C, Users, /grant:everyone,full. Los usuarios podrán acceder a la carpeta compartida
usando los mismos métodos de los que hablamos antes. El comando net share
también puede usarse para listar las actuales carpetas compartidas en tu computadora.
Para ello, debes ejecutarlo sin ningún argumento. Así. Si deseas más información
sobre net share y sus habilidades, consulta la documentación
en la lectura complementaria.