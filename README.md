Alternus
========

*Alternus* es una colección de fichas descriptivas de alternativas y
soluciones a servicios y trámites incompatibles con Software Libre para la
ciudad de Tijuana, México.

Ejemplos del propósito de *Alternus*:

* Un usuario quiere comenzar a usar Ubuntu pero su banca en línea usa
  un control ActiveX. En *Alternus* podemos documentar la opción de usar
  Virtualbox que, aunque dista de ser lo óptimo, le funcionaría. Esto
  serviría como referencia a otros usuarios.

* Un usuario de Fedora logra hacer funcionar su proveedor de video bajo
  demanda (tal vez uno que empieza con *N* y termina con *etflix*) con
  openSUSE. El usuario *forkea* *Alternus* y nos manda una ficha
  técnica nueva para documentarla para beneficio del resto de la comunidad.

* Un usuario de FreeBSD no puede tramitar su inscripción en línea
  porque el botón de *Enviar* sólo funciona con Internet Explorer. En
  el sitio observa que otros han tenido éxito a partir de la versión
  22 de Firefox bajo Debian Sid. Esto le da información para intentar
  cosas: probar Firefox 22 bajo FreeBSD; instalar Debian Sid en
  Virtualbox, etc.

* El sitio de la Secretaría de *algo*, ofrece una aplicación
  para descargar, pero es un .exe para Win32. Gracias a
  *Alternus* se entera que alguien lo ha hecho funcionar con Wine
  usando versiones específicas de ciertos DLL de Microsoft. Al proveedor
  le sirve esta información para probar la compatibilidad del programa
  al ser ejecutado bajo Wine y, aunque el soporte no es oficial, el
  programa funciona mejor.

* El *otro* sitio de la Secretaría de *algo*, ofrece una
  aplicación, otro .exe y sirve para hacer algunos cálculos. El cálculo es
  relativamente simple. Alguien del público logra implementar el mismo
  cálculo en una hoja de LibreOffice Calc. La hoja se podría publicar en
  *Alternus*.

* Un ISP recibe algunos reportes de que gente con Linux no puede
  entrar a la consulta de estado de servicio. El ISP considera que, al
  ser pocos los usuarios afectados, han decidido no darle soporte a
  corto plazo de manera oficial, es decir, no quieren implementar
  procedimientos, cambios a sistema, etc. "sólo para unos cuántos".
  Sin embargo, alguno de sus ingenieros lo hizo funcionar y le permiten
  publicar el procedimiento en Alternus aunque el soporte no sea oficial
  y ellos sigan diciendo que no soportan Linux. Incluso, tal vez a ese
  ingeniero le permitan darle mantenimiento a la ficha técnica
  mientras no lo haga bajo el nombre de la empresa.

¿Qué necesita el proyecto *Alternus*?
=====================================

* Difusión del proyecto: pasar la voz para que la gente se entere,
  pero la mejor manera de difundir el proyecto es colaborando y
  haciendo un sitio tan completo que la gente hable bien de él por
  gusto.

* Contenido: reporte de fichas, revisión, validación de que los datos
  sean verdaderos y actuales, etc. Más que la apariencia, lo más importante
  es **el contenido** del sitio.

* Evolucionar y mejorar. Todo es perfectible. Al ser un proyecto
  abierto y libre, cualquiera puede ver el código, aportar, corregir,
  etc.

Por qué es fácil participar
===========================

*Alternus* es un sitio estático escrito en Markdown, generado con
Jekyll/Liquid y publicado en Github.

* Las fichas están hechas en Markdown sobre YAML. Al usar YAML, se puede
  tener una ficha decente simplemente declarando algunos encabezados. Al
  usar Markdown, no se requiere de conocimiento de HTML para ofrecer
  contenido. Prácticamente es un archivo de texto plano.

* Al usar Jekyll, no requiere de programación *server-side*. Requiere
  de un poco de Jekyll y Liquid, pero sólo para modificar la estructura del
  sitio, más no para ofrecer fichas. Aún así, es mínimo comparado con PHP,
  Python, Ruby y sus respectivos frameworks.

* Está manejado en Git, lo que permite que cualquier persona pueda
  clonar el código, levantar el sitio en su PC con un esfuerzo mínimo
  (jekyll serve) y probar antes de enviar sus cambios.

* Al estar hospedado en Github, se puede manejar el branch gh-pages y
  mostrar los cambios en público antes de enviárnoslos.

Cómo participar
===============

Si tienes cuenta en Github sólo dale *Fork*. Si no, usando Git clónalo con:

	git clone git@github.com:alvarezp/alternus.gultij.org.git

* La discusión y propuesta de páginas nuevas, así como modificaciones
  a documentos existentes se pueden realizar por medio de los
  *Issues* de Github.

* Si ya sabes manejar Git, directamente manda un pull-request (sea
  por Github o por correo) con tus cambios propuestos. Éstos se revisarán
  antes de ser aceptados, así que es posible que se necesiten algunos
  cambios previos a su aceptación final. Si no le tienes confianza a
  alvarezp, mándaselo a dualbus, y viceversa. Después de todo, es Git.

Alcance del proyecto
====================

El alcance central abarca páginas y software de proveedores para el
público en general como transacciones, trámites y consultas en
sitios de gobierno, bancos en línea, universidades públicas y
privadas, proveedores de telefonía e Internet, empresas locales, etc.

También los sitios a nivel nacional y mundial son aceptados, mientras
sean de interés, al menos, para el público tijuanense.

