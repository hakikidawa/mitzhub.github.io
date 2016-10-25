---
layout: page-fullwidth
title: ''
teaser: ' '
permalink: /about-us/
header:
  image_fullwidth: header_roadmap_2.jpg
published: true
---




## About MiTz

*HakikiDawa* College of Informatics and Virtual Education (CIVE) of the University of Dodoma (UDOM), through the financial support of Tanzania Communications Regulatory Authority (TCRA), embarked on a three-year research on Applying Mobile Technology for Drugs Verification in Tanzania. The main objective of the research was to design, develop, implement and support a mobile technology-based system to secure the Tanzanian health sector .
{: style="text-align: justify;"}

### Mission
To promote, facilitate and support the development of innovative  ICT solutions and services that address Tanzania Health sector challenges.
{: style="text-align: justify;"}

### Vision


</div><!-- /.medium-8.columns -->
</div><!-- /.row -->

<!-- Team members -->
{% if site.data.team-members.size > 0 %}
<section class="team-members">
  <h2>Our Team</h2>
  <div class="grid-container">
    {% for member in site.data.team-members %}
    {% comment %}Check whether total no. of staff members is odd / even and structure final member accordingly{% endcomment %}
    {% assign columnMod = forloop.length | modulo:2 %}
    {% if columnMod == 0 %}
      {% cycle '<div class="row">', '' %}
      <!-- Team member card -->
      {% include staff-card.html columnClass='one-half col' %}<!-- End team member card -->

      {% cycle '', '</div>' %}
    {% else %}
      {% unless forloop.last == true %}
        {% cycle '<div class="row">', '' %}
        <!-- Team member card -->
        {% include staff-card.html columnClass='one-half col' %}<!-- End team member card -->

        {% cycle '', '</div>' %}
      {% else %}
      <!-- Team member card -->
        {% include staff-card.html columnClass='one-half col final-col' %}<!-- End team member card -->
      {% endunless %}
    {% endif %}
  {% endfor %}
  </div>
</section>
{% endif %}<!-- End team members -->

 [1]: http://kramdown.gettalong.org/converter/html.html#toc
 [2]: {{ site.url }}/blog/
 [3]: http://srobbin.com/jquery-plugins/backstretch/
 [4]: #
 [5]: #
 [6]: #
 [7]: #
 [8]: #
 [9]: #
 [10]: #
