---
title: Herramientas de soporte (Cablemás)
layout: servicio

f_creacion: 2013-09-28
f_revision: 2013-09-29

liga: http://personal.cablemas.com/soportecablemas/soporte/herramientas.html

resumen: Las herramientas de soporte técnico de Cablemás están programadas como una "Aplicación HTML" de Microsoft (una Microsoft HTA).

problemas: ['microsoft/hta']
alternativas: ['virtualbox/windows', 'gnome/network']

proveedor: Cablemás

colaboradores: ['alvarezp']
---

# Detalles

Las herramientas de soporte técnico de Cablemás están programadas como una "Aplicación HTML" de Microsoft (una Microsoft HTA). Estas sólo son reconocidas por Internet Explorer y, por lo tanto, sólo bajo Windows.

Se trata de una sección de la página de Soporte usada por el proveedor para facilitar el diagnóstico al usuario final, de modo que disponga de fácil acceso a un *ping* y *traceroute* y enviar los resultados.

## Alternativas

### Ping y traceroute desde la terminal

La mayoría de las distribuciones de Linux y BSD incluyen las herramientas `ping` y `traceroute`. Estas herramientas se usan desde la terminal, así que el primer paso es abrir una terminal.

El representante nos dará una *dirección* para la prueba. En estos ejemplos usaremos *8.8.8.8*, pero también podría ser el nombre de una página.

Si el representante pide un *ping*, usaremos `ping -n 4` en un solo paso:

1. `ping -n 4 8.8.8.8`. Si uno no especifica `-n 4`, se harán *pings* por un tiempo indefinido hasta que uno lo cancele con Ctrl+C.

Si le piden a uno usar la herramienta *traceroute*, se deberá abrir una terminal y seguir dos pasos:

1. Volverse *root* usando `su` o `sudo -s`, según la distribución.

2. Usar la instrucción `traceroute` con la opción `-I` de la misma manera: `traceroute -I 8.8.8.8`. Si *traceroute* tarda en completarse, se debe a la *resolución de nombres*, es normal. Hay que darle tiempo.

Observación: si no es posible volverse *root* para hacer `traceroute -I`, es posible usar `traceroute` sin `-I`, pero los resultados pueden variar ligeramente.

Para enviar los resultados sería necesario hacerlo de forma manual, copiando y pegando los resultados por correo electrónico o algún otro medio.

### Ejecutar las herramientas bajo una máquina virtual con Windows

También es posible instalar Microsoft Windows en una [máquina virtual usando Oracle Virtualbox](/alternativas/virtualbox/windows/). Aún así se requiere de una licencia válida de Windows. Es importante configurar la tarjeta de red como *bridged network* para no alterar el resultado de las pruebas.

### GNOME Network

GNOME Network es un juego de herramientas de diagnóstico de red.

# Soluciones

Por las implicaciones de seguridad, la manera que mejor garantiza la interoperabilidad es la implementación de las herramientas de soporte en el módem/router y desde ahí se realice el diagnóstico. Esto permitiría al usuario contar con una herramienta con funcionalidad independiente del sistema operativo.
