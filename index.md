---
layout: home
title: Deep Mining
nav_exclude: true
toc: true
seo:
  type: Courses
  name: Deep Mining
---

# {{ site.tagline }}
{: .no_toc .mb-2 }
{{ site.description }}
<br>
MoWe / 3-4:20PM, [L101 WEB](https://bit.ly/3wBNjzE); will be recorded
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}


We will use **<span style="color: red;">Canvas</span>** for:
* **Syllabus** (office hours, grading criteria, policies, etc.) 
* **Announcements** 
* **Discussions** (questions on homework, projects, material covered in class, schedule, etc.)
* **Turning in assignments** and **project** components,
* **Communicating grades**. 

Please use the discussion forum as the preferred medium for interacting with the instructor and the teaching assistants rather than emailing/messaging directly. 

Through **<span style="color: red-300;">this website</span>** we will share:
* **Schedule**, 
* **Lecture notes**, 
* **Lecture videos**, 

Take advantage of the instructor and TA office hours. We will work hard to be accessible to students. Don’t be shy if you don’t understand something: come to office hours, send emails, or speak up in class!

## Description

Data mining is the study of efficiently finding structures and patterns in large data sets. We will focus on several aspects of this: (1) converting from a messy and noisy raw data set to a structured and abstract one, (2) applying scalable and probabilistic algorithms to these well-structured abstract data sets, and (3) formally modeling and understanding the error and other consequences of parts (1) and (2), including choice of data representation and trade-offs between accuracy and scalability. These steps are essential for training as a data scientist.

Algorithms, programming, probability, and linear algebra are required tools for understanding these approaches.

Topics will include: similarity search, clustering, regression/dimensionality reduction, graph analysis, PageRank, and small space summaries. We will also cover several recent developments, and the application of these topics to modern applications, often relating to large internet-based companies.

Upon completion, students should be able to read, understand, and implement ideas from many data mining research papers.

## Calendar

Calendar is **tentative and subject to change**.
More details will be added as the semester continues.

<table>
  <thead>
  <tr>
    <th>Week</th>
    <th>Date</th>
    <th width="20%">Theme</th>
    <th width="30%">Contents</th>
    <th width="13%">Work due</th>
  </tr>
  </thead>
  <tbody>
  {% for week in site.data.calendar %}
    {% for day in week.days %}
      <tr>
        {% if forloop.index == 1 %}
        <td rowspan="{{week.size}}">{{week.week}}</td>
        {% endif %}
        <td>{{day.date}}</td>
        <td>{{day.theme}}</td>
        <td class="cal-content">
          {{day.topics}}
          {% if day.slides %}
            <a href="{{day.slides}}" class="cal-content-link">[slides]</a>
          {% endif %}
          {% if day.readings %}
            <a href="{{day.readings}}" class="cal-content-link">[readings]</a>
          {% endif %}
        </td>
        <td class="cal-content">{{day.due}}</td>
      </tr>
    {% endfor %}
  {% endfor %}
  </tbody>
</table>

