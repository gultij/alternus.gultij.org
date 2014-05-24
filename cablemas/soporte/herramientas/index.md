---
title: Cablemás&#58; página de herramientas de soporte
layout: servicio

f_creacion: 2013-09-28
f_revision: 2013-09-29

liga: http://personal.cablemas.com/soportecablemas/soporte/herramientas.html

funciona_trisquel: no
funciona_debian: no
funciona_ubuntu: no

funciona_blah: no
funciona_fedora: no

funciona_parabola: no
funciona_archlinux: no
---

# Descripción y alcance de esta ficha

Se refiere sólo a la página de herramientas de soporte de Cablemás. Es una sección de la página de Soporte que usan para facilitarle herramientas de diagnóstico al usuario final, de modo que disponga de fácil acceso a un *ping* y *traceroute* y pueda enviar los resultados.

# Por qué no funcionan con Software Libre

Las herramientas son scripts [HTA](https://es.wikipedia.org/wiki/Aplicaciones_en_HTML) que sólo son reconocidos por Internet Explorer y, por lo tanto, sólo bajo Windows. Estos HTA están programados en VBScript, que sólo trabaja en Internet Explorer.

Estos scripts internamente realizan llamadas a las instrucciones `ping` y `tracert`, características de Windows. En Linux no se llama `tracert` sino `traceroute`.

# Alternativas

Existen algunas alternativas para poder realizar el procedimiento de soporte que solicite el proveedor.

## Ping y traceroute desde la terminal

La mayoría de las distribuciones de Linux y BSD incluyen las herramientas `ping` y `traceroute` (a diferencia de en Windows donde esta última se llama `tracert`). Estas herramientas se usan desde la terminal, así que el primer paso es abrir una terminal.

A modo de ejemplo se menciona *4.2.2.2* como dirección de destino. Para hacer 5 pings se usa `ping -n 5 4.2.2.2`. Windows hace por defecto 4 pings, el equivalente de `ping -n 4 4.2.2.2`. Si uno no especifica *-n 5*, `ping` continuará indefinidamente hasta que uno cancele con Ctrl+C.

Si le piden a uno usar la herramienta traceroute, basta con entrar a una terminal y usar la instrucción `traceroute` de la misma manera: `traceroute 4.2.2.2`. Traceroute tarda en completarse por la *resolución de nombres*. La resolución de nombres puede evitarse con la opción -n: `traceroute -n 4.2.2.2`, pero arroja sólo direcciones IP en lugar de nombres de host.

OJO: hay una diferencia entre Windows y Linux con el traceroute. Windows realiza el traceroute usando internamente ICMP (algo como un ping) mientras que Linux lo hace por medio de UDP, por lo que los resultados pueden variar. Para emular el mismo traceroute que Windows, se usa la opción -I: `traceroute -I 4.2.2.2` pero se requiere estar como el usuario *root*.

## GNOME Nettool

GNOME Nettool es una suite de herramientas de red.

Búscala en tu distribución. Por ejemplo:

* Bajo Debian Sid ya vienen instaladas y están disponibles en System Tools » Nettool. Si no, el paquete se llama gnome-nettool.

* Bajo Fedora... (si sabes cómo es bajo Fedora, mándanos la información).

* Bajo Arch Linux... (si sabes cómo es bajo Arch Linux, mándanos la información).

* Bajo Ubuntu... (si sabes cómo es bajo Ubuntu, mándanos la información).

## Acceder a las herramientas de Soporte desde una máquina virtual

Como última alternativa, se puede visitar la página de las [herramientas de Soporte de Cablemás]({{page.liga}}) desde una [máquina virtual corriendo Windows](/virtualbox/windows/).

Es importante considerar que la tarjeta de red de la máquina virtual debe estar configurada como *bridge*. De esta manera, la tarjeta de red de la máquina virtual pertenecerá a la misma red que la máquina real y las pruebas serán confiables. Por defecto, Virtualbox configura las tarjetas de red como *NAT*, lo que altera el comportamiento de la tarjeta y puede llevar a la incorrecta interpretación de los resultados e invalidación de las pruebas.

# Ideas para mejorar la compatibilidad con Software Libre

La dependencia en Windows y sus mecanismos internos es muy profunda. La única manera sería reprogramar todo de alguna manera compatible. Esto no es fácil por las implicaciones de seguridad. Posibilidades:

* Un applet de Java. Dista mucho de ser lo ideal, sobre todo porque Java de repente se rompe debido a su conducción por Oracle.

* Que el módem/router incluyera una página con herramientas ping y traceroute sin necesidad de login y que se redirigiera al usuario a estas herramientas que se ejecutarían desde el propio módem/router.

# Cómo mejorar esta ficha

* Incluir pantallazos y ejemplos de las alternativas en acción. Podría servir también para referencia del proveedor, lo mismo que para el usuario.

* Incluir pantallazos de la herramienta funcionando bajo Windows para mostrar de la intención original del proveedor.

* Ofrecer una implementación compatible de la herramienta que pudiera hospedarse en *Alternativas*.

# Colaborador(es) de esta ficha

[Octavio Alvarez](https://github.com/alvarezp)
