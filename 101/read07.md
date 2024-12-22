# ¿Qué es y cómo funciona el control de versiones en Git?

Git es un sistema de control de versiones distribuido que permite rastrear cambios en archivos y coordinar el trabajo entre desarrolladores. Funciona mediante un historial de cambios, permitiendo revertir a versiones anteriores, colaborar en equipo y manejar diferentes ramas de desarrollo.

## Comandos básicos de Git

**1. Configuración inicial:**  

Configura tu identidad para los commits:  

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
```

**2. Inicializar o clonar un repositorio:**

- `git init`: Crea un nuevo repositorio Git en un directorio.
- `git clone [URL]`: Clona un repositorio remoto existente.

```bash
git init
git clone https://github.com/usuario/repositorio.git
```

**3. Rastreo y guardado de cambios:**

- `git status`: Muestra el estado actual del repositorio.
- `git add [archivo]`: Agrega un archivo al área de preparación (staging area).
- `git commit -m "mensaje"`: Guarda los cambios en el historial del repositorio.

```bash
git status
git add archivo.txt
git commit -m "Añadido archivo inicial"
```

**4. Sincronización con repositorios remotos:**

- `git push origin [rama]`: Sube los cambios al repositorio remoto.
- `git pull origin [rama]`: Descarga y fusiona cambios del repositorio remoto.

```bash
git push origin [rama]: Sube los cambios al repositorio remoto.
git pull origin [rama]: Descarga y fusiona cambios del repositorio remoto.
```

**5. Ramas:**

- `git branch [nombre]`: Crea una nueva rama.
- `git checkout [nombre]`: Cambia a una rama específica.
- `git merge [rama]`: Fusiona una rama con la rama actual.

```bash
git branch desarrollo
git checkout desarrollo
```

## Ejemplo de flujo básico de trabajo

```bash
# 1. Inicializar un repositorio o clonar uno existente
git init
git clone https://github.com/usuario/repositorio.git

# 2. Crear y rastrear cambios
echo "Hola, mundo" > archivo.txt
git add archivo.txt
git commit -m "Creado archivo inicial"

# 3. Subir cambios al repositorio remoto
git push origin main

# 4. Crear y trabajar en una rama nueva
git branch nueva-rama
git checkout nueva-rama
echo "Nueva característica" >> archivo.txt
git add archivo.txt
git commit -m "Añadida nueva característica"

# 5. Fusionar la rama nueva a la rama principal
git checkout main
git merge nueva-rama
git push origin main
```

Con estos comandos, puedes gestionar versiones y colaborar eficazmente en proyectos usando Git.

### READ 07

**1. ¿Qué es el control de versiones?**
Git es un sistema de control de versiones distribuido que permite rastrear cambios en archivos y coordinar el trabajo entre desarrolladores. Funciona mediante un historial de cambios, permitiendo revertir a versiones anteriores, colaborar en equipo y manejar diferentes ramas de desarrollo.

**2. ¿Qué es “clone” en Git?**
En Git, el comando clone se utiliza para crear una copia de un repositorio existente en un nuevo directorio local. Este comando es fundamental cuando deseas trabajar en un proyecto que ya existe en un repositorio remoto, como GitHub.

**3. ¿Cuál es el comando para agregar los archivos modificados a la zona de preparación?**

Para agregar los archivos modificados a la zona de preparación (staging area) en Git, utilizas el comando git add.

- Agregar un archivo específico:

Esto agrega un archivo específico a la zona de preparación.
`git add nombre_del_archivo`

- Agregar todos los archivos modificados

Este comando agrega todos los archivos modificados en el directorio actual y sus subdirectorios a la zona de preparación.
`git add .`

- Agregar archivos en un directorio específico:

Esto agrega todos los archivos modificados dentro de un directorio específico a la zona de preparación.

`git add nombre_del_directorio/`

- Agregar archivos que coincidan con un patrón:

Este comando agrega todos los archivos con la extensión .txt a la zona de preparación.

`git add *.txt`

**4. ¿Cuál es el comando para enviar la captura de los archivos modificados a Github?**

Para enviar los cambios confirmados (commits) a un repositorio remoto en GitHub, utilizas el comando git push. Los pasos son:

- Asegurar de que los cambios estén confirmados

`git commit -m "Descripción de los cambios"`

- Envía los cambios al repositorio remoto:

`git push origin nombre-de-la-rama`

**origin**: Es el nombre predeterminado del repositorio remoto. Si has clonado el repositorio, este nombre ya estará configurado.

**nombre-de-la-rama**: Especifica la rama a la que deseas enviar los cambios. Por ejemplo, main o master.

`git push origin main`

Este comando enviará los cambios confirmados en tu rama local al repositorio remoto en GitHub. Si es la primera vez que haces un push a una nueva rama, puede que necesites usar la opción -u para establecer la rama de seguimiento:

`git push -u origin nombre-de-la-rama`
