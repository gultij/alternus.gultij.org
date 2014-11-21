---
title: Pipelight
layout: alternativa

f_creacion: 2014-05-21
f_revision: 2014-05-21

resumen: Pipelight es un <span class="extranjerismo">plug-in</span> especial que permite el uso en navegadores en Linux de <span class="extranjerismo">plug-ins</span> exclusivos de Windows.

liga: http://fds-team.de/cms/articles/2013-08/pipelight-using-silverlight-in-linux-browsers.html

proveedor: FDS-Team

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no
---

# Pipelight

[*Pipelight*](http://fds-team.de/cms/articles/2013-08/pipelight-using-silverlight-in-linux-browsers.html) es un *plug-in* especial que permite el uso en navegadores en Linux de *plug-ins* exclusivos de Windows. Por ejemplo, es la solución técnica por excelencia a la necesidad de ejecutar Microsoft Silverlight en Linux.

Funciona permitiendo la instalación del *plug-in* problemático dentro de una envoltura NPAPI y ser ejecutado bajo Wine dentro de un navegador.

Si bien Pipelight es Software Libre, Pipelight instala Silverlight. Por eso Pipelight se considera sólo como una alternativa o rodeo *meramente técnico* pues, si bien habilita el funcionamiento de Silverlight, se violan los preceptos de libertad del usuario al forzarlo a instalar software privativo.

# Instalación

La instalación de Pipelight varía según la distribución. La página del proyecto ofrece una [lista completa de instrucciones de instalación para diversas distribuciones](http://fds-team.de/cms/pipelight-installation.html).

## Instalación de Pipelight en Ubuntu

	sudo add-apt-repository ppa:pipelight/stable
	sudo aptitude update
	sudo aptitude install --install-recommends pipelight

La instalación fue directa, sin necesidad de realizar ajustes posteriores.

## Instalación de Pipelight en otras distribuciones

Actualmente soportan las siguientes distros de manera sencilla:

* [Ubuntu](http://fds-team.de/cms/pipelight-installation.html#section_1_1)
* [Arch Linux](http://fds-team.de/cms/pipelight-installation.html#section_1_2)
* [Debian Wheezy/Jessie/Sid](http://fds-team.de/cms/pipelight-installation.html#section_1_3)
* [openSUSE](http://fds-team.de/cms/pipelight-installation.html#section_1_4)
* [AVLinux](http://fds-team.de/cms/pipelight-installation.html#section_1_6)
* [SteamOS](http://fds-team.de/cms/pipelight-installation.html#section_1_8)

Todas estas instrucciones provienen de la página [Pipelight - Installation](http://fds-team.de/cms/pipelight-installation.html).

# Colaboradores en esta ficha

[Ricardo Rosales](https://github.com/missingcharacter), [Octavio Alvarez](https://github.com/alvarezp)
