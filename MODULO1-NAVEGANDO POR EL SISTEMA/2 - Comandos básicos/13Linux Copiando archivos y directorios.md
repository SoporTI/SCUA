> [!TIP]  
> [Ver video](https://youtu.be/l_THDqQDt_Y)

En bash se puede usar exactamente
el mismo comando de Windows para copiar archivos. Veamos este directorio.

Copiemos `my_very_cool_file.txt`
a mi escritorio y ahí está. También podemos usar el mismo comodín
(asterisco) para seleccionar patrones. Como esto es similar a nuestro comando
de copia de Windows, ¿qué crees que podemos usar para copiar
los archivos .png en este directorio? Tengo archivos llamados `Pizza.png`,
`Soda.png`, `Cake.png`. Puedo usar `cp *.png`,
y luego, el directorio `Desktop`. Ahora si vuelvo a mirar mi escritorio,
allí están. Las mismas reglas de copia se aplican en bash.

Si queremos copiar un directorio, tenemos que copiarlo de forma recursiva
para obtener todos los contenidos. El indicador para la copia recursiva es `-r`. Si quiero copiar la carpeta
con fotos de mi gato al escritorio, puedo hacer algo como esto. Y ahí está.
