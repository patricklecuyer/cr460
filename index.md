---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---
<ul>
  {% for slide in site.slides %}
  <li>
    <h1>
      <a href="{{ slide.url | prepend: site.baseurl | remove: 'index' }}">
        {{ slide.title }}
      </a>
    </h1>
    <p> {{ slide.description }}</p>
  </li>
  {% endfor %}
</ul>
