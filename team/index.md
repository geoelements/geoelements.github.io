---
layout: page
title: Team
excerpt: "Geoelements research team"
#image:
#  feature: geoelements/banner.png
---

<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "academic" %}
       <div class="user"> <a href="{{member.url}}">
         <div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
         </div> </a>
         <h4><a href="{{member.url}}">{{ member.name }}</a></h4>	
         {{ member.position }}, {{member.uni }}<br/>
	       <a href="mailto:{{ member.email }}">{{ member.email }}</a>
       </div>
      {% endif %}
    {% endfor %}
   </div>
<!-- End team -->



<!-- Team filled from _data/members.yaml
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "researcher" %}
       <div class="user">
         <div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
         </div>
         <h4>{{ member.name }}</h4>	
         {{ member.position }}, {{member.uni }}<br/>
	 <a href="mailto:{{ member.email }}">{{ member.email }}</a>
       </div>
      {% endif %}
    {% endfor %}
   </div>
<!-- End team -->

### Ph.D. students

<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "student" %}
       <div class="user">
         <a href="{{member.url}}"><div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
         </div></a>
         <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
         <a href="mailto:{{ member.email }}">{{ member.email }}</a>
       </div>
      {% endif %}
    {% endfor %}
   </div>
<!-- End team -->

### Alumni

<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "masters" %}
       <div class="user"><a href="{{member.url}}">
         <div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
         </div> </a>
         <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
          Graduated {{ member.year }} <br/>{{ member.position }}, {{ member.uni }}.
       </div>
      {% endif %}
    {% endfor %}
   </div>
<!-- End team -->
