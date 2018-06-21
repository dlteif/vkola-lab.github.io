---
title: "Sanders Lab - Publications"
layout: gridlay
excerpt: "Sanders Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

---

## Featured

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="row">
 	<img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="25%" style="float: left" />
  <p><a href="{{ publi.link.url }}">{{ publi.title }}</a></p>
  <p>{{ publi.link.display }}</p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

---

<div>
## Full List

For a full list, please go to [Google Scholar](https://scholar.google.ch/citations?user=TqxYWZsAAAAJ), [Pubmed](https://www.ncbi.nlm.nih.gov/pubmed?term=Sanders%20SJ%5BAuthor%5D)
<br><br><br>

</div>
