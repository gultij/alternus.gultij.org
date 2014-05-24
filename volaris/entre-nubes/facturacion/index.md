---
title: Volaris&#58; página de facturación de servicio "Entre Nubes"
layout: servicio

f_creacion: 2014-05-21
f_revision: 2014-05-21

liga: http://e-facpos.com/#/GRO

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

funciona_blah: no
funciona_fedora: no

funciona_parabola: no
funciona_archlinux: no
---


# Descripción y alcance de esta ficha

Se refiere únicamente a la *herramienta de facturación* del servicio *Entre Nubes* de Volaris. *Entre Nubes* es un servicio de venta de alimentos que se ofrece durante sus vuelos.

De la misma manera que en el resto de México, para obtener la factura correspondiente a un pago realizado sobre este servicio, es necesario ingresar a una dirección Web e ingresar los datos del recibo y el RFC. En el caso de Entre Nubes de Volaris, la dirección Web para facturar es [http://e-facpos.com/#/GRO](http://e-facpos.com/#/GRO).

Sin embargo esta página no es compatible con Software Libre.

# Por qué no funciona con Software Libre

La herramienta está programada en Microsoft Silverlight y requiere su *plug-in* para funcionar. Microsoft sólo ofrece el *plug-in* para Windows y Mac OS. Otros sistemas operativos quedan excluidos del uso de esta tecnología.

Nota: Si bien existió un proyecto de implementación alterna, Moonlight, [su desarrollo se detuvo](http://lists.ximian.com/pipermail/moonlight-list/2011-December/001392.html). Según se explica, inicialmente había especificaciones abiertas para Moonlight, pero en versiones más recientes, las especificaciones no fueron totalmente liberadas.

Por lo anterior, Silverlight no debe ser usado para desarrollar herramientas Web multiplataforma.

# Al proveedor: cómo corregir

Puesto que sólo se ofrece el *plug-in* de Silverlight para Windows y Mac OS, y que no hay especificaciones abiertas para su libre implementación, la única solución es migrar la aplicación a una plataforma interoperable.

## Migrar la aplicación a HTML 5 (recomendado)

Al ser un protocolo estándar, abierto y de libre implementación, la responsabilidad de la implementación de HTML 5 queda a cargo de cada sistema operativo. En este momento existen múltiples navegadores multiplataforma que soportan HTML 5 en buena medida.

La aplicación puede ser programada bajo cualquier herramienta o ambiente de desarrollo, incluso privativo. Lo importante es que la interfaz entre la aplicación y el navegador sólo utilice HTML 5 y las tecnologías relacionadas (CSS, DOM estándar y JavaScript).

# Al usuario: alternativas disponibles y soluciones temporales

## Pipelight (solución temporal)

[*Pipelight*](/pipelight/) es un *plug-in* especial que permite el uso en navegadores en Linux de *plug-ins* exclusivos de Windows.

Esta alternativa fue verificada bajo el siguiente ambiente:

* Ubuntu 13.04
* Firefox 26.0
* Pipelight 0.2.4.2~ubuntu13.04.1
* Wine Compholio 1.7.11~ubuntu13.04.1.

Los detalles de esta tecnología y sus procedimientos de instalación están disponibles en [la ficha de Pipelight](/pipelight/).

## Correr sobre una máquina virtual

(Pendiente por documentar)

# Colaborador(es) de esta ficha

[Octavio Alvarez](https://github.com/alvarezp)
