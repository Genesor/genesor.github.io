---
layout: page
title: "Talks"
---

{% for talk in site.data.talks %}
<div class="post-preview">
  <a href="{{talk.url}}" target="_blank">
      <h2 class="post-title">{{ talk.title }}
      </h2>
      <h3 class="post-subtitle">
        {{talk.event}} in {{talk.place}}<br>
        {% if talk.speakers %}
          <span class='small-text'>
              Done with
              {% for speaker in talk.speakers %}
                {{speaker}}
              {% endfor %}
          </span><br>
        {% endif %}
        <b class='small-text'>{{talk.date}}</b>
      </h3>
  </a>
</div>
<hr>
{% endfor %}