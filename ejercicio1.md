# Primer ejercicio
## Creación del repositorio y de los archivos
Desde Github, creamos el repositorio de la tarea y dejamos las opciones por defecto

![Creación del repositorio](capturas/capturacreacion.png)
### Añadimos los archivos e inicializamos el repositorio
Creamos los archivos con texto usando echo y la redirección de archivos. Crearemos un repositorio local usando `git init`

![Creación de archivos](capturas/Captura1.png)

## Agregamos el repositorio local al repositorio remoto
Usamos el comando `git remote add origin` para convertirlo en repositorio remoto. Debemos usar el token que generamos en el panel de control de Github junto con nuestro usuario y el enlace del repositorio que se encuentra en la página web. La sintaxis sería la siguiente: `https://USERNAME:TOKEN@github.com/USERNAME/REPO.git`

![Repositorio local a Repo remoto](capturas/Captura2.png)

## Subir repositorio remoto a Github
Usamos `git add .` para seleccionar los archivos que hemos creado para subirlos a Github. Con `git commit`, aplicaremos los cambios y con el comando `git push origin master`, subiremos los cambios a Github. Debemos tener en cuenta el nombre del repositorio remoto, en este caso `origin` y la rama, `branch`.

![Subir a Github](capturas/Captura3.png)

### Resultado en Github

![Resultado Github](capturas/Captura4.png)

## Clonación del repositorio remoto a Debian Virtual
Usamos `git clone https://USERNAME:TOKEN@github.com/USERNAME/REPO.git` para clonar el repositorio remoto y poder aplicar cambios remotamente

![Clonar a Debian](capturas/Captura5.png)

## Añadir y modificar nuevos archivos para el repositorio remoto
Previamente, creamos el nuevo archivo y modificamos uno de los que ya existen y con `git add` y  `git commit`, agregamos los cambios y los confirmamos.
![Nuevos archivos](capturas/Captura6.png)

### Resultado en Github
![Resultado](capturas/Captura7.png)
## Actualizar los archivos en Debian Virtual
Una vez hayamos confirmado los cambios, usaremos el comando `git pull` en la máquina virtual

![Git pull](capturas/Captura8.png)