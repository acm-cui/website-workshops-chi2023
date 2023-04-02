---
layout: page
title: Accepted position papers

nav_text: Accepted papers
nav_position: 3
---

<!-- The accepted papers will be available here before the workshop, if you would like to submit please check out our [Call for Papers](https://www.conversationaluserinterfaces.org/workshops/CHI2023/call-for-papers.html) page for details about submitting to the workshop. -->

The following papers were accepted for inclusion in the workshop: 

<!-- <table>
  <tr>
    <th>Themes</th>
    <th>Author(s)</th>
    <th>Title</th>
  </tr>
  {% for entry in site.data.papers %}
  <tr>
    <td>{{ entry.theme}}</td>
    <td></td>
    <td></td>
  </tr>
  {% for paper in entry.papers %}
  <tr>
    <td></td>
    <td>{{paper.authors}}</td>
    <td><a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a></td>
  </tr>
   {% endfor %}

{% endfor %}
</table> -->

<table>
  <tr>
    <th>Author(s)</th>
    <th>Title</th>
  </tr>
  <!-- {% for entry in site.data.papers %} -->
  {% for paper in entry.papers %}
  <tr>
    <td>{{paper.authors}}</td>
    {% if paper.pdf %}
    <td><a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a></td>
    {% else %}
    <td>{{ paper.title }}</td>
    {% endif %}
  </tr>
   {% endfor %}

<!-- {% endfor %} -->
</table>
