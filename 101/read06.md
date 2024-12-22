# Comandos básicos de Linux para desarrollar en Git Bash y GitHub

Linux, Git Bash y GitHub son herramientas esenciales en el desarrollo de software. Linux proporciona comandos para manejar archivos y directorios, mientras que Git y GitHub se utilizan para control de versiones y colaboración.

## Comandos básicos de Linux en Git Bash

**1. Navegación y manipulación de archivos:**  

- `ls`: Lista los archivos y directorios.  
- `cd [directorio]`: Cambia al directorio especificado.  
- `mkdir [nombre]`: Crea un nuevo directorio.  
- `rm [archivo]`: Elimina un archivo. Usa `rm -r [directorio]` para eliminar un directorio.

Ejemplo:  

```bash
mkdir proyecto
cd proyecto
```

**2. Visualización y edición:**

- cat [archivo]: Muestra el contenido de un archivo.
- nano [archivo]: Abre un archivo para editarlo (si nano está instalado).

```bash
nano README.md
```

## Comandos de Git para desarrollar en GitHub

**1.Inicializar y clonar repositorios:**

- git init: Inicializa un repositorio Git en un directorio.
- git clone [URL]: Clona un repositorio remoto.

```bash
git init
git clone https://github.com/usuario/repositorio.git
```

**2.Rastreo de cambios:**

- git status: Muestra el estado de los cambios.
- git add [archivo]: Agrega archivos al área de preparación (staging area).
- git commit -m "mensaje": Guarda los cambios en el historial.

```bash
git add archivo.txt
git commit -m "Añadido archivo inicial"
```

**3.Sincronización con GitHub:**

- git push origin [rama]: Sube cambios al repositorio remoto.
- git pull origin [rama]: Descarga y fusiona cambios del repositorio remoto.

```bash
git push origin main
git pull origin main
```

## Ejemplo de flujo de trabajo con GitHub

```bash
# 1. Clonar un repositorio
git clone https://github.com/usuario/repositorio.git
cd repositorio

# 2. Crear y editar archivos
echo "Mi primer proyecto" > README.md
git add README.md

# 3. Realizar un commit
git commit -m "Añadido README.md"

# 4. Subir cambios a GitHub
git push origin main
```
