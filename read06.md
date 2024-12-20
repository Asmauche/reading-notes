 # READ 06: Developer Tools
 ## 1.	¿Qué hacen los siguientes comandos?
 * Pwd: Muestra la ruta completa del directorio de trabajo actual en el que te encuentras
 * Ls: El comando ls lista los archivos y directorios de tu sistema.
 * Cd: El comando cd se utiliza para navegar por los archivos y directorios de Linux.
 * Mkdir: El comando mkdir crea uno o varios directorios y establece sus permisos.
 * Touch: El comando touch te permite crear un archivo vacío en una ruta de directorio específica.
## 2.	¿Puedes explicar qué sucede en el siguiente escenario si ingresas estos comandos y argumentos en la línea de comandos? (Los argumentos son instrucciones adicionales dadas a un comando).
* cd projects: Ingresaras a la carpeta y/o directorio “projects”
* mkdir new-project: Creación de un directorio nuevo además de establecer permisos para la misma.
* touch new-project/newfile.md: Creacion del archivo newfile.md dentro del Directorio new-project
* cd ..: Cuando ejecutas cd .., el sistema te moverá un nivel hacia arriba en la jerarquía de directorios. Por ejemplo, si estás en /home/usuario/documentos, al ejecutar cd .., te moverás a /home/usuario.
* ls projects/new-project: El comando mostrará una lista de los archivos y subdirectorios dentro del directorio "new-projects".
## 3.	¿Qué comando usarías en la terminal para listar todos los archivos, incluidos los archivos ocultos, en un directorio de Linux o macOS? Explica qué significan los parámetros utilizados en el comando.
* ls: Este es el comando básico para listar el contenido de un directorio.
* -a: Esta opción le indica al comando ls que incluya todos los archivos en la lista, incluidos los archivos ocultos.
**ls -a**
