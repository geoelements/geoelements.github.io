---
layout: page
title: "Lattice Boltzmann Method"
categories: research
tags: [LBM]
---

The Lattice Boltzmann equation Method (LBM) is an alternative approach to the classical Navier-Stokes
solvers for fluid flow and works on an equidistant grid  of cells, called lattice cells, which interact only with their direct neighbours (He & Luo, 1997). The fluid domain is divided into a rectangular grid or lattice, with the same spacing ‘h’ in both the x- and the y-directions, as shown in the figure. Multiple Relaxation Time (MRT) with Large-Eddy Simulations is used to model turbulent behaviour at high Reynolds number.

![The Lattice Boltzmann discretization and D2Q9 scheme: (a) a standard LB lattice; (b) D2Q9 model]({{site.url}}/research/lbm-d2q9.png)

Lattice Boltzmann approach can accommodate large grain sizes and the interaction between the fluid and the moving grains can be modelled through relatively simple fluid – grain interface treatments. Further,
employing the Discrete Element Method (DEM) to account for the grain – grain interaction naturally leads
to a combined LB – DEM procedure (Kumar, Soga, & Delenne, 2012). The Eulerian nature of the LBM formulation, together with the common explicit time step scheme of both LBM and DEM makes this coupling
strategy an efficient numerical procedure for the simulation of grain – fluid systems.

## Main features

* 2D Coupled LBM-DEM
* D2Q9 with Multiple Relaxation Time
* Large Eddy Simulations for turbulence modelling

## Code

* The 2D version of the LBM-DEM code is now available at [GitHub](https://www.github.com/cb-geo/2d-lbm-dem) 

* The docker image of the LBM code is available at [DockerHub](https://hub.docker.com/r/cbgeo/lbmdem/)

## Simulations

<iframe width="1280" height="720" src="https://www.youtube.com/embed/videoseries?list=PLi1zSZT1LUhD5cXf-UBK6WOebbMzcIznz" frameborder="0" allowfullscreen></iframe>


## Team
<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role != "alumni" %}
        {% for area in member.area %}
          {% if area == "LBM" %}
            <div class="user">
              <div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
              </div>
              <h4>{{ member.name }}</h4>	
              {{ member.position }}, {{member.uni }}<br/>
    <a h   ref="mailto:{{ member.email }}">{{ member.email }}</a>
            </div>
          {% endif%}
        {% endfor %}
      {% endif%}
    {% endfor %}
   </div>
<!-- End team -->

## Publications
<!-- Publications filled automatically -->
<div class="publications">
{% assign researcharea = "lbm" %}
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