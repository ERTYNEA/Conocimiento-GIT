# Conocimiento-GIT
Comandos sencillos de GIT para usarlos en el dia a dia 🤓👍
---
**Clonar una rama especifica del servidor:**
```
git clone -b NombreDeLaRamaDelServidorAClonar DirectorioLocalDondeSeClonara
```
**Ver la configuración actual de git:**
```
git config --list
```
**Cambiar el nombre de usuario en la configuración actual de git a nivel global:**
```
git config --global user.name "NombreDeUsuaio"
```
**Cambiar el email de usuario en la configuración actual de git a nivel global:**
```
git config --global user.email “EmailDeUsuaio”
```
**Ver la url del origen remoto de datos del repositorio:**
```
git remote -v
```
**Cambiar la url del origen remoto de datos del repositorio:**
```
git remote set-url origin NuevaUrl
```
**Ver el estado del repositorio local:**
```
git status
```
**Consultar cambios en el reposorio del servidor:**
```
git fetch
```
**Consultar cambios en el reposorio del servidor y borrar las ramas locales prunadas en el servidor:**
```
git fetch --prune
```
**Almacenar temporalmente en la pila los cambios que aun no se han comiteado incluyendo los cambios de los archivos no trackeados:**
```
git stash save -u
```
**Mostrar los cambios temporales que se almacenaron en la pila:**
```
git stash list
```
**Volver a aplicar los ultimos cambios temporales que se almacenaron en la pila:**
```
git stash apply "stash@{0}"
```
**Limpiar la pila de los cambios temporales almacenados:**
```
git stash clear
```
**Aplicar en nuestra rama local los cambios que se han consultado al servidor (previamente mediante un git fetch):**
```
git pull
```
**Aplicar en nuestra rama local actual los cambios que tiene otra de nuestras ramas locales (posteriormente se puede hacer git push para subir nuestra rama actual al servidor):**
```
git merge NombreDeLaRamaConLosCambios
```
**Ver de forma grafica todas las ramas con todos sus cambios y autores de cada cambio:**
```
gitk --all
```
**Crear una rama local:**
```
git branch NombreDeLaRamaACrear
```
**Cambiar a otra rama local:**
```
git checkout NombreDeLaRamaALaQueCambiar
```
**Ver los cambios que tiene un archivo y que aun no se han comiteado:**
```
git diff RutaAlArchivo
```
**Añadir manualmente pequeños cambios de un archivo a un futuro commit:**
```
git add -p RutaAlArchivo
```
**Comitear cambios que se han añadido (mediante git add):**
```
 git commit -m MensajeDelCommit
```
**Mandar los cambios que ya se han comiteado al servidor:**
```
git push
```
**Quitar los cambios de un archivo que aun no se han comiteado:**
```
git restore RutaAlArchivo
```
**Ver las ramas locales:**
```
git branch
```
**Ver las ramas del servidor:**
```
git branch -r
```
**Ver las ramas locales y las ramas del servidor:**
```
git branch -a
```
**Borrar una rama local (posteriormente se puede hacer git push origin NombreDeLaRamaBorrada para borrarla en el servidor):**
```
git branch -d NombreDeLaRamaABorrar
```
**Borrar una rama local de forma forzada (posteriormente se puede hacer git push origin NombreDeLaRamaBorrada para borrarla en el servidor):**
```
git branch -D NombreDeLaRamaABorrar
```
**Ver el historial de cambios de un archivo:**
```
git log RutaAlArchivo
```
**Restaurar un archivo a un commit anterior:**
```
git checkout CodigoDelCommitExtraidoConGitLog RutaAlArchivo
```