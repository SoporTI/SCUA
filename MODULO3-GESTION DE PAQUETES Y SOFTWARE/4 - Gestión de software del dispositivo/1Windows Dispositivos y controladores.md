Una parte importante del software
de la que hemos hablado, pero que realmente no vimos en acción,
se conoce como controlador. Recuerda que un controlador se utiliza para ayudar
a que los dispositivos de hardware interactúen con nuestro sistema operativo. En esta lección, hablaremos de controladores
de dispositivos y cómo gestionarlos. En primer lugar, vamos a hablar de cómo gestionar
los dispositivos que nuestra computadora ve y luego vamos a repasar
cómo instalarles sus respectivos controladores. En Windows, Microsoft agrupa todos los dispositivos
y controladores de la computadora en una sola consola de gestión de Microsoft
llamada Administrador de dispositivos. Puedes acceder al Administrador de dispositivos
de maneras diferentes. Puede abrir el cuadro de diálogo Ejecutar
y escribir devmgmt.msc. O puedes hacer clic derecho en This PC (Este equipo),
seleccionar Manage (Administrar), y luego hacer clic en la opción Device Manager (Administrador de dispositivos)
en el menú de navegación de la izquierda. Voy a abrirlo desde aquí. La mayoría de los dispositivos que tienes en tu computadora
se agruparán según algunas categorías generales de Windows. Cualquier pantalla que puedas estar usando
en tu computadora va a aparecer en la sección Monitors (Monitores)
en el Administrador de dispositivos. De este modo. Esto suele agruparse automáticamente
cuando conectas un nuevo dispositivo. Es parte del sistema "plug and play" (PnP) que usa Windows para detectar automáticamente
nuevo hardware conectado a tu computadora. Luego reconoce e instala
el software adecuado para gestionarlo. Si te interesa aprender más, puedes leer más sobre el sistema PnP
en la lectura complementaria. Te daremos una visión general
de cómo funciona esto para que puedas comprenderlo. Cuando conectas un nuevo dispositivo,
como un mouse o teclado en tu computadora, el sistema operativo de Windows
sigue unos pasos para intentar que funcione. La mayoría de fabricantes o vendedores de hardware de computadora
le asignarán una string especial de caracteres a sus dispositivos
que se denomina una ID de hardware. Cuando Windows nota que se conectó un nuevo dispositivo,
lo primero que hará es preguntar al dispositivo
por su ID de hardware. Una vez que Windows tiene la ID de hardware del nuevo dispositivo,
el sistema operativo la utiliza para buscar el controlador correcto para dicho dispositivo. Lo busca en algunos lugares,
comenzando con una lista local de controladores reconocidos. Luego pasa a Windows Update o a la tienda de controladores
si es necesario ampliar la búsqueda. A veces, el dispositivo vendrá
con un disco de instalación que contiene un software de controlador personalizado,
y puedes indicarle a Windows que busque allí también. Finalmente, Windows tomará
el software del controlador que encontró y lo instalará para que puedas usar tu nuevo dispositivo. Aunque este proceso, en su mayoría,
sucede automáticamente y de manera imperceptible, puedes interactuar
directamente con los controladores de Windows a través de la consola para la administración de dispositivos
que mencionamos anteriormente. Puedes ampliar cualquiera de las categorías
en el administrador de dispositivos para ver los dispositivos que se encuentran dentro de ellas, de esta forma. También puedes usar el todopoderoso clic derecho de Windows
para abrir un menú con opciones que te permiten trabajar con ellas. Puedes desinstalar, deshabilitar y actualizar
un controlador de dispositivo desde este menú. También le puedes decir a Windows que busque cambios en el hardware,
como un dispositivo recién conectado. Por último, si eliges Properties (Propiedades)
desde el menú del botón derecho, podrás ver algunos detalles sobre
el dispositivo y su controlador. Como el fabricante y la versión
del controlador en uso. Si estás interesado en acceder
a los controladores a través de Windows CLI, consulta la siguiente lectura para
más información.