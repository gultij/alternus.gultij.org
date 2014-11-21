---
title: Microsoft Silverlight
layout: problema

f_creacion: 2014-05-22
f_revision: 2014-05-22

alternativas: ['fds-team/pipelight', 'virtualbox/windows']
soluciones: ['rediseno-html-css']

liga: http://www.microsoft.com/silverlight/

proveedor: Microsoft

resumen: Los sitios Web desarrollados con Microsoft Silverlight requieren un <span class="extranjerismo">plug-in</span> para funcionar. Microsoft sólo ofrece el <span class="extranjerismo">plug-in</span> para Microsoft Windows y Apple OS X. Otros sistemas operativos quedan excluidos del uso de esta tecnología. Microsoft no ofrece documentación suficiente para que un equipo independiente pueda preparar una implementación 100% funcional.

colaboradores: ['ricdros', 'alvarezp']
---

# Descripción de la plataforma

Según [la página de Silverlight en Wikipedia](https://es.wikipedia.org/wiki/Silverlight):

> Microsoft Silverlight es una estructura para aplicaciones Web que agrega nuevas funciones multimedia como la reproducción de vídeos, gráficos vectoriales, animaciones e interactividad, en forma similar a lo que hace Adobe Flash."

# Problemas de Microsoft Silverlight con Software Libre

{{ page.resumen }}

Nota: Si bien existió un proyecto de implementación alterna, Moonlight, [su desarrollo se detuvo](http://lists.ximian.com/pipermail/moonlight-list/2011-December/001392.html). Según se explica, inicialmente había especificaciones abiertas para Moonlight, pero en versiones más recientes, las especificaciones no fueron totalmente liberadas.

Considerando que existen otras herramientas para el desarrollo Web con contenido multimedia que resultan en sitios apropiadamente interoperables, Microsoft Silverlight no debe ser usado para desarrollar herramientas Web multiplataforma.

## Moonlight (no recomendado)

Moonlight era una implementación abierta de la especificación de Silverlight 1 y 2. El proyecto fue abandonado debido a la pobre adopción de Silverlight y las restricciones impuestas por Microsoft sobre su utilidad en el escritorio.

Según Wikipedia, el proyecto estuvo oficialmente soportado por Microsoft, que permitió acceso a Novell y al equipo de desarrollo de Mono a las especificaciones de Silverlight. Sin embargo, este acceso imponía limitaciones que hacían la implementación incompatible con las licencias clásicas del Software Libre y el de Código Abierto.

Por estas limitaciones no se recomienda el uso de Moonlight.

