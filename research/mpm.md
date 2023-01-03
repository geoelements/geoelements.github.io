---
title: "Material Point Method"
categories: research
tags: [mpm]
layout: page
---

Material Point Method (MPM) is a particle based method that represents the
material as a collection of material points, and their deformations are
determined by Newton’s laws of motion. The MPM is a hybrid Eulerian-Lagrangian
approach, which uses moving material points and computational nodes on a background mesh.
This approach is very effective particularly in the context of large deformations.

![algorithm]({{site-url}}/research/mpm-algorithm.png)

> Illustration of the MPM algorithm (1) A representation of material points overlaid on
a computational grid. Arrows represent material point state vectors (mass, volume, velocity, etc.)
being projected to the nodes of the computational grid. (2) The equations of motion are solved onto
the nodes, resulting in updated nodal velocities and positions. (3) The updated nodal kinematics
are interpolated back to the material points. (4) The state of the material points is updated, and the
computational grid is reset

## MPM Online course book
Learn to code MPM with Python [online book](https://www.geoelements.org/LearnMPM/intro.html)

## CB-Geo MPM code

* The CB-Geo MPM code is available at [GitHub](https://github.com/cb-geo/mpm)

## Documentation

* [MPM documentation](https://mpm.cb-geo.com)


## Team
<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% for area in member.area %}
        {% if area == "MPM" %}
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
{% assign researcharea = "mpm" %}
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