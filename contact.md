---
layout: page
title: Contact
permalink: /contact/
---

<p>
  Vous pouvez nous contacter par e-mail : 
  <a href="mailto:{{ site.email }}">
    <i class="fa fa-envelope-o"></i>
    <span class="username">{{ site.email }}</span>
  </a>
</p>

<hr>

<p>
  Vous pouvez également utiliser les réseaux sociaux :
  <ul class="social-media-list">
    {% for social in site.social %}
      {% if social.url != null %}
      <li>
        <a href="{{ social.url }}" title="{{ social.desc }}">
          <i class="fa fa-{{ social.icon }}"></i>
          <span class="username">{% if social.username %}{{ social.username }}{% else %}{{ social.name }}{% endif %}</span>
        </a>
      </li>
      {% endif %}
    {% endfor %}
  </ul>
</p>

<hr>
