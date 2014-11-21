---
title: Tecnologías incompatibles
layout: front

extra_breadcrumb: 'Tecnologías incompatibles'
---

# Tecnologías incompatibles

Las siguientes tecnologías presentan incomopatibilidades con Software Libre.

<!-- Listado de páginas  -->
<ul class="listado-plataformas">
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
	{% if page.layout == 'problema' %}
	<li class="listado-problema-entrada">
		<a href="{{ site.url }}{{ page.url }}">
			{{ page.title }}
		</a>
	</li>
	{% endif %}
{% endfor %}
</ul>

Los motivos pueden variar por caso, pero incluyen:

* Falta de una implementación libre de la tecnología.

* Falta de especificaciones abiertas que permitan una implementación libre y
  100% funcional.

* Restricciones legales para la implementación libre de la tecnología.
