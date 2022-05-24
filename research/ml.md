---
layout: page
title: "Machine Learning and X-AI"
categories: research
tags: [LBM]
---

Our research on ML and X-AI focuses on developing interpretable techniques for modeling liquefaction and full-wave form inversions. We also develop Graph-Network Simulator (GNS) to model large-deformation flows.


## Code

* Graph Network Simulator (GNS)[GitHub](https://www.github.com/geoelements/gns) 

## Simulations

![GNS simulation of granular flow](https://raw.githubusercontent.com/geoelements/gns/main/figs/rollout_0.gif)


## Team
<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% for area in member.area %}
        {% if area == "ML" %}
          <div class="user">
            <div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
            </div>
            <h4>{{ member.name }}</h4>	
            {{ member.position }}, {{member.uni }}<br/>
	 <a h   ref="mailto:{{ member.email }}">{{ member.email }}</a>
          </div>
        {% endif%}
      {% endfor %}
    {% endfor %}
   </div>
<!-- End team -->

## Publications
<!-- Publications filled automatically -->
<div class="publications">
{% assign researcharea = "ml" %}
{% assign postsbyTags = site.posts | where_exp: "post", "post.categories contains 'publications'" |
group_by_exp:
'posts', 'posts.tags' %}
{% for postarticles in postsbyTags %}
  {% if postarticles.name contains researcharea %}
    <div class="entries-{{ page.entries_layout | default: 'list' }}">
    {% for entry in postarticles.items %}
      {% include pub-entry.html %}
    {% endfor %}
    </div>
  {% endif %}
{% endfor %}
</div>