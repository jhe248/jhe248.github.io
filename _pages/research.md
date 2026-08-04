---
permalink: /research/
title: "Research"
layout: default
author_profile: false
---

<div class="home-wrapper">
  <h1 class="page__title">Research</h1>

  <div class="page__content">
    <p>
      My research focuses on environmental processes and Earth system science.
      Replace this paragraph with an overview of your research interests.
    </p>

    <h2>Research Themes</h2>
    <p>Describe your first research theme here.</p>

    <h2>Publications</h2>
    {% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
    {% if sorted_pubs.size > 0 %}
      {% for pub in sorted_pubs %}
      <div class="home-entry">
        <p>
          {% if pub.paperurl %}<a href="{{ pub.paperurl }}">{{ pub.title }}</a>{% else %}<a href="{{ base_path }}{{ pub.permalink }}">{{ pub.title }}</a>{% endif %}.
          {% if pub.authors %}{{ pub.authors }}. {% endif %}
          {% if pub.venue %}<em>{{ pub.venue }}</em>{% endif %}{% if pub.date %}, {{ pub.date | date: "%Y" }}{% endif %}.
        </p>
      </div>
      {% endfor %}
    {% else %}
      <p>Publications will appear here.</p>
    {% endif %}

    <h2>Talks</h2>
    {% assign sorted_talks = site.talks | sort: 'date' | reverse %}
    {% if sorted_talks.size > 0 %}
      {% for talk in sorted_talks %}
      <div class="home-entry">
        <p>
          {{ talk.title }}.
          {% if talk.venue %}<em>{{ talk.venue }}</em>{% endif %}{% if talk.location %}, {{ talk.location }}{% endif %}{% if talk.date %}, {{ talk.date | date: "%Y" }}{% endif %}.
        </p>
      </div>
      {% endfor %}
    {% else %}
      <p>Talks will appear here.</p>
    {% endif %}
  </div>
</div>
