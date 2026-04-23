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