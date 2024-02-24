{% extends "section.md" %}

{% block body %}
<div class="well well-sm" style="max-height: 15em; overflow: auto">
<ul class="list-group">
    {% for i in items %}
        <li class="list-group-item col-md-12 col-xs-12 col-sm-12"><span class='col-md-2 col-xs-2'>{{ i.date }}&nbsp;&nbsp;&nbsp;&nbsp;</span>{{ i.info }}</li>
    {% endfor %}
</ul>
</div>
{% endblock body %}
