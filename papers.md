---
layout: page
title: Accepted position papers

nav_text: Accepted papers
nav_position: 3
---

<!-- The accepted papers will be available here before the workshop, if you would like to submit please check out our [Call for Papers](https://www.conversationaluserinterfaces.org/workshops/CHI2023/call-for-papers.html) page for details about submitting to the workshop. -->

The following papers were accepted for inclusion in the workshop:

<table>
  <tr>
    <th>Author(s)</th>
    <th>Title</th>
  </tr>
  {% for paper in site.data.papers %}
  <tr>
    <td>{{paper.authors}}</td>
    <td>{% if paper.pdf %}<a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a>{% else %}<strong>{{ paper.title }}</strong>{% endif %}</td>
  </tr>
  {% endfor %}
</table>
