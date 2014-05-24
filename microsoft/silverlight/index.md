---
title: Microsoft Silverlight
layout: plataforma

f_creacion: 2014-05-22
f_revision: 2014-05-22

liga: http://www.microsoft.com/silverlight/

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

funciona_blah: no
funciona_fedora: no

funciona_parabola: no
funciona_archlinux: no
---

# Descripción de la plataforma

Según [la página de Silverlight en Wikipedia](https://es.wikipedia.org/wiki/Silverlight):

> Microsoft Silverlight es una estructura para aplicaciones Web que agrega nuevas funciones multimedia como la reproducción de vídeos, gráficos vectoriales, animaciones e interactividad, en forma similar a lo que hace Adobe Flash."

# Problemas de Microsoft Silverlight con Software Libre

# Cómo corregirlo

# Rodeos y alternativas

## Pipelight

Pipelight es actualmente la mejor solución *técnica* al problema Silverlight. Si bien no remplaza a Silverlight, permite instalar el *plug-in* dentro de una envoltura NPAPI y ser ejecutado bajo Wine dentro de un navegador.

Si bien Pipelight es Software Libre, Pipelight instala Silverlight. Por eso Pipelight se considera sólo como una solución *técnica* pues, si bien habilita el funcionamiento de Silverlight, se violan los preceptos de libertad del usuario al forzarlo a instalar software privativo.

Los detalles de esta tecnología y sus procedimientos de instalación están disponibles en [la ficha de Pipelight](/pipelight/).

## Moonlight (no recomendado)

Moonlight era una implementación abierta de la especificación de Silverlight 1 y 2. El proyecto fue abandonado debido a la pobre adopción de Silverlight y las restricciones impuestas por Microsoft sobre su utilidad en el escritorio.

Según Wikipedia, el proyecto estuvo oficialmente soportado por Microsoft, que permitió acceso a Novell y al equipo de desarrollo de Mono a las especificaciones de Silverlight. Sin embargo, este acceso imponía limitaciones que hacían la implementación incompatible con las licencias clásicas del Software Libre y el de Código Abierto.

No se recomienda el uso de Moonlight por sus limitaciones técnicas.

## Usar una máquina virtual

Como última alternativa, se puede visitar la página en cuestión desde una [máquina virtual corriendo Windows](/virtualbox/windows/).

# Servicios populares que hacen uso de Microsoft Silverlight

* [Netflix](/netflix/)

# Cómo mejorar esta ficha

* Complementar la información faltante en las diferentes secciones.
