## <i class="fa fa-chevron-right"></i> {{ name }}
<div class="well" style="padding:5px">
<div class="media">
<div class="media-left media-middle col-xs-1 col-sm-1 col-md-1 col-lg-1">
<img class="media-object img-rounded" style="width:2em" src="/images/notion.png" alt="Deatiled Research Overview">
</div>
<h4 class="media-heading"><a href="https://gjchen.notion.site/" target="_blank">Research Overview</a>
</h4>
<div class="media-body media-middle">
<p style="margin:0">
<a href="https://gjchen.notion.site/" target="_blank">
To learn more about my research and its direction, be sure to click this link for a detailed document with rich text and images.
</a>
</p>
</div>
</div>
</div>
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


