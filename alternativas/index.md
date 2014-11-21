---
title: Alternativas
layout: front

extra_breadcrumb: 'Alternativas'
---

# Alternativas

Las siguientes son alternativas disponibles para los usuarios de Software
Libre:

<!-- Listado de páginas  -->
<ul class="listado-alternativas">
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
	{% if page.layout == 'alternativa' %}
	<li class="listado-alternativas-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>

Algunas de las alternativas no son libres pero permiten sobrellevar el
uso de [servicios incompatibles]({{ site.url }}/servicios/).

La solución definitiva siempre es la interoperabilidad nativa del servicio.
Estas alternativas se consideran *rodeos* (*workarounds*) y podrían presentar
inconvenientes.

Como ejemplo, el [uso de Windows bajo una máquina virtual]({{ site.url }}/alternativas/virtualbox/windows/)
es una alternativa genérica, pero presenta los siguientes inconvenientes para
el usuario:

* El rendimiento de una máquina virtual no es el mismo que el de una
computadora física. Esto es especialmente notorio en servicios de video.

* El usuario se ve obligado a adquirir una licencia de Windows para hacer
uso del servicio problemático.

* Se obliga al usuario a ejecutar código que no puede ser auditable, pues
el código fuente de Microsoft Windows no está disponible al público.

