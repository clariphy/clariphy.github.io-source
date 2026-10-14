---
permalink: /jobs.html
layout: default
title: Available Positions
---

# Machine Learning and AI research positions in Physics

A number of employment opportunities for ML/AI-related research exist with the groups involved in CLARIPHY as well as collaborating projects. If you have a strong interest in challenging problems in an exciting research environment, please consider applying! This page will be updated from time to time. As such please check back for the latest opportunities.

{% comment %}
The positions are taken from the yml files in _data/jobs (one file per
position, see the comments there for the fields). Positions with a deadline
are listed first, with the earliest deadline at the top; positions whose
deadline has passed are dropped automatically (the site is rebuilt nightly).
Positions with no deadline are listed afterwards, by institution.
{% endcomment %}

{% assign today = site.time | date: "%Y-%m-%d" %}
{% assign dated_jobs = "" | split: ',' %}
{% assign undated_jobs = "" | split: ',' %}
{% for job_hash in site.data.jobs %}
  {% assign job = job_hash[1] %}
  {% if job.deadline %}
    {% assign deadline_key = job.deadline | date: "%Y-%m-%d" %}
    {% if deadline_key >= today %}
      {% assign dated_jobs = dated_jobs | push: job %}
    {% endif %}
  {% else %}
    {% assign undated_jobs = undated_jobs | push: job %}
  {% endif %}
{% endfor %}
{% assign dated_jobs = dated_jobs | sort: 'deadline' %}
{% assign undated_jobs = undated_jobs | sort: 'institution' %}
{% assign open_jobs = dated_jobs | concat: undated_jobs %}

{% if open_jobs.size == 0 %}
**Coming Soon**
{% else %}
<ul>
{% for job in open_jobs %}
<li>
<a href="{{ job.url }}">{{ job.title }}</a>
<ul>
<li>Institution: {{ job.institution }}{% if job.location %} ({{ job.location }}){% endif %}</li>
{% if job.rank %}<li>Rank: {{ job.rank }}</li>{% endif %}
<li>Deadline: {% if job.deadline %}{{ job.deadline | date: "%-d %B %Y" }}{% else %}none given; applications accepted until the position is filled{% endif %}</li>
{% if job.description %}<li>{{ job.description }}</li>{% endif %}
</ul>
</li>
{% endfor %}
</ul>
{% endif %}
