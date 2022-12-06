# Configuracion Global
git config --global user.name "nombre"
git config --global user.email user@correo
git config --global core.editor "code --wait"

# Evita problemas de return carriage entre windows y linux/mac
git config --global core.autocrlf true
git config --global core.clrf "code --wait"

# BAJA LOS CAMBIOS DE GITHUB
git pull origin <current_branch>

# MUESTRA LOS CAMBIOS QUE HAY
git status
git status -s

# AGREGA TODOS LOS ARCHIVOS NUEVOS Y MODIFICADOS LOCALMENTE O STAGE
git add .
git add regex

# HACE COMMIT A LOS CAMBIOS NUEVOS Y MODIFICADOS LOCALMENTE 
git commit -m "comentario"

# MUESTRA LA RAMA ACTUAL
git branch

# CREAR UNA NUEVA RAMA APARTIR DE LA ACTUAL
git checkout -b <nombrerama>

# CAMBIAR DE RAMA
git checkout <nombrerama>

# SUBE TODOS LOS CAMBIOS DE LOS COMMITS HECHOS LOCALMENTE A GITHUB
git push origin <branch> 

# -u indica que la rama no existe en github
git push -u origin <current_branch>

# RECUPERA UN ARHIVO DEL STAGE
git restore <filename>

# ELIMINAR ARCHIVOS
git rm <filename>

# RENOMBRAR ARCHIVOS
git mv <filename> <newfilename>

# VER CAMBIOS DE MANERA VISUAL EN ARCHIVOS
git diff
git diff --staged

# Muestra todos el log de todos los commits
git log --oneline

# PARA SUBIR CODIGO LOCAL A GITHUB CREANDO UN REPOSITORIO O UNO EXISTENTE
git remote add origin <urlgitrepo>
