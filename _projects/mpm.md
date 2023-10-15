---
title: "In Situ Viz with Material Point Method"
collection: projects
excerpt: "Real-time rendering of MPM landslide simulations"
image: 
  path: /images/projects/insitu-oso-mpm.png
  thumbnail: /images/projects/insitu-oso-mpm.png
---

Our research group has developed a new scalable approach for in situ visualization of regional-scale natural hazards using the Material Point Method (MPM) coupled with the Galaxy ray tracing engine. As described in the recent article by [Abram et al.](https://arxiv.org/pdf/2109.02754.pdf), we can simulate large-scale landslide runouts with millions of material points and visualize the dynamics in real time. For example, we simulated the 2014 Oso landslide with 4.2 million particles and achieved compelling visuals of the runout using spheres colored by particle displacement. Our in situ approach had a minimal runtime increase of only 2% compared to non-visualized simulations. This scalable MPM and Galaxy architecture enables new insights into regional hazards through high-fidelity real-time visualization. Our group continues to push the capabilities of in situ visualization to handle increased scale and complexity for geoscience applications.

![In situ](/images/projects/insitu-oso-mpm.png)
> In situ rendering of the Oso washington landslide with 4.2 Million material points.

## MPM and Galaxy codes

* The CB-Geo MPM code is available at [GitHub](https://github.com/cb-geo/mpm)

* The TACC Galaxy viz code is available at [GitHub](https://github.com/tacc/galaxy)

## Publications
<!-- Publications filled automatically -->
<div class="publications">
{% assign researcharea = "insitu" %}
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