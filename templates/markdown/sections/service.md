{% extends "section.md" %}

{% block body %}

### <i class="fa fa-chevron-right"></i> Paper Review / External Review

<table class="table table-hover">
{% for item in items.main %}
<tr>
  <td style='padding-right:0;'>
  <span class='cvdate'>{{ item.year }}</span>
  {% if item.url %}
     <a href="{{ item.url }}">{{ item.details }}</a>
  {% else %}
      {{item.details }}
  {% endif %}
  {% if item.sub_details %}
  <br><p style="color:grey;font-size:1.2rem">{{ item.sub_details }}</p>
  {% endif %}
  </td>
</tr>
{% endfor %}
</table>


{% endblock body %}
