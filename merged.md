---
layout: minimal
title: Annotation guidelines for pathogenic mechanism corpus for lung disease, IPF
---

<h1 style="font-size:32px">Entities</h1>

Entities and cues will be described below.

{% assign sorted = site.entity | sort: 'order' %}
{% for i in sorted %}
## {{ i.title }}{% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{{ i.content }}
{% endfor %}

<h1 style="font-size:32px">Events</h1>

Phenomena and processes are defined as events in this corpus.
The events will be described below.

{% assign sorted = site.event | sort: 'order' %}
{% for i in sorted %}
## {{ i.title }}{% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% if i.category %}**Category: {{ i.category }}**{% endif %}
{{ i.content }}
{% endfor %}

<h1 style="font-size:32px">Relations</h1>

In addition to the relations between event triggers and their arguments (*Theme*, *Cause*, etc.), which are described above, several types of relations were defined. 

<!--
{% include image.html name="relation-examples.jpg" width="100%" %}
-->

Those relations are defined as follows:

{% assign sorted = site.relation | sort: 'order' %}
{% for i in sorted %}
## {{ i.title }}{% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{{ i.content }}
{% endfor %}

<h1 style="font-size:32px">Attributes</h1>
Attributes indicate the states/characteristics of events or entities.

Those attributes are defined as follows:

{% assign sorted = site.attribute | sort: 'order' %}
{% for i in sorted %}
## {{ i.title }}{% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{{ i.content }}
{% endfor %}
