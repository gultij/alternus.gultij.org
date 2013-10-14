---
title: Cómo participar
layout: front
---
# Cómo participar

Según si tienes cuenta de Github y si sabes manejar Git o si tienes correo electrónico, hay varias formas de participar.


## Si cuentas con Github, Git y Jekyll 1.x.

Este es el método que nos ahorra más trabajo a nosotros.

1. *Forkea* este repositorio usando el botón *Fork* en [la página del repositorio](https://github.com/alvarezp/alternativas.gultij.org).

1. Usando Git, clona el repositorio que se creó en tu cuenta. Si tu nombre de usuario es `nombreusuario`:

   `git clone git@github.com:nombreusuario/alternativas.gultij.org.git`

1. Realiza tus modificaciones. Las fichas están en archivos .md en formato Markdown.

1. Ejecuta `jekyll serve -w --config _config_local.yml` en el directorio raíz del repositorio y visita desde tu navegador [tu copia local de Alternativas](http://localhost:4000).

1. *Commitea* los cambios con `git commit -a`. Usa un **buen** mensaje de commit: la primera línea debe ser concreta sobre lo que hiciste y después de un renglón en blanco, un párrafo que explique a detalle por qué era necesario el cambio. Un buen mensaje de commit permite a los desarrolladores contestar dudas sobre tu trabajo y tomar decisiones más precisas.

1. Empuja los cambios hacia tu *fork* de Github con `git push`. Es posible que Git te haga seguir uno o dos pasos más, como el uso de *--set-upstream* o configurar el funcionamiento de *git push*. Estos pasos extra no son recurrentes; son configuraciones iniciales.

1. Regresa a la página de tu copia en Github y presiona el botón *Pull Request*. Sigue las instrucciones. No olvides también documentar apropiadamente el *Pull Request*. Si sólo tienes un *commit*, puedes usar el mismo texto.


## Para contribuir usando Git y Jekyll 1.x, sin Github

1. Usando Git, clona el repositorio de *Alternativas*:

   `git clone git@github.com:alvarezp/alternativas.gultij.org.git`

1. Realiza tus modificaciones. Las fichas están en archivos .md en formato Markdown.

1. Ejecuta `jekyll serve -w --config _config_local.yml` en el directorio raíz del repositorio y visita desde tu navegador [tu copia local de Alternativas](http://localhost:4000).

1. *Commitea* los cambios con `git commit -a`. Usa un **buen** mensaje de commit: la primera línea debe ser concreta sobre lo que hiciste y después de un renglón en blanco, un párrafo que explique a detalle por qué era necesario el cambio. Un buen mensaje de commit permite a los desarrolladores contestar dudas sobre tu trabajo y tomar decisiones más precisas.

1. Prepara los parches con `git format-patch origin/master`. Esto generará algunos archivos cuyo nombre será algo como `0001-descripcion-del-parche.patch`. Generará tantos archivos como commits hayas realizado.

1. Envía los parches adjuntos por correo electrónico a alvarezp o a dualbus.


## Para contribuir usando sólo Github (no Git, no Jekyll)

1. *Forkea* este repositorio usando el botón *Fork* en [la página del repositorio](https://github.com/alvarezp/alternativas.gultij.org). Esto creará una copia del repositorio en **tu** cuenta.

1. Visita esta copia del repositorio en tu cuenta. Si tu nombre de usuario es `nombreusuario`, el repositorio estará en [https://github.com/nombreusuario/alternativas.gultij.org]().

1. Hay un botón llamado "branch: master". Haz clic y cambia la *rama (branch)* por `gh-pages`

1. Entra a la página de la ficha que quieres cambiar. Las fichas están en archivos .md en formato Markdown. Navega a través de los archivos vía Web hasta que encuentres el que deseas modificar.

   Para facilitarlo, cada ficha menciona al final la ruta al archivo de la ficha. No hagas clic a la liga, sólo busca el archivo descrito en la ficha, en tu repositorio.

1. Usa el botón *Edit* y realiza tus modificaciones. Ese cambio se registrará como un *commit*. Usa un **buen** mensaje de commit: la primera línea debe ser concreta sobre lo que hiciste y después de un renglón en blanco, un párrafo que explique a detalle por qué era necesario el cambio. Un buen mensaje de commit permite a los desarrolladores contestar dudas sobre tu trabajo y tomar decisiones más precisas.

1. Regresa a la página de tu copia en Github y presiona el botón *Pull Request*. Sigue las instrucciones. No olvides también documentar apropiadamente el *Pull Request*. Si sólo tienes un *commit*, puedes usar el mismo texto.


## Para contribuir por correo electrónico (no necesitas Git ni Github ni Jekyll)

Este es el medio que más trabajo nos demanda, así que tal vez nos tardemos un poco más en tomar los cambios. Sin embargo, es un medio oficial deliberadamente aceptado. Que no te de pena enviar cambios de esta forma.

1. Al final de cada ficha está la liga a su código fuente. Haz clic.

1. Copia y pega el código en un editor simple (gedit, Notepad; no LibreOffice, no Word).

1. Realiza tus modificaciones y guarda el archivo.

1. Envía el nuevo archivo adjunto a alvarezp o a dualbus. Es muy importante que detalles los cambios y el motivo de los mismos. Si sabes usar *diff*, también puedes enviarlo como *parche*.


