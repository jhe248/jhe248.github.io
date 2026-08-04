---
permalink: /cv/
title: "Curriculum Vitae"
layout: default
author_profile: false
# Update this whenever you replace files/cv_jiahanghe.pdf. If left blank the
# page falls back to the PDF's timestamp, which on GitHub Pages is the build
# date rather than the date you last edited the CV.
cv_updated: 2026-08-04
redirect_from:
  - /resume
---

{% assign cv = site.static_files | where: "path", "/files/cv_jiahanghe.pdf" | first %}

<div class="home-wrapper">
  <h1 class="page__title">Curriculum Vitae</h1>

  {% if cv %}
  <div class="cv-meta">
    <p class="cv-meta-label">CV last updated</p>
    <p class="cv-meta-date">{% if page.cv_updated %}{{ page.cv_updated | date: "%B %-d, %Y" }}{% else %}{{ cv.modified_time | date: "%B %-d, %Y" }}{% endif %}</p>
  </div>

  <div class="cv-download">
    <a href="{{ base_path }}/files/cv_jiahanghe.pdf" download>Download current CV</a>
  </div>

  <div class="cv-embed">
    <iframe src="{{ base_path }}/files/cv_jiahanghe.pdf" title="Curriculum Vitae of Jiahang He"></iframe>
  </div>
  {% else %}
  <div class="page__content">
    <p>
      The CV is not published yet. Add the PDF at <code>files/cv_jiahanghe.pdf</code>
      and this page will show a download button and an inline viewer automatically,
      with the date taken from the file itself.
    </p>
  </div>
  {% endif %}
</div>
