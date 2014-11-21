---
title: Usar una máquina virtual con Virtualbox
layout: alternativa

resumen: Es posible instalar Microsoft Windows y otros en una máquina virtual usando Oracle Virtualbox. Aún así se requiere de una licencia válida de los sistemas a instalar.

liga: https://www.virtualbox.org/

proveedor: Oracle
---

# Descripción detallada

Virtualbox es un sistema de virtualización para escritorio disponible bajo la
licencia GNU GPL (Licencia Pública General).

Uno de los sistemas operativos que Virtualbox puede hospedar es Microsoft
Windows.

La primera vez que se *prende* la *máquina virtual* emulada por Virtualbox
se encuentra en blanco, de la misma manera en la que una PC nueva no cuenta
con software. Por esto es necesario llevar a cabo la instalación de Windows
dentro de la máquina virtual.

Es importante considerar que la tarjeta de red de la máquina virtual debe
estar configurada como *bridge*. De esta manera, la tarjeta de red de la
máquina virtual pertenecerá a la misma red que la máquina real y el
comportamiento de la misma será equivalente al de la máquina real.
Por defecto, Virtualbox configura las tarjetas de red como *NAT*, lo que
cambia topología de red.

# Instalación

Virtualbox, al ser Software Libre y ser popular, es común encontrarlo
ya disponible en las distribuciones de Linux.

## Debian y Ubuntu

	apt-get install virtualbox

## Otros sistemas operativos

(Pendiente)


# Consideraciones

Para la instalación legal de Windows dentro de la máquina virtual es necesario
cubrir apropiadamente el licenciamiento del sistema operativo.


# Colaboradores de esta ficha

[Octavio Alvarez](https://github.com/alvarezp)
