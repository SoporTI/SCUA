Así como podemos anotar
los eventos de nuestra vida en un diario, los eventos también se registran en nuestras máquinas. En Windows,
los eventos registrados por el sistema operativo se guardan en una aplicación
llamada Visor de eventos. Si estás tratando de averiguar
por qué un juego de computadora sigue fallando, o de solucionar de problemas de acceso,
o solo buscas satisfacer tu curiosidad sobre lo que ocurre en tu sistema,
el Visor de eventos es una gran punto de referencia. Veamos algo
de la información que recopila y cómo puedes usar el Visor de eventos
para obtener las respuestas que estás buscando. Puedes iniciar el Visor de eventos
desde el menú Inicio o escribiendo eventvwr.msc
en el cuadro Ejecutar. La vista predeterminada del Visor de eventos
nos muestra un resumen de eventos recientes potencialmente importantes. En nuestro caso, esto no nos interesa mucho, ya que nos preocupa más
cualquier problema que haya ocurrido. En su lugar,
vamos a mirar el panel izquierdo, donde podemos ver
algunos grupos diferentes de eventos. El primer grupo que vemos
se llama Custom Views (Vistas personalizadas). El Visor de eventos registra mucha información
sobre el sistema. A veces, puede ser un poco difícil
separar la señal, como los eventos recientes,
del ruido o las cosas que no te importan. Aquí es donde el concepto de vistas personalizadas
es muy útil. Con una vista personalizada,
puedes crear un filtro que examinará todos los registros de eventos
que el Visor de eventos conoce y aislará solo la información
que te interesa. Supongamos que solo queríamos ver
eventos de error, de gravedad o superiores, que se registraron en la última hora. Para ello, haz clic en Create custom view (Crear vista personalizada)
en el panel Actions (Acciones) de la derecha. Esto abrirá una pestaña llamada Filter (Filtro). Desde allí, haz clic en las casillas de verificación
Error y Critical (Crítico). Vamos a cambiar el menú desplegable Logged (Registrado)
a Last hour (Última hora). En Event logs (Registros de eventos),
vamos a seleccionar solo los registros de Windows, a continuación, hacemos clic en OK (Aceptar). Vamos a darle a nuestra vista
un nuevo nombre. Hacemos clic en OK (Aceptar) una vez más. Cuando todo esté listo, verás que aparece una nueva vista
en los menús personalizados, en la que solo se muestran
los eventos que coincidieron con tus filtros. Las otras dos categorías de registros que verás
en la página de navegación de la izquierda son Windows Logs (Registros de Windows)
y Application and Services (Registros de aplicación y servicios). Las categorías de los registros de Windows
contienen registros de eventos que, en general, se aplican a todo el sistema operativo. Supongamos que tienes un problema
con un controlador que falla durante el inicio. El registro llamado System (Sistema)
sería un buen lugar para comenzar. Si quieres ver
quiénes accedieron a la computadora, entonces empieza a investigar
por el registro Security (Seguridad). La otra categoría se llama
Registros de aplicaciones y servicios. Esta categoría contiene registros
que rastrean eventos de una sola aplicación o componente del sistema operativo, en lugar de los eventos a nivel de sistema
de la categoría de registros de Windows. Por ejemplo,
si estás teniendo problemas con PowerShell y querías obtener más información al respecto,
revisar el registro de PowerShell la sección Aplicaciones y servicios
sería un gran primer paso. Más allá de su categoría, cada línea en un registro dado
en el Visor de eventos representa un evento. Cada evento contiene información
agrupada en columnas sobre el evento, como el nivel de acceso. "Información" es el nivel más bajo
y "Crítico" es el más alto. También puedes encontrar la fecha y hora
en que ocurrió el evento. Seleccionar un evento sacará a relucir
más información detallada en el panel inferior del Visor de eventos. Esto puede ayudarte a profundizar en la solución de problemas
o darte contexto para un informe de errores. El Visor de Eventos es una herramienta utilísima
para especialistas en soporte informático. Puede ofrecerte una gran cantidad
de información muy detallada sobre los problemas que cualquier software o hardware
podría estar experimentando en tu sistema. Hay mucha información allí,
sin embargo. No olvides sus vistas personalizadas
y sus funcionalidades de filtrado. Más importante aún,
no dudes en curiosear la herramienta y acostúmbrate a encontrar
cosas en su interfaz. Te divertirás y aprenderás mucho. Siguiente parada,
el salvaje mundo de los registros de Linux.