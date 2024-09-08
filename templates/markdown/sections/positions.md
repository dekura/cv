{% extends "section.md" %}

{% block body %}
<table class="table table-hover">
{% for i in items %}
<tr>
  <td style='padding-right:0;'>
    <span class='cvdate'>{{ i.dates }} </span>
    <p markdown="1" style='margin: 0'>
    <img src="{{i.logo}}" alt="Logo" style="border:none;height:1.5rem;margin:0;padding:0">&nbsp;
    <strong>{{ i.place}}</strong> &nbsp;
    <span style="color:grey;">{{ i.title }}</span> \\
    {% if i.inline_detail %}
        <span markdown="1" style="color:grey;font-size:1.3rem;margin: 0">
        {{ i.inline_detail }}
        </span>
    {%- endif -%}
    <span class='cvdate' style="color:grey;font-size:1.3rem;margin: 0">{{ i.location }} </span>
    </p>
    </td>
    </tr>
    {% endfor %}
</table>


{% endblock body %}



