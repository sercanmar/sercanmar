# Resumen de Git 1 DAW
---
---
## Configuración de herramientas
- git config --global user.name "[name]
> Establece el nombre que desea esté anexado a sus transacciones de commit
- git config --global user.email "[email address]" 
> Establece el e-mail que desea esté anexado a sus transacciones de commi
- git config --global color.ui auto 
> Habilita la útil colorización del producto de la línea de comando
---
## Crear repositorios
- git init [nombre_proyecto] 
> Crea un nuevo repositorio local con el nombre especificado
- git clone [url] 
> Descarga un proyecto y toda su historia de versión
---
## Cambios
- git status
> Enumera todos los archivos nuevos o modificados que se deben confirmar
- git diff 
> Muestra las diferencias de archivos que no se han enviado aún al
área de espera
- git add [archivo] 
> Toma una instantánea del archivo para preparar la versión
- git diff --staged 
> Muestra las diferencias del archivo entre el área de espera y la última versión del archivo
- git reset [archivo] 
> Mueve el archivo del área de espera, pero preserva su contenido
- git commit -m "comentario commit" 
> Registra las instantáneas del archivo permanentemente en el historial de versión
---
## Cambios grupales
- git branch 
> Enumera todas las ramas en el repositorio actual
- git branch [nombre_rama] 
> Crea una nueva rama
- git checkout [nombre_rama] 
> Cambia a la rama especificada y actualiza el directorio activo
- git merge [nombre_rama] 
> Combina el historial de la rama especificada con la rama actual
- git branch -d [nombre_rama] 
> Borra la rama especificada
---
## Nombres del archivo de refactorización
- git rm [archivo] 
> Borra el archivo del directorio activo y pone en el área de espera el archivo borrado
- git rm --cached [archivo] 
> Retira el archivo del control de versiones, pero preserva el archivo a nivel local
- git mv [archivo_original] [archivo_renombrado] 
> Cambia el nombre del archivo y lo prepara para commit
---
## Repasar historial
- git log 
> Enumera el historial de la versión para la rama actual
- git log --follow [archivo] 
> Enumera el historial de versión para el archivo, incluidos los cambios de nombre
- git diff [primera_rama]...[segunda_rama] 
> Muestra las diferencias de contenido entre dos ramas
- git show [commit] 
> Produce metadatos y cambios de contenido del commit especificado
---
## Rehacer commits
- git reset [commit] 
> Deshace todos los commits después de [commit], preservando los cambios localmente
- git reset --hard [commit] 
> Desecha todo el historial y regresa al commit especificado
---
## Sincronizar cambios
- git fetch [marcador] 
> Descarga todo el historial del marcador del repositorio
- git merge [marcador]/[rama] 
> Combina la rama del marcador con la rama local actual
- git push [alias] [rama] 
> Carga todos los commits de la rama local al GitHub
- git pull 
> Descarga el historial del marcador e incorpora cambios
---
---
