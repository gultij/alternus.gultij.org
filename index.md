---
title: Bienvenido al proyecto Alternativas
layout: front
---

# ¡Bienvenido al proyecto Alternativas!

Alternativas es una collección de fichas descriptivas con alternativas y rodeos en el uso de sitios y programas oficiales con Software Libre. El sitio tiene varios propósitos:

* Proveer a la comunidad regional de Software Libre información para poder aprovechar los recursos regionales usando Software Libre sin morir en el intento.

* Ofrecer a los proveedores documentación técnica sobre las posibles mejoras a sus sitios en cuanto a su relación con Software Libre. El concepto es que *programar para Software Libre es prácticamente una garantía de portabilidad (incluso para Windows y Mac OS X)*.

* Actualizar el sitio conforme haya mejoras en cada caso, de modo que los usuarios que usan Software Libre puedan considerarlos como una opción comercial.

# Listado de servicios incompatibles con Software Libre

<!-- Listado de páginas  -->
<ul class="listado-servicios">
{% for page in site.pages | sort: 'title' %}
	{% if page.layout == 'servicio' %}
	<li class="listado-servicios-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>

# Listado de plataformas incompatibles con Software Libre

<!-- Listado de páginas  -->
<ul class="listado-plataformas">
{% for page in site.pages | sort: 'title' %}
	{% if page.layout == 'plataforma' %}
	<li class="listado-plataformas-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>

# Listado de rodeos y soluciones alternas

<!-- Listado de páginas  -->
<ul class="listado-alternativas">
{% for page in site.pages | sort: 'title' %}
	{% if page.layout == 'alternativa' %}
	<li class="listado-alternatiass-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>

# ¿Qué necesita el proyecto Alternativas?

* Imagen del sitio

* Difusión del proyecto

* Contenido: reporte de fichas, revisión, validación de que los datos sean verdaderos y actuales, etc.

* Evolucionar y mejorar.

# Cómo participar

Colaborar con el proyecto Alternativas es fácil:

* Su código está escrito en Jekyll y está hospedado en Github. Puedes clonar [el repositorio](http://www.github.com/alvarezp/alternativas.gultij.org/) fácilmente usando:

		git clone git@github.com:alvarezp/alternativas.gultij.org.git

  O bien, si tienes cuenta en Github, sólo dale *Fork*.

* La discusión y propuesta de páginas nuevas, así como modificaciones a documentos existentes se pueden realizar por medio de los *Issues* de Github.

* El sitio tiene ya un ejemplo de una página que no es amigable con el Software Libre, pero ojalá pudiéramos llenarlo de experiencias

* Ojo: si algún sitio funciona muy bien, también hay que ponerlo.

* Hay información paso a paso en [Cómo participar](como-participar), según si cuentas con Git, Github o una u otra versión de Jekyll.

# Alcance del proyecto

El alcance central abarca páginas y software de proveedores para el público en general, como transacciones, trámites y consultas en sitios de gobierno, bancos en línea, universidades públicas y privadas, proveedores de telefonía e Internet, empresas locales, etc.

Si el sitio es meramente publicitario para una empresa privada, no es incluíble. Hay que usar el criterio para que el sitio no se convierta en un repositorio de publicidad. Por eso se le debe dar prioridad a sitios de gobierno y escuelas, así como a trámites problemáticos.

