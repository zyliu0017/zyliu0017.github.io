<h2 id="projects" style="margin: 2px 0px -15px;">Projects</h2>

<div class="projects">
<ol class="bibliography">

{% for link in site.data.projects.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative; padding-right: 15px; padding-left: 20px;  margin-top: 10px;">
      <div class="title" style="font-size: 20px; color: blue;">{{ link.title }}</div>
      <div class="info1">{{ link.info1 }}</div>
      <div class="info2">{{ link.info2 }}</div>
    <div class="links">
      {% if link.notes %} 
      <strong><em>{{ link.notes }}</em></strong>
      {% endif %}
      {% if link.Link %} 
      <a href="{{ link.Link }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:15px;">LINK</a><br>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>
