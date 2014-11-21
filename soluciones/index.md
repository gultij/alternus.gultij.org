---
title: Soluciones
layout: front

extra_breadcrumb: 'Soluciones'
---

# Soluciones

El siguiente es un listado de posibles soluciones definitivas a los problemas
presentados por los servicios incompatibles.

Al adoptar este tipo de soluciones, el desarrollador apuesta por mejorar la
interoperabilidad de su servicio. Esto permite un mayor alcance de usuarios
beneficiados.

<!-- Listado de páginas  -->
<ul class="listado-solucion">
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
	{% if page.layout == 'solucion' %}
	<li class="listado-solucion-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>


