---
layout: post
title:  "Como crear tu primer blog con Jekyll"
date:   2021-11-09 15:19:08 -0600
categories: jekyll update
---

## Instalación
Estos son los pasos para la estructura inicial de como crear un blog simple en Jekyll. Primero necesitamos descargar la versión más reciente de Ruby e instalar Jekyll en la computadora esto se puede realizar desde la página oficial. Después de esto realizaremos la instalación de Jekyll desde la consola de Windows.

##### Links de descarga
* [Ruby]
* [Jekyll]
* [Guía de instalación Brocollini]
* [Youtube video instalación]
* [Stackoverflow soluciones server]

[Ruby]: https://rubyinstaller.org/
[Jekyll]:   https://jekyllrb.com/
[Guía de instalación Brocollini]: https://broccolini.net/swiss/about/
[Youtube video instalación]: https://www.youtube.com/watch?v=yNSOL3KYJ7Y&ab_channel=DrupalalSur
[Stackoverflow soluciones server]: https://stackoverflow.com/questions/37055554/jekyll-serve-not-working

Una vez realizadas las descargas debemos correr el Ruby Installer. Después debemos de iniciar command prompt desde el buscador de Windows o Inicio, otra opción seria iniciar la consola de Windows y verificar desde allí si Ruby fue instalado.

Ejemplos:
{% highlight ruby %}
C:\Users\user>ruby -v
ruby 3.0.2p107 (2021-07-07 revision 0db68f0233) [x64-mingw32]
{% endhighlight %}

Para checar Gem version de Ruby usamos:
{% highlight ruby %}
C:\Users\user>gem -v
3.2.22
{% endhighlight %}

Para installar Jekyll realizaríamos la instalación desde command prompt de Ruby.
{% highlight ruby %}
C:\Users\user>gem install jekyll bundler
{% endhighlight %}

Verificando la versión de Jekyll obtendríamos
{% highlight ruby %}
C:\Users\user>jekyll -v
jekyll 4.2.1
{% endhighlight %}

## Creando el blog
Para crear el primer blog el estilo por default es minima. Para crearlo utilizaremos lo siguiente.

{% highlight ruby %}
C:\Users\user>jekyll new nombredetublog
{% endhighlight %}

Ahora hay que cambiar el directorio a la carpeta que creamos.
{% highlight ruby %}
C:\Users\user>cd nombredetublog
{% endhighlight %}

Para ver el resultado abrimos el server local. El cual sera: http://localhost:4000 
{% highlight ruby %}
C:\Users\user>bundle exec jekyll serve
{% endhighlight %}

## Plantillas

Este blog fue creado con la plantilla de Swiss existen distintas plantillas y sitios en los cuales puedes elegir la opción que más te guste o necesites.

![](https://cloud.githubusercontent.com/assets/334891/18477206/d9dc55fc-799a-11e6-89f2-b4ae150caa80.png)

##### Sitios en donde puedes encontrar plantillas

* Links
  * [Jekyll Themes]
  * [Jamstack Themes]
  * [Jekyll-Themes.com]

 [Jekyll Themes]: https://jekyllthemes.io/
 [Jamstack Themes]: https://jamstackthemes.dev/ssg/jekyll/
 [Jekyll-Themes.com]: https://jekyll-themes.com/
 
## Instalacion de plantillas
Para realizar la instalación de la plantilla Swiss buscaremos el archivo `_config.yml` en el cual modificaremos la información general de la web como los datos e información acerca del blog.

Se utilizan archivos markdown como contenedores de infomación general estos después se actualizan desde la terminal que estes utilizando ya sea el de windows o el editor de tu preferencia, para generar el render del archivo html de la página del blog.

Tendremos dos archivos el `index.markdown` y `about.markdown` los post se nombran por medio de la fecha en la que se van creando más el nombre del post `2021-11-09-titulo.markdown`

## Plantilla Swiss instalacion
Desde la consola agregamos:
{% highlight ruby %}
C:\Users\user>gem "jekyll-swiss"
{% endhighlight %}

Abrimos desde el editor el documento vscode (o el que utilizes) de `_config.yml` y agregamos:
{% highlight ruby %}
theme: jekyll-swiss
{% endhighlight %}

Para actualizar agregamos en la terminal:
{% highlight ruby %}
C:\Users\user>bundle
{% endhighlight %}

Para finalizar la instalacion agregamos
{% highlight ruby %}
C:\Users\user>gem install jekyll-swiss
{% endhighlight %}

En caso de que no detecte la actualizacion o existan errores en el server, podemos agregar lo siguiente.
{% highlight ruby %}
C:\Users\user>gem cleanup
{% endhighlight %}

{% highlight ruby %}
C:\Users\user>bundle exec jekyll serve
{% endhighlight %}

Otra opcion seria agregar:
{% highlight ruby %}
C:\Users\user>bundle add webrick
{% endhighlight %}

{% highlight ruby %}
C:\Users\user>bundle exec jekyll serve
{% endhighlight %}

> Puedes leer la documentacion de Jekyll en caso de tener dudas mas complejas acerca del funcionamiento de este asi como revisar el apartado de Stackoverflow en caso de tener dudas sobre el codigo.