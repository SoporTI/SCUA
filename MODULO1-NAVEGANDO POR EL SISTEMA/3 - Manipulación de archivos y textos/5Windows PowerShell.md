Hasta ahora, en este curso hemos estado usando alias de comando en PowerShell. PowerShell es un lenguaje de comandos complejo, poderoso y muy sólido también. Pudimos usar alias comunes, que son exactamente los mismos que sus equivalentes de Linux.

Pero de aquí en adelante, tendremos que implementar algunas funciones avanzadas de línea de comandos, por lo que tendremos que mirar comandos reales de PowerShell. Ya viste un ejemplo de un verdadero comando de PowerShell, Get-Help, que se usa para ver más información sobre los comandos.

Hay otro comando de PowerShell que podemos usar para mirar uno de los alias que estuvimos usando, ls, o "listar directorio". Para ver cuál comando de PowerShell se ejecuta realmente, podemos usar el comando de PowerShell, Get-Alias.

Interesante, cuando invocamos ls, estamos invocando el comando Get-ChildItem de PowerShell, que obtiene o lista los elementos secundarios, que son los archivos y subdirectorios del elemento dado. Vamos a ejecutar este comando Get-ChildItem con el elemento C:\. Verás que es la misma salida que con ls C:\. Interesante.

Los comandos de PowerShell son muy largos y descriptivos, lo que los hace más fáciles de entender. Pero esto implica tener que escribir mucho más cuando estás trabajando interactivamente en el CLI. Los alias para los comandos comunes son una gran manera de trabajar más rápido en PowerShell. Los hemos estado usando hasta ahora para arrancar a toda marcha con la línea de comandos.

En Windows, más que nada tienes tres formas diferentes de ejecutar comandos. Puedes usar comandos reales de PowerShell o los nombres de alias relacionables. Otro método que mencionamos, pero del que todavía no hablamos, es el grupo de comandos cmd.exe. Los comandos cmd.exe son comandos de los viejos días de MS-DOS de Windows. Pero todavía se pueden ejecutar gracias a la compatibilidad con versiones anteriores.

Tenlo en cuenta: no son tan poderosos como los comandos de PowerShell. Un ejemplo de un comando cmd.exe es dir, que casualmente apunta al comando Get-ChildItem de PowerShell, que es también donde apunta el alias ls.

¿Recuerdas el comando de PowerShell Get-Help? Bueno, hay un parámetro de comando que puedes usar para obtener ayuda con comandos de command.exe: "/?". Recuerda la diferencia: Get-Help se usa con comandos de PowerShell, como Get-Help ls, mientras que /? se usa para otros comandos, como "dir /?". Si tratara de usar ls /?, no devolverá nada, porque el comando de PowerShell del que ls es un alias no sabe cómo manejar el parámetro /?, y viceversa.

Eres libre de usar cualquier comando con el que te sientas cómodo. Pero en este curso vamos a usar alias comunes y comandos de PowerShell.
