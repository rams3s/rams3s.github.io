---
title: Projects
menu: true
order: 2
---

<link rel="stylesheet" href="../css/vertical_timeline.css">

* list
{:toc}

{% for category in site.data.projects %}
## {{category.name}}

<section class="cd-timeline js-cd-timeline">
  <div class="cd-timeline__container">
{% for project in category.projects %}
    <div class="cd-timeline__block js-cd-block">
      <div class="cd-timeline__img cd-timeline__img--picture js-cd-img">
        <!-- <img src="img/cd-icon-picture.svg" alt="Picture"> -->
      </div>

      <div class="cd-timeline__content js-cd-content">
        <h2>{{project.name}}</h2>
        {% if project.img %}
        <div class="cd-timeline__content_img">
          <img src="../assets/img/projects/{{project.img}}"/>
        </div>
        {% endif %}
        <p>
        {% if project.platforms %} Platforms: {{project.platforms}} <br/> {% endif %}
        {% if project.engine %} Engine: {{project.engine}} <br/> {% endif %}
        {% if project.publisher %} Publisher: {{project.publisher}} <br/> {% endif %}
        </p>
        {% if project.description %} <p>{{project.description}}</p> {% endif %}
        {% if project.url %}
        <a href="{{ project.url }}" class="cd-timeline__read-more">{{project.url_txt}}</a>
        {% elsif project.external_url %}
        <a href="{{ project.external_url }}" target="_blank" class="cd-timeline__read-more">{{project.url_txt}}</a>
        {% endif %}
        <span class="cd-timeline__date">{{ project.date }}</span>
      </div>
    </div>
{% endfor %}
  </div>
</section>
{% endfor %}

<script src="../js/vertical_timeline.js"></script>