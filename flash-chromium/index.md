---
title: Chromium y Flash
layout: plataforma

f_creacion: 2014-01-10
f_revision: 2014-01-10

liga: http://developer.chrome.com/extensions/npapi.html

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

funciona_blah: no
funciona_fedora: no

funciona_parabola: no
funciona_archlinux: no
---

# Descripción de la página

A partir de Abril de 2014 Google dejará de soportar 'Netscape Plugin API' ([NPAPI](http://en.wikipedia.org/wiki/NPAPI)).

# Por que no funcionan con Software Libre

Adobe detuvo el desarrollo del plugin para linux en 2012, siendo su última versión 11.2 desarrollada con base a NPAPI.

Adobe ha decidido trabajar en conjunto con Google para empaquetar nuevas versiones de flash basadas en  'Pepper Plugin API' ([PPAPI](https://developers.google.com/native-client/pepperc/)).

Como flash es software propietario no se puede empaquetar y/o distribuir legalmente por nadie más.

# Cómo corregirlo

Desgraciadamente no hay manera de hacerlo debido a que el desarrollo de flash para linux solo se hará para Chrome.

# Rodeos y alternativas

* Utilizar Google Chrome, si te gusta Chromium es muy probable que Google Chrome cumpla con tus expectativas solo toma en cuenta que estarás usando Software Propietario.
* Cambiar de navegador, Firefox seguirá soportando NPAPI (hasta el momento de esta publicación) así que podrás seguir utilizando Flash 11.2 en él y otros navegadores que soporten NPAPI.
