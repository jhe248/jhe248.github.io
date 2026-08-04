---
permalink: /cv/
title: "CV"
layout: default
author_profile: false
redirect_from:
  - /resume
---

<div class="home-wrapper">
  <h1 class="page__title">CV</h1>

  <div class="page__content">

    <h2>Education</h2>
    <ul>
      <li>Ph.D. in Earth and Environment, Boston University, in progress</li>
    </ul>

    <h2>Experience</h2>
    <ul>
      <li>Add a position here.</li>
    </ul>

    <h2>Skills</h2>
    <ul>
      <li>Add a skill here.</li>
    </ul>

    <h2>Publications</h2>
    {% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
    {% if sorted_pubs.size > 0 %}
      {% for pub in sorted_pubs %}
      <div class="home-entry">
        <p>
          {% if pub.paperurl %}<a href="{{ pub.paperurl }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}.
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
