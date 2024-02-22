---
layout: page
dropdown: true
navbar: false
title: Portfolio
---
<article>
  <h2>EACH PROJECT THING APPEARS HERE</h2>
  {% for project in site.data.portfolio %}
    <h3>
      {{ project.name }}
    </h3>
    <p>
      {{ project.description }}  
    </p>
    <ul>Images
    {% for img in project.images %}
        <li><img src="{{img}}"/></li>
    {% endfor %}
    </ul>
  {% endfor %}
</article>