# ¿Qué es y cómo funciona el control de versiones en Git?

Git es un sistema de control de versiones distribuido que permite rastrear cambios en archivos y coordinar el trabajo entre desarrolladores. Funciona mediante un historial de cambios, permitiendo revertir a versiones anteriores, colaborar en equipo y manejar diferentes ramas de desarrollo.

## Comandos básicos de Git

**1. Configuración inicial**  

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
