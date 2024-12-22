---
layout: page
title: Publications
permalink: /publications/
---

# Publications

## Recent Journal Articles

{% for paper in site.data.publications.journal_papers limit:5 %}
- {{ paper.authors }} ({{ paper.year }}). {{ paper.title }}. *{{ paper.journal }}*{% if paper.doi %} [DOI]({{ paper.doi }}){% endif %}
{% endfor %}

[View all journal articles](#journal-articles)

## Recent Conference Papers

{% for paper in site.data.publications.conference_papers limit:5 %}
- {{ paper.authors }} ({{ paper.year }}). {{ paper.title }}. In *{{ paper.conference }}*{% if paper.doi %} [DOI]({{ paper.doi }}){% endif %}
{% endfor %}

[View all conference papers](#conference-papers)

## Journal Articles {#journal-articles}

{% for paper in site.data.publications.journal_papers %}
- {{ paper.authors }} ({{ paper.year }}). {{ paper.title }}. *{{ paper.journal }}*{% if paper.doi %} [DOI]({{ paper.doi }}){% endif %}
{% endfor %}

## Conference Papers {#conference-papers}

{% for paper in site.data.publications.conference_papers %}
- {{ paper.authors }} ({{ paper.year }}). {{ paper.title }}. In *{{ paper.conference }}*{% if paper.doi %} [DOI]({{ paper.doi }}){% endif %}
{% endfor %}

## Preprints

{% for paper in site.data.publications.preprints %}
- {{ paper.authors }} ({{ paper.year }}). {{ paper.title }}. {% if paper.arxiv %}[arXiv]({{ paper.arxiv }}){% endif %}
{% endfor %}