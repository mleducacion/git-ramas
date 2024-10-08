# GIT RAMAS (Branches)

## Crear un repositorio

```sh
git init
```

## Ver el status de los archivos

```sh
git status
```

## Git Alias

```sh
git config --global alias.st "status --short"
git config --global alias.a "add"
git config --global alias.c "commit -m"
git config --global alias.l "log --oneline"
```

## Ver las diferencias entre el WD y LR

```sh
git diff
``` 

## Ver el contenido de cada commit

```sh
git show <numero-hash>
```

## Crear un rama

```sh
git branch <nombre-rama> # crea una rama y nos deja en la rama original
git branch feature/ramas # ejemplo
git switch -c <nombre-rama> # crea una rama y nos mueve a la rama que se creo
```

## Me mueve entre ramas

```sh
git switch <nombre-rama>
git switch feature/ramas # ejemplo
``` 

## Comparar entre los últimos commits de las ramas

```sh
git diff <nombre-rama-que-quiero-comparar> # Compararo la rama actual contra la rama que indico
git diff dev # ejemplo. comparo feature/ramas con dev
```

## Ver las ramas locales y remotas

```sh
git branch -a # Me muestra las ramas locales y remotas
```

## Fusionando ramas
Estoy sobre la rama main y me quiero traer lo que está en feature/ramas

```sh
git merge <rama-que-quiero-fusionar>
# ejemplo
git switch main 
git merge feature/ramas # Me traigo a main lo que tenía en feature/ramas
```

* Fusión -> Fast-forward -> git hace la fusión automaticamente.

## Eliminar un rama 

```sh
git branch -d <nombre-rama> # Si la rama que estoy borrando ya fue fusionada me va a borrar la rama.
git branch -D <nombre-rama> # confirmación de borrado de una rama que todavía no ha sido fusionada en el repositorio
git branch -d feature/ramas #ya estaba fusionada feature/ramas
git branch -D alejo # no estaba fusioanda por lo cual me pidio confirmación
```






