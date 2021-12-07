---
layout: post
title:  "Github y Jekyll"
date:   2021-11-09 15:19:08 -0600
categories: jekyll update
---
## Como usar Github como hosting junto con Jekyll
Primero tendremos que hacer una cuenta en Gihub, en la cual haremos un nuevo repository desde el sitio web para poder guardar nuestro blog o sitio creado con Jekyll. Creamos el repository cuidando que este sea un código publico. Para hacer el primer commit vamos a hacerlo directamente desde la terminal del editor que estes utilizando.

Desde el archivo dentro de nuestro blog buscaremos `_config.yml` y agregaremos el nombre de nuestro repository en `baseurl:""` guardaremos los cambios.
Ejemplo:
````
baseurl: "mentalnotes"
````

## Iniciamos codeando:

````
git init
````
>Es opcional agregar README.md en caso de que lo necesites.

````
git checkout -b gh-pages
git status
git add .
git commit -m "comentario"
git remote add origin "www.tuweb.com"
git push origin gh-pages
````
Para verificar el estado de los archivos que aún no se han cargado marcados en color rojo y verde si ya se encuentran en el repository
````
git status
````

Agregamos los documentos que contiene nuestra carpeta
````
git add.
````
Realizamos el commit
````
git commit -m "comentario"
````
````
git remote add origin "www.github.io/tublog"
````
>La dirección de tú repository la puedes encontrar en github al crearlo te dará una pequeña lista de código.

Este sera la rama en la que se encontrara el blog, se puede seleccionar directamente desde la página de github en caso de que esta no cargue.

````
git push origin gh-pages
````
>Esto cargara los archivos directamente al repository para corroborarlo visitamos el link que nos proporciono github previamente

## Como actualizar el código

Utilizaremos lo siguiente:

````
git add .
git commit -m "comentario"
git push origin gh-pages
````
>Algunos errores que me encontré fueron como hacer el loging directamente desde la consola o la detección del theme que seleccione.

## Links de ayuda
* [Youtube Tutorial]
* [Stackoverflow]
* [MadeMistakes.com]

[Youtube Tutorial]: https://www.youtube.com/watch?v=fqFjuX4VZmU&t=156s&ab_channel=MikeDane
[Stackoverflow]: https://stackoverflow.com/questions/22514104/cant-get-site-baseurl-to-work-in-jekyll
[MadeMistakes.com]: https://mademistakes.com/mastering-jekyll/site-url-baseurl/
