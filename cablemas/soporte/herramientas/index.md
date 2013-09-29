---
title: Cablemás
layout: ficha

f_creacion: 2013-09-28
f_revision: 2013-09-28

liga: http://personal.cablemas.com/soportecablemas/soporte/herramientas.html

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

funciona_blah: no
funciona_fedora: no

funciona_parabola: no
funciona_archlinux: no
---

# Descripción de la página

Herramientas de soporte de redes de Cablemás. Las usan para facilitar que el usuario tenga acceso a ping y traceroute.

# Por qué no funcionan con Software Libre

Las herramientas son scripts HTA que sólo son reconocidos por Internet Explorer y, por lo tanto, sólo bajo Windows.

Además, los scripts HTA están programados en VBScript, que sólo trabaja en Internet Explorer.

Encima, esos scripts de VBScript internamente realizan llamadas a las instrucciones `ping` y `tracert` usando su sintaxis específica y por medio de cmd.exe.

# Cómo corregirlo

La dependencia en Windows y sus mecanismos internos es muy profunda. La única manera sería reprogramar todo usando JavaScript. Desafortunadamente ejecutar instrucciones de una PC desde una página Web es inseguro, por lo que sólo cuando JavaScript soporte ping y traceroute en su API esto será posible.

La MEJOR manera sería enlazar al usuario a herramientas ping y traceroute que estuvieran disponibles en una página de su módem.

# Rodeos y alternativas

Existen algunas alternativas. No olvides indicarle a Cablemás que debido a que no usas Windows no puedes usar su herramienta, y que por lo tanto usarás uno de los rodeos, y cuál de todos estás usando.

## Ping y traceroute desde la terminal

Cuando te pidan usar la herramienta ping, entra a una terminal y usa la instrucción `ping`. Si te piden hacer ping a la dirección 4.2.2.2, usa la instrucción `ping 4.2.2.2`. Deja pasar unos cuantos pings (digamos, 5) y cancela con Ctrl+C.

Cuando te pidan usar la herramienta traceroute, entra a una terminal y usa la instrucción `traceroute`.

## GNOME Nettool

GNOME Nettool es una suite de herramientas de red.

Búscala en tu distribución. Por ejemplo:

* Bajo Debian Sid ya vienen instaladas y están disponibles en System Tools » Nettool. Si no, el paquete se llama gnome-nettool.

* Bajo Fedora...

* Bajo Arch Linux...

# Ideas para mejorar esta página

Incluir screenshots de la página funcionando bajo Windows según la intención original de Cablemás.

Incluir screenshots y ejemplos de cada uno de los rodeos, para que si un agente de Cablemás opta por consultar esta página le sirva para guiar al usuario.
