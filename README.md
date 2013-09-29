¡Bienvenido al proyecto Alternativas!
=====================================

Alternativas es una colección comunitaria de fichas técnicas con soluciones, alternativas y rodeos de compatibilidad entre el Software Libre y el día a día de nuestra ciudad. Por ejemplo:

* Un usuario quiere comenzar a usar Ubuntu pero su banca en línea usa un ActiveX. En *Alternativas* podemos documentar la opción de usar Virtualbox que, aunque dista de ser lo óptimo, le funcionaría.

* Un usuario de Fedora logra hacer funcionar su proveedor de video bajo demanda (uno que empieza con *N* y termina con *etflix*) con openSUSE. El usuario forkea el proyecto y nos manda una ficha técnica nueva para documentarla para el resto de la comunidad.

* Un usuario de FreeBSD no puede tramitar su inscripción en línea porque el botón de *Enviar* sólo funciona con Internet Explorer. En el sitio observa que otros han tenido éxito a partir de la versión 22 de Firefox bajo Debian Sid. Esto le da información para intentar cosas: probar Firefox 22 bajo FreeBSD; instalar Debian Sid en Virtualbox...

* El sitio de la Secretaría de ____________, ofrece una aplicación para descargar, pero es un .exe para Win32. Gracias a *Alternativas* se entera que alguien lo ha hecho funcionar con Wine usando versiones específicas de ciertos DLL de Microsoft.

* El *otro* sitio de la Secretaría de _______________, ofrece una aplicación, otro .exe y sirve para hacer un cálculo. El cálculo es muy simple y alguien implementó una alternativa en una hoja de LibreOffice Calc. La hoja se podría publicar en Alternativas.

* Un ISP recibe algunos reportes de que gente con Linux no puede entrar a la sección de facturación. Como son pocos no piensan darle soporte a corto plazo de manera oficial, es decir, no quieren implementar procedimientos, cambios a sistema, etc. sólo para unos cuantos Linuxeros (así lo ven ellos). Sin embargo, alguno de sus ingenieros lo hizo funcionar y le permiten publicar el procedimiento en Alternativas aunque no sea soporte *oficial* y ellos sigan diciendo que no soportan Linux. Es más, tal vez a ese ingeniero le permitan darle mantenimiento a la ficha técnica mientras no lo haga bajo el nombre de la empresa.

¿Qué necesita el proyecto Alternativas?
=======================================

* Imagen del sitio: se necestan layouts que van en el directorio _layouts de Jekyll.

* Difusión del proyecto: pasar la voz para que la gente se entere, pero la mejor manera de difundir el proyecto es colaborando y haciendo un sitio tan completo que la gente hable bien de él por gusto.

* Contenido: reporte de fichas, revisión, validación de que los datos sean verdaderos y actuales, etc. Más que la apariencia, es **el contenido** lo más importante del sitio.

* Evolucionar y mejorar. Todo es perfectible. Al ser un proyecto abierto y libre, cualquiera puede ver el código, aportar, corregir, etc.

Por qué es fácil participar
===========================

*Alternativas* es un sitio estático escrito en Markdown, generado con Jekyll/Liquid y publicado en Github.

* Al usar Markdown, no se requiere de conocimiento de HTML para ofrecer contenido. Prácticamente es un archivo de texto plano.

* Al usar Jekyll, no requiere de programación *server-side*. Requiere de un poco de Jekyll y Liquid, pero es mínimo comparado con PHP, Python, Ruby y sus respectivos frameworks.

* Está manejado en Git, lo que permite que cualquier persona pueda clonar el código, levantar el sitio en su PC con un esfuerzo mínimo (jekyll --server) y probar antes de enviar los cambios.

* Al estar hospedado en Github, se puede manejar el branch gh-pages y mostrar los cambios en público antes de enviárnoslos.

Cómo participar
===============

Si tienes cuenta en Github sólo dale *Fork*. Si no, usando Git clónalo con:

	git clone git@github.com:alvarezp/alternativas.gultij.org.git

* La discusión y propuesta de páginas nuevas, así como modificaciones a documentos existentes se pueden realizar por medio de los *Issues* de Github.

* Si ya sabes manejar Git, directamente manda un pull-request (sea por Github o por correo) con tus cambios propuestos. No te "agüites" si tu cambio es rechazado la primera vez (o las primeras 5). Si no le tienes confianza a alvarezp, mándaselo a dualbus, y viceversa. Después de todo, es Git.

Alcance del proyecto
====================

El alcance central abarca páginas y software de proveedores para el público en general, como transacciones, trámites y consultas en sitios de gobierno, bancos en línea, universidades públicas y privadas, proveedores de telefonía e Internet, empresas locales, etc.

Si el sitio es meramente publicitario para una empresa privada, no es incluíble. Hay que usar el criterio para que el sitio no se convierta en un repositorio de publicidad. Por eso se le debe dar prioridad a sitios de gobierno y escuelas, así como a trámites problemáticos.
