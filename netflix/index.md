---
title: Netflix y Linux
layout: servicio

f_creacion: 2014-01-10
f_revision: 2014-01-10

liga: http://compholio.com/netflix-desktop/

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

funciona_blah: no
funciona_fedora: no

funciona_parabola: no
funciona_archlinux: no
---

# Descripción de la página

Como utilizar netflix desde Linux, aunque realmente es como utilizar Silverlight en Linux.

# Por que no funcionan con Software Libre

[Silverlight](http://www.microsoft.com/silverlight/) es una tecnología propietaria de Microsoft y creo que esto es suficiente información para saber por que no funciona con software.

# Cómo corregirlo

Desgraciadamente no hay manera de hacerlo debido a que el desarrollo de Silverlight para linux no existe.

# Rodeos y alternativas

## Instalar software híbrido (Open Source y Propietario) pensado únicamente en servicios como Netflix

En este caso tenemos a [Netflix-Desktop](http://www.webupd8.org/2012/11/how-to-use-netflix-in-ubuntu-through.html) desarrollado por [Erich Hoover](https://plus.google.com/+ErichHoover).

Esta herramienta Instala una versión de wine (mantenida por el autor) y un conjunto de scripts que se encargan de instalar Firefox (win32), Silverlight y mantenerlos actualizados.

Existen maneras sencillas de instalar Netflix-Desktop para Ubuntu, Arch y Fedora.

### Ubuntu 12.04 en adelante

* Abre una terminal
* Agrega el repositorio del autor en Launchpad ejecutando ``sudo apt-add-repository ppa:ehoover/compholio``
* Actualiza tu información de los repositorios ejecutando ``sudo apt-get update``
* Instala Netflix-Desktop ejecutando ``sudo apt-get install netflix-desktop``
* Una vez que termine tendrás una archivo ``netflix-desktop.desktop`` en ``/usr/share/applications`` por lo cual la mayoría de aplicaciones de menu deberían mostrar el atajo de ejecución de Netflix-Desktop
* Ejecútalo y permite que instale ``Wine Mono Installer`` y ``Wine Gecko Installer``
* Una vez que termine te aparecerá en pantalla completa la página de Netflix y podrás utilizarlo sin problema.

### Arch Linux

* No he intentado personalmente en Arch así que estas instrucciones son para ejecutarlas bajo tu propio riesgo.
* Debes tener habilitado el repositorio AUR.
* La ubición del paquete es [esta](https://aur.archlinux.org/packages/netflix-desktop/).

### Fedora (Disculpa pero desconozco desde que versión)

* No he intentado personalmente el proceso por lo cual prefiero dejar el [link](http://forums.fedoraforum.org/showthread.php?t=286230) a las instrucciones y que el interesado tome la decisión si desea o no seguirlas.

## Ejecutar Silverlight desde cualquier navegador que soporte [NPAPI](http://en.wikipedia.org/wiki/NPAPI).

Para este caso existe [Pipelight](https://launchpad.net/pipelight), los mismos desarrolladores pensaron en esta herramienta como una solución para ejecutar Flash, Silverlight y Shockwave Player de Windows en Linux a través de NPAPI.

Actualmente soportan las siguientes distros de manera sencilla:

* [Ubuntu](http://fds-team.de/cms/pipelight-installation.html#section_1_1)
* [Arch Linux](http://fds-team.de/cms/pipelight-installation.html#section_1_2)
* [Debian Wheezy/Jessie/Sid](http://fds-team.de/cms/pipelight-installation.html#section_1_3)
* [openSUSE](http://fds-team.de/cms/pipelight-installation.html#section_1_4)
* [AVLinux](http://fds-team.de/cms/pipelight-installation.html#section_1_6)
* [SteamOS](http://fds-team.de/cms/pipelight-installation.html#section_1_8)

Y también si quieres compilar la herramienta por tu cuenta lo puedes hacer siguiendo estas [instrucciones](http://fds-team.de/cms/pipelight-installation.html#section_1_9).

### Como utilizarlo en Ubuntu 12.04 en adelante

* Abre una terminal
* Agrega el repositorio del autor en Launchpad ejecutando ``sudo apt-add-repository ppa:pipelight/stable``
* Actualiza tu información de los repositorios ejecutando ``sudo apt-get update``
* Si solo te interesa utilizar Silverlight ejecuta ``sudo apt-get install pipelight``
* Si te interesa utilizar otros plugins ejecuta ``sudo apt-get install pipelight-multi`` y para activarlos (ejemplo) ejecuta ``sudo pipelight-plugin --enable silverlight``.
* Algunos sitios, como Netflix, no te permitirán utilizar los plugins debido al 'User Agent' del navegador por lo cual tendrás que cambiarlo.
    * En Firefox puedes utilizar [UAControl](https://addons.mozilla.org/en-us/firefox/addon/uacontrol/) ó [User Agent Overrider](https://addons.mozilla.org/en-US/firefox/addon/user-agent-overrider/) con los siguientes datos:
        * Mozilla/5.0 (Windows NT 6.1; WOW64; rv:15.0) Gecko/20120427 Firefox/15.0a1
        * Mozilla/5.0 (Windows NT 6.1; WOW64; rv:22.0) Gecko/20100101 Firefox/22.0
        * Mozilla/5.0 (Windows NT 6.1; rv:23.0) Gecko/20131011 Firefox/23.0
    * En Chrome puedes instalar [User Agent Switcher](https://chrome.google.com/webstore/detail/user-agent-switcher-for-c/djflhoibgkdhkhhcedjiklpkjnoahfmg) y escoger Windows Firefox 15 y es todo.

La imagen es original de http://www.iheartubuntu.com/2012/11/ppa-for-netflix-desktop-app.html

# Colaboradores de esta ficha

[Ricardo Rosales](https://github.com/missingcharacter)
