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




