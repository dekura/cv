## <i class="fa fa-chevron-right"></i> {{ name }}

Representative publications that I am a primary author on are
<span style='background-color: #ffffd0'>highlighted.</span>
<br>
[<a href="https://scholar.google.com/citations?user={{ scholar_id }}" target="_blank">Google Scholar</a>; {{ scholar_stats.citations }}+ citations, h-index: {{ scholar_stats.h_index}}+]
[<a href="/data/bibtex/all.bib" download="gjchen.bib">Download bibtex for all publications</a>]
[<a href="https://orcid.org/0000-0001-9457-9583" target="_blank">ORCID</a>]

{% for type_content in content %}

### <i class="fa fa-chevron-right"></i> {{type_content.title}}

{{ type_content.details }}

{% endfor %}
