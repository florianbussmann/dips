---
layout: default
---
| Produkt | Preis |
| --- | ---:| {% assign items = site.digistore24 | sort: 'id' | reverse %} {% for product in items limit:30 %}
| [{{ product.title }}]({{ site.baseurl }}{{ product.url }}) | {{ product.price }} | {% endfor %}