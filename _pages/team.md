---
title: "Star-AI Lab - Team"
layout: gridlay
excerpt: "Star-AI Lab: Team members"
sitemap: false
permalink: /team/
---

# Team Members

<!---Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [administrative support](#administrative-support), [visiting scholors](#lab-visitors).-->

## Directors
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Student Collaborators from other Universities
{% assign number_printed = 0 %}
{% for member in site.data.collaborator_students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!---
## Master's and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
-->



## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!--
## Former visitors, BSc/ MSc students
<div class="row">

<div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitors %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Master students</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
{% endfor %}
</div>

</div>



-->

### Collaborators from University of Arizona (Supervised by Dr. Hsinchun Chen)
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/ua.jpg" class="img-responsive" width="65%" style="float: left; padding:8px" />
</div>

<br/>
<br/>


### Founder's Bio, [Curriculum vitae](/files/Ebrahimi_CV_2025.pdf), and [Google Scholar](https://scholar.google.com/citations?user=4DmURbEAAAAJ&hl=en) 
<div class="col-sm-12 clearfix">
  <!--<a href="https://scholar.google.com/citations?user=4DmURbEAAAAJ&hl=en"> <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/rebrahimi.jpg" class="img-responsive" width="25%" style="float: left; padding:8px" /></a>
  <h4>&nbsp;&nbsp; <a href="https://scholar.google.com/citations?user=4DmURbEAAAAJ&hl=en"> Reza Ebrahimi </a></h4>
  <i>&nbsp;&nbsp; ebrahimim[ at ]usf.edu</i>-->
  <!--<p>&nbsp;&nbsp; Reza is an assistant professor and the director of Star-AI Lab at School of Information Systems and <br>&nbsp;&nbsp; Management (SISM) at the University of South Florida. He received his Ph.D. in Information Systems from <br>&nbsp;&nbsp; the University of Arizona, where he was a research assistant at the Artifical Intelligence (AI) Lab conducted <br>&nbsp;&nbsp; by Regents’ Professor Hsinchun Chen. In 2016, He received his Master's in Computer Science from <br>&nbsp;&nbsp; Concordia University in Montreal, Canada. His Ph.D. Thesis targets two interconnected research areas: <br>&nbsp;&nbsp; Security of AI and AI for Security. His Master's thesis leveraged crime data mining to enhance juveniles' <br>&nbsp;&nbsp; safety in the cyberspace.</p>-->
  <p>Reza is an assistant professor and the director of Star-AI Lab at the School of Information Systems and Management (SISM) at the University of South Florida. He received his Ph.D. in Management Information Systems from the University of Arizona, where he was a research associate at the Artificial Intelligence (AI) Lab in 2021. He received his master’s degree in Computer Science from Concordia University, Canada, in 2016. His Master’s thesis leveraged crime data mining to enhance juveniles’ safety in cyberspace. Reza’s PhD dissertation on AI-enabled cybersecurity analytics won the ACM SIGMIS best doctoral dissertation award in 2021. Reza’s research focuses on statistical and adversarial machine learning for AI-enabled secure and trustworthy cyberspace.</p>
  <p>Reza has published over 40 articles in peer reviewed security journals, conferences, and workshops, including NeurIPS, ICLR, SIAM, IEEE TPAMI, IEEE TDSC, IEEE S&PW, IEEE ACSAC, AAAIW, IEEE ISI, IEEE ICDMW, Applied Artificial Intelligence, Digital Forensics, MIS Quarterly, and JMIS. He has been serving as a Program Chair and Program Committee member in IEEE ICDM Workshop on Machine Learning for Cybersecurity (MLC) and IEEE S&P Workshop on Deep Learning Security and Privacy (DLSP). He servs as an organizer of 2025 IEEE S&P Workshop on Human-Machine Intelligence for Security Analytics (HMI-SA). He has contributed to several projects supported by the National Science Foundation (NSF). He is an IEEE Senior Member and a member of the ACM, AAAI, and AIS.</p>
  
</div>