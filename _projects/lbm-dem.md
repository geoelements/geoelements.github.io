---
title: "Micromechanics of soil-water-characteristic curve (SWCC)"
collection: projects
image: 
  path: /images/projects/lbm/lbm-unsaturated.png
  thumbnail: /images/projects/lbm/lbm-unsaturated.png
---

The soil-water characteristic curve (SWCC) relates the amount of water in a soil to its matric suction. This curve exhibits hysteresis - higher suction values are observed during drainage versus imbibition at the same water content. In our recent paper, we used multiphase lattice Boltzmann simulations to elucidate the source of this hysteretic behavior.

We demonstrated that the difference arises from the pore emptying process during drainage versus the pore filling process during imbibition. During drainage, the existing gas phase can only expand into adjacent pores, forcing it through small openings and resulting in small meniscus radii and high suction values. In contrast, during imbibition, new liquid bridges form throughout the pore space. This allows simultaneous expansion and the formation of larger meniscus radii, leading to lower suction values. We validated the source of hysteresis using both 2D and 3D simulations of granular packings. For small 2D packs, hysteresis only occurred when pores were partially filled, but for larger 3D packs, it extended over the entire saturation range.

![SWCC LBM](/images/projects/lbm/gas-cluster-hysteresis.png)
> Hysteresis in gas cluster shapes results in changes in SWCC between drainage and imbibition.

In a follow-up study, we leveraged X-ray computed tomography (CT) experiments on a sandy soil sample to validate our lattice Boltzmann modeling approach. Our simulations successfully reproduced the hysteretic water retention behavior and liquid morphology transitions observed experimentally. Pronounced hysteresis was seen in gas-related parameters like gas cluster count and liquid-gas interfacial area in our models. Our study also revealed that local suction increases or decreases during drainage depending on the pore size, but uniformly decreases during imbibition. Furthermore, larger pores exhibited greater hysteresis as they drained first but filled last.

![DigitalTwin LBM-CT](/images/projects/lbm/digital-twin-ct-lbm.png)
> Constructing a 3D digital twin of CT image using multiphase LBM.

![LBM CT SWCC](/images/projects/lbm/lbm-ct-hysteresis.png)
> CT and LBM SWCC.

Together, these advanced simulations provide unprecedented insights into the microscale physics controlling hysteresis in the SWCC. We elucidate the underlying pore-scale mechanisms and dependence on parameters like pore structure. Our findings will help improve the predictive capabilities of models that rely on the SWCC.

## Code
* The Multiphase LBM code is available at [GitHub](https://github.com/geoelements/mcmp-lbm)

## Publications
<!-- Publications filled automatically -->
<div class="publications">
{% assign researcharea = "swcc" %}
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