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
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="info1">{{ link.info1 }}</div>
      <div class="info2">{{ link.info2 }}</div>
      </div>
    <div class="links">
      {% if link.link %} 
      <a href="{{ link.link }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:15px;">LINK</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
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
