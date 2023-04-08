# BuenasPracticas
Report asignatura BPP 

# Comandos de la consola:  -->

- Añadir tu Git: 
git config --global user.email "mirilh96@gmail.com
git config --global user.name "Mirilh"

- confirmar el status de nuestra version, saber si esta al dia:
git status

(si estamos al dia On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean)

- Subir un cambio desde la consola, preguntamos el status, nos dice que no estamos al dia, lo subimos: 
git add . (sube todos)
git add main.py (solo actualiza ese archivo especificado)
te dice que se guarda pero hay que hacer el conmmit 

- confirmamos cambios y escribimos mensaje: 
git commit -m 'tercer cambio'

- Ver los cambios que se han ido haciendo, tipo el historial:
git log

resultado: '''commit d18f02644a3e3a42ef638ddd104d46e0428a0b67 (HEAD -> main)
Author: Mirilh <mirilh96@gmail.com>
Date:   Sat Apr 8 12:35:44 2023 +0930

    tercer cambio

commit deeb33096331cf334d5355d12d6660b1592f4254 (origin/main, origin/HEAD)
Author: Mirilh <117718699+Mirilh@users.noreply.github.com>
Date:   Sat Apr 8 12:16:35 2023 +0930
'''

- Volver a una version anterior:
git revert 'El codigo que viene en el log de la version que quieres'


- Crear una rama: 
git branch -m nueba_branch

- guardar en la nueva rama: 
git checkout nueba_branch
git add .
git commit -m 'nueva branch'
git push --set-upstream origin nueba_branch

- como combinar las dos ramas, 1. volvemos a la rama principal
git chechout main
git merge
git push
