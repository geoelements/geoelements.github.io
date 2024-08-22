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

### Postdoctoral Research Fellows

<!-- Team filled from _data/members.yaml -->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "postdoc" %}
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


### Ph.D. students

<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "student" %}
        {% if member.position == "PhD candidate" %}
        <div class="user">
          <a href="{{member.url}}"><div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
          </div></a>
          <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
          <a href="mailto:{{ member.email }}">{{ member.email }}</a>
        </div>
        {% endif %}
      {% endif %}
    {% endfor %}
   </div>
<!-- End team -->

### MS students


<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "student" %}
        {% if member.position == "MS student" %}
        <div class="user">
          <a href="{{member.url}}"><div class="userimg" style="background-image:url('{{ site.baseurl }}/images/geoelements/team/{{ member.image }}')">
          </div></a>
          <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
          <a href="mailto:{{ member.email }}">{{ member.email }}</a>
        </div>
        {% endif %}
      {% endif %}
    {% endfor %}
   </div>
<!-- End team -->

### Alumni

<!-- Team filled from _data/members.yaml-->
   <div class="team">
    {% for member in site.data.members %}
      {% if member.role == "alumni" %}
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

### Prospective students
If you are interested in joining our research team, read our [wiki](https://geoelements.org/wiki/), especially the section on 
[prospective students](https://www.geoelements.org/wiki/#/prospective-students) and [expectations and responsibilities](https://www.geoelements.org/wiki/#/expectations). Please read [the email guidelines](https://www.geoelements.org/wiki/#/prospective-students?id=i-want-to-get-on-krishna39s-radar-before-i-submit-my-application-how-do-i-do-that) before contacting Krishna to express your research interest. 