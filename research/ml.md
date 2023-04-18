---
layout: page
title: "Scientific Machine Learning and Differentiable Simulator"
categories: research
tags: [LBM]
---

Our research on Scientific Machine Learning (SciML) and differentiable programming focuses on discovering new physics and developing fast algorithms to accelerate numerical simulations.


## Code
 
* Graph Network Simulator (GNS)[GitHub](https://www.github.com/geoelements/gns) 
Graph Network-based Simulator (GNS) is a framework for developing generalizable, efficient, and accurate machine learning (ML)-based surrogate models for particulate and fluid systems using Graph Neural Networks (GNNs). GNS code is a viable surrogate for numerical methods such as Material Point Method, Smooth Particle Hydrodynamics and Computational Fluid dynamics. GNS exploits distributed data parallelism to achieve fast multi-GPU training. The GNS code can handle complex boundary conditions and multi-material interactions.

## Simulations

![GNS simulation of granular flow](https://raw.githubusercontent.com/geoelements/gns/main/docs/img/rollout_0.gif)

## Videos
X-AI and Machine Learning, 2022 SimCenter-DesignSafe AI workshop
<iframe width="560" height="315" src="https://www.youtube.com/embed/NO8D_vyFzBE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

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