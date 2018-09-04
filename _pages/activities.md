---
title: "ESMG-MX: Activities"
layout: gridlay
excerpt: "ESMG-MX -- Activities"
sitemap: false
permalink: /activities/
---


# Activities
The ESMG-MX conducts courses, seminars, documentation and publication of scientific articles. In addition, it proposes methods, models and software aimed at researchers and students interested in earth-science modeling.

## Education

{% assign number_printed = 0 %}
{% for publi in site.data.activities-education %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
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

## Knowledge

{% assign number_printed = 0 %}
{% for publi in site.data.activities-knowledge %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
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

<div>
         <iframe src="https://calendar.google.com/calendar/embed?title=Eventos%20ESMG%20MX&amp;showTitle=0&amp;showNav=0&amp;showPrint=0&amp;showTabs=0&amp;height=468&amp;wkst=1&amp;bgcolor=%23ffffff&amp;src=esmg.mx%40gmail.com&amp;color=%23BE6D00&amp;ctz=America%2FMexico_City" style="border:solid 1px #777" width="700" height="300" frameborder="0" scrolling="no"></iframe>
         </div>

<p> &nbsp; </p>

