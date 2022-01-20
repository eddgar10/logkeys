# logkeys
Keylogger para ubuntu con diccionario para teclado español

 logkeys - a GNU/Linux keylogger that works!

https://exdebian.org/wiki/logkeys-un-keylogger-para-gnulinux

# instalación y configuración:

> ## ejecutar el archivo .deb con 
###### ` sudo dpkg -i logkeys_0.1.1a+git5ef6b0dcb9e3-2_amd64.deb` 

> ## ejecución con el mapa de caracteres predeterminado dara una salida a caracteres distintos al teclado en español:
###### ` sudo logkeys -s` 

> ## ejecucion con el mapa de caracteres en español:
###### ` sudo logkeys -s -m /home/nombre_usuario_sudo/carpeta_donde_se_descargo/es_ES.map` 

> ## consulta de caracteres tecleados:
el archivo .log se genera automaticamente en el direciorio
###### ` /var/log/logkeys.log` 
para visualizarlo se debe ejecutar con privilegios de administrador
###### ` sudo cat /var/log/logkeys.log` 

###### ` sudo tail -f /var/log/logkeys.log` 

> ## si el servicio se ejecuta desde ssh al cerrar la terminal se temrina la ejecucion del proceso por lo cual se debe ejecutar con nohup para un proceso en segundo plano, referencia:

http://www.nexolinux.com/bash-scripting-nohup-y-procesos-en-segundo-plano/

 ###### ` sudo nohup logkeys -s -m /home/home/nombre_usuario_sudo/carpeta_donde_se_descargo/es_ES.map` 

> ## para remover:
###### ` sudo apt remove logkeys -y` 
