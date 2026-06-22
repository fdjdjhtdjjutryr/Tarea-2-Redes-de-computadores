Requisitos
Para ejecutar la aplicacion es nesesario contar con:
-Sistema operativo Linux.
-Compilador de C (gcc).
-Terminal de comandos.

Instalacion:
-Descargar Repositorio en formato .zip.
-Descomprimir archivo.
-Abrir una terminal en la carpeta donde se encuentra el archivo del proyecto.

Compilacion:
-Ejecutar los siguientes comandos en la terminal:
      *Para compilar servidor*
      gcc sercidor_C.c -o servidor (donde nuestro ejecutable sera "servidor").
      *Para compilar el cliente*
      gcc Cliente_C.c -o cliente (donde nuestro ejecutable sera "cliente").

Ejecucion:
-Para obtener la ip del servidor , ejecutar el siguiente comando en la terminal:
      *ip a*
-Para ejecutar el servidor
      *./servidor 12345*
      Donde 12345 es el puerto , pero puede ser cualquier puerto disponible.
-Para ejecutar el cliente(en otra maquina o en la misma)
      *./cliente <ip_servidor> <puerto>*
      Donde ip_servidor es la ip que obtuvimos con ip a , en pasos anteriores , en caso de compilar en la misma maquina , igual se puede usar localhost 127.0.0.1 , y puerto es el mismo puerto utilizado en servidor.

Funcionalidades: La aplicacion soporta 2 comandos:
-Comando "listar" :Muestra todos los archivos disponibles del servidor , que son los que se encuentran en la misma carpeta del ejecutable.
      *ejemplo: Al conectarse de manera exitosa , escribimos en la terminal del cliente "listar"*
Comando "descargar" :Permite descargar un archivo desde el servidor al cliente, se debe procurar escribir el nombre y la extension del archivo a descargar.
      *ejemplo: al listar y ver los posibles archivos , escribimos "descargar nombre_archivo.extension" -> ejemplo:"descargar texto_enviado.txt" luego el archivo se guardara en la carpeta donde este el ejecutable
      de cliente*

A tener en cuenta:
El servidor debe estar andando antes de querer conectar el cliente.
Ambos equipos deben estar en la misma red.
Si el puerto esta en uso se debe elegir otro puerto.
Los archivos se buscan en el directorio donde esta el servidor , y se desvargan donde esta el directorio del cliente.

Profesor: Yasmany Prieto.
Autores: Oscar Gonzalez , Jeremy Mendoza , Franco Videla.
