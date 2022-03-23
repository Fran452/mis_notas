# Que es git
    software de control de versiones

# qué es Github
    Es una plataforma colaborativa que nos va a permitir 
    llevar un control de versión sobre nuestro código.

# comandos de Github
    git init => crea un nuevo repositorio local
    git config user.name "nombre de usuario" => cunfigura usuario en una carpeta Github
    git config user.name => te dice que usuario esta configurado
    git config user.email "mail" => cunfigura mail en una carpeta Github
    git config user.email => te dice que email esta configurado
    git clone "url" => clona repositorio de git
    git add . => agrega todos los archivos dentro del repositorio
    git add "archivo" => guarda archivo al repositorio
    git status => muestra el estado de los archivos de la carpeta
    git push origin master => subir las modificaciones del archivo
    git commit -m "comentario" => comenta los archivos agregado
    git pull origin master=> baja los cambios de la nube
    git remote add origin link => configuarcion repositorio remoto

# Ramas en git
    
## orden =>    
    1| main     => proyecto listo para mostrar
    2| release  => poryecto a probar
    3| develop  => preyecto en proceso de desarrollo
    4| ramas auxiliares => ramas para trabajos diferidos

## Comandos
    git checkout -b "nuevaRama"=> crea y te envia a x rama
    git checkout "rama" => moverse entre ramas
    git merge ramaAClonar => clona una rama a la rama actual
    git branch -m nombre => renombrar una rama
    git push origin --delete rama => para eliminar una rama