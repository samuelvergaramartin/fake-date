# fake-date
Este repositorio trata sobre cómo hacer commits con fechas totalmente personalizadas, y con dos commits de ejemplo en dos archivos: `example-1970.txt` y `example-2099.txt`.

![1970](images/1970.png)

![2099](images/2099.png)

## Ejemplo de uso

Para hacer un commit con una fecha personalizada primero teneis que añadir los archivos de vuestro repositorio de git con `git add`:

```sh
git add .
```
Después teneis que establecer la variable de entorno `GIT_COMMITTER_DATE` con la **fecha** y **hora** que vosotros queráis seguido del comando `git commit`, por ejemplo:

```sh
GIT_COMMITTER_DATE="1970-12-31 23:59:59" git commit --date="1970-12-31 23:59:59" -m "feat: Committed with a fake date"
```

Y ya por último haceis un push normal y corriente:

```sh
git push
```

Y ya tendríais vuestro commit con fecha modificada en vuestro repositorio de GitHub.

Espero que os haya gustado este tutorial! Muchas gracias!