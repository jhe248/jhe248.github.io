---
permalink: /
layout: default
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<div class="home-wrapper">
  <div class="home-intro">
    <div class="home-text">
      <h1>Jiahang He</h1>
      <p class="subtitle">PhD Student in Earth Environment · Boston University</p>
      <p>
        I am a PhD student in the Department of Earth and Environment at Boston University.
        My research focuses on environmental processes and Earth system science.
      </p>
      <ul class="contact-list" style="margin-top:1em;">
        <li><i class="fas fa-envelope" aria-hidden="true"></i> <a href="mailto:jhhe@bu.edu">jhhe@bu.edu</a></li>
        <li><i class="fab fa-github" aria-hidden="true"></i> <a href="https://github.com/jhe248">github.com/jhe248</a></li>
      </ul>
    </div>
    <div class="home-photo">
      <img src="/images/profile.png" alt="Jiahang He">
    </div>
  </div>

  <div class="home-section">
    <h2>Publications</h2>
    {% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
    {% for pub in sorted_pubs %}
    <div class="home-entry">
      <p>
        {% if pub.paperurl %}<a href="{{ pub.paperurl }}">{{ pub.title }}</a>{% else %}<a href="{{ pub.permalink }}">{{ pub.title }}</a>{% endif %}.
        <em>{{ pub.venue }}</em>{% if pub.date %}, {{ pub.date | date: "%Y" }}{% endif %}.
      </p>
    </div>
    {% endfor %}
  </div>

  <div class="home-section">
    <h2>Talks</h2>
    {% assign sorted_talks = site.talks | sort: 'date' | reverse %}
    {% for talk in sorted_talks %}
    <div class="home-entry">
      <p>
        {{ talk.title }}.
        {% if talk.venue %}<em>{{ talk.venue }}</em>{% endif %}{% if talk.location %}, {{ talk.location }}{% endif %}{% if talk.date %}, {{ talk.date | date: "%Y" }}{% endif %}.
      </p>
    </div>
    {% endfor %}
  </div>
</div>
