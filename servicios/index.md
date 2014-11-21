---
title: Servicios incompatibles
layout: front

extra_breadcrumb: ['Servicios incompatibles']
---

# Servicios incompatibles con Software Libre

Los siguientes servicios tienen algún tipo de incompatibilidad con Software
Libre, lo que orilla a los usuarios a utilizar software privativo, comprar
licencias innecesariamente.

Para cada servicio se ofrecen alternativas al alcance de los usuarios y se
detallan las soluciones definitivas que los desarrolladores podrían adoptar.

<!-- Listado de páginas  -->
<ul class="listado-servicios">
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
	{% if page.layout == 'servicio' %}
	<li class="listado-servicios-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>


