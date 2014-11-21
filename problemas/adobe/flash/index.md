---
title: Adobe Flash
layout: problema

f_creacion: 2014-01-10
f_revision: 2014-01-10

resumen: Adobe Flash es una tecnología sin especificaciones abiertas para su libre implementación. Además, Adobe ha cancelado el soporte oficial para Linux.

proveedor: Adobe

liga: http://developer.chrome.com/extensions/npapi.html

alternativas: ['virtualbox/windows', 'gnu/gnash']
soluciones: ['rediseno-html-css']

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

colaboradores: ['ricdros', 'alvarezp']
---

# Detalles

Adobe detuvo el desarrollo del *plug-in* para Linux en 2012, quedando la versión 11.2 como la última desarrollada.

Adobe ha decidido trabajar en conjunto con Google para empaquetar nuevas versiones de flash basadas en 'Pepper Plugin API' ([PPAPI](https://developers.google.com/native-client/pepperc/)).

Como Flash es software propietario no se puede empaquetar y/o distribuir legalmente por nadie más.

# Cómo corregirlo

Desgraciadamente no hay manera de hacerlo debido a que el desarrollo de Flash para Linux solo se hará para Chrome.

# Alternativas

* Utilizar Google Chrome, si te gusta Chromium es muy probable que Google Chrome cumpla con tus expectativas solo toma en cuenta que estarás usando Software Propietario.
* Cambiar de navegador, Firefox seguirá soportando NPAPI (hasta el momento de esta publicación) así que podrás seguir utilizando Flash 11.2 en él y otros navegadores que soporten NPAPI.

