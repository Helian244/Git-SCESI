# Curso GIT SCESI 2026
# Clase 1
## ¿Qué es GIT?
Es un Sistema Controlador de Versiones (VCS).
Permite guardar archivos y sus versiones tanto de manera local como remota.
## ¿Cómo nació GIT?
Su creador es Linus Torvalds, cuando él se animo a hacer trabajos con contribuidores
externos, siendo que le agotaba revisar cada email con los aportes del resto.

# Clase 2
## Estados en GIT
### Modified
Cuando un archivo acaba de ser editado en el local y aun no esta en el remoto, estos cambios no estan confirmados
### Staged
Cuando se preparan los archivos y cambios que se desean guardar en el repositorio
### Committed
Cuando el archivo y sus cambios se guardan en el local con un indentificador que pasa al historial

![git states](<Git States.png>)

## Directorio de Trabajo (Modified)
### Untracked
Archivo sin seguimiento, usualmente recien creado, que no tiene una version anterior
### Modified
Un archivo con version previa, pero que ha sido modificado, eliminado o con nuevo nombre

### ***git restore \<archivo>***
Elimina todo lo escrito o modificado dentro de un archivo

### ***.gitignore***
Dentro de este archivo modificamos las referecias, para agregar un archivo que deseamos que no sea visto por git

![.gitignore](<.gitignore.png>)

## Staged Area (Staged)
En este estado se permite seleccionar los archivos modificados para guardarlos en el commit

### ***git add \<archivo>***
Agrega un archivo en específico
### ***git add .***
Agrega todos los archivos que estan modificados vistos por GIT

### ***git restore --staged \<archivo>***
Mueve un archivo del staged area a su estado anterior

## Repositorio Local (Committed)
En este estado se guarda un punto de guardado en el historial
### ***git commit -m "mensaje"***
Para guardar todos los cambios en el staged area
### ***git reset --soft HEAD~1***
Para deshacer los cambios del último commit

# Clase 4
## ***git remote***
Nos permite gestionar nuestra conexion con repositorios remotos, direcciona donde lleva o traer los cambios al local
### ***git remote -v***
Nos deja ver las URLs que estan siendo apuntadas por nuestro repositorio
### ***git remote add \<apodo> "url"***
Vincula nuestro local con un repo de la nube
### ***git remote set-url \<apodo> "url"***
Cambia la URL donde apunta nuestro local

# Clase 5
## Ramas
De las principales funciones para llevar a cabo un mejor control del código.
Bifurca el estado del código y crea un nuevo camino para la evolucion del mismo en paralelo a otras modificaciones.
## Git Branch
Es un comando que nos permite gestionar las ramas que tiene el proyecto
### ***git branch***
Nos permite listar las ramas y ver donde esta el HEAD
### ***git branch \<rama>***
Crea una rama a partir de la rama en la que nos encontremos
### ***git branch -D \<rama>***
Borra la rama

# Clase 6
## ***git merge***
Nos permite combinar dos ramas para que tenga ambos commits realizados
## ***git fetch***
Permite ver cambios en la rama principal y en las ramas hijas