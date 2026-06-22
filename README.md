Para ejecutar , se deben tener las dependencias , se debe tener las dependencias c/c++ nesesarias para la compilacion.
Descarguen el repositorio en formato .zip , luego descompriman .

En linux , abran la terminal y trabajando siempre en la carpeta donde estan los archivos.
-Para crear el ejecutable de el servidor utilizen el comando gcc servidor_C.c -o servidor
-Para crear el ejecutable de el cliente utilizen el comando gcc Cliente_C.c -o cliente
-Para saber el ip del servidor , en la maquina que funcione de servidor , escriban en la terminal "ip a".
-Corran el servidor , usando el puerto que deseen , en la terminal escriban por ejemplo ./servidor 12345 , asi usaran el ejecutable servidor y le daran el puerto 12345
      -En caso de que el servidor este ocupado , sirve ejecutar con otro puerto que no este ocupado.
-Luego de que el servidor este corriendo , pueden conectarse escribiendo en la terminal , ./cliente *ip del servidor* *puerto servidor* donde *ip del servidor* es la direccion que obtuvimos usando el comando ip a y 
*puerto servidor* es el puerto que tengamos en el servidor.

Nuestra aplicacion soporta 2 comandos 
-Comando "listar" , el cual nos muestra todos los archivos que esten en la carpeta donde esta el ejecutable del servidor
-Comando "descargar" , el cual combinando con el nombre textual de algun archivo+ la extension de este (.txt , .pdf , etc) podremos descargar , como ejemplo al descargar el zip y ejecutar el servidor , si no mueven el
ejecutable de la carpeta , el cliente podria descargar el archivo "texto_enviado.txt" usando el siguiente comando "descargar texto_enviado.txt".
