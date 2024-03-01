Para cambiar tu contraseña en Linux,
todo lo que debes hacer es ejecutar el comando passwd o contraseña. Intentemos cambiar mi contraseña. Cuando estableces una contraseña,
se la codifica con seguridad, luego se la guarda en un archivo especial con privilegios
llamado /etc/shadow. Solo un root puede leer este archivo,
para alejar ojos curiosos. Aun si tuvieras acceso, no podrías decodificar
las contraseñas encontradas aquí. Si estás administrando una computadora
y quieres forzar a un usuario estándar a que cambie su contraseña, como hicimos en Windows,
puedes usar -e o "marca de expiración", con passwd, así. Esto inmediatamente
hace expirar una contraseña de usuario y luego hace que establezca una nueva contraseña
la próxima vez que acceda.