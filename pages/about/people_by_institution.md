---
permalink: /about/people_by_institution.html
layout: people
title: CLARIPHY Collaboration
---

{% include institution_list.html %}

<div>
    {% for uniindex in institution_list %}
      {%- assign univ = site.data.universities[uniindex] -%}
      <h5>{{univ.name}}</h5>
<div class="container pt-6 pb-6">
  <div class="row pt-6 pb-6">
      {%- assign sorted_mapping = "" | split:"," -%}
      {%- for memberid in univ.personnel -%}
        {%- assign member = site.data.people[memberid] -%}
        {%- assign sortable_name = member.name | split:" " | reverse | join:" " -%}
        {%- capture item -%}
          {{sortable_name}};{{memberid}}
        {%- endcapture -%}
        {%- assign sorted_mapping = sorted_mapping | push: item -%}
      {%- endfor -%}
      {%- assign sorted_people = sorted_mapping | sort -%}

      {% for member in sorted_people %}
           {%- assign item = member | split:";" -%}
           {%- assign item = item[1] -%}
           {% assign person = site.data.people[item] %}
           {% include standard_person_card_2.md %}
      {% endfor %}
  </div>
</div>
    {% endfor %}
</div>

