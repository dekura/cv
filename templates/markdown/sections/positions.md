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

<div class="well" style="padding:15px">
<div class="media">
<div class="media-left media-middle col-xs-3 col-sm-2 col-md-1">
<a href="https://ai4eda.github.io/" target="_blank">
    <img class="media-object img-rounded" src="/images/ai4eda.png" alt="AI for EDA">
</a>
</div>
<h4 class="media-heading"><a href="https://ai4eda.github.io/" target="_blank">AI for EDA</a>
<img style="border:none;max-height:.9em;margin:0;padding:0" src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fai4eda.github.io%2F&labelColor=%231863e6&countColor=%23d9e3f0&style=flat-square&labelStyle=upper" />
</h4>
<div class="media-body media-middle">
<p style="margin:0">
I'm also maintaining a curated list of <b>AI for EDA</b> papers. Check it out here:
<a href="https://ai4eda.github.io" target="_blank">Awesome AI for EDA</a>. <br>
The list is under construction and you are welcomed to submit your publications follow
<a href="https://ai4eda.github.io/about/" target="_blank">the instructions</a>.
</p>
</div>
</div>
</div>
{% endblock body %}



