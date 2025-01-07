---
layout: page
title: Staff
description: A listing of all the course staff members.
nav_order: 4
---

# Staff

<!--Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.-->

## Student Instructor

{% assign student_instructors = site.staffers | where: 'role', 'Student Instructor' %}
{% for staffer in student_instructors %}
{{ staffer }}
{% endfor %}

{% assign instuctor_of_record = site.staffers | where: 'role', 'Instructor of Record' %}
{% assign num_instuctor_of_record = instuctor_of_record | size %}
{% if num_instructor_of_record != 0 %}

## Instructor of Record

{% for staffer in instuctor_of_record %}
{{ staffer }}
{% endfor %}
{% endif %}

<!--{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}-->
<!--{% assign num_teaching_assistants = teaching_assistants | size %}-->
<!--{% if num_teaching_assistants != 0 %}-->
<!--## Teaching Assistants-->
<!---->
<!--{% for staffer in teaching_assistants %}-->
<!--{{ staffer }}-->
<!--{% endfor %}-->
<!--{% endif %}-->
<!---->
<!--{% assign tutors = site.staffers | where: 'role', 'Tutor' %}-->
<!--{% assign num_tutors = tutors | size %}-->
<!--{% if num_tutors != 0 %}-->
<!--## Tutors-->
<!---->
<!--{% for staffer in tutors %}-->
<!--{{ staffer }}-->
<!--{% endfor %}-->
<!--{% endif %}-->
<!---->
<!--{% assign academic_interns = site.staffers | where: 'role', 'Academic Intern' %}-->
<!--{% assign num_academic_interns = academic_interns | size %}-->
<!--{% if num_academic_interns != 0 %}-->
<!--## Academic Interns-->
<!---->
<!--{% for staffer in academic_interns %}-->
<!--{{ staffer }}-->
<!--{% endfor %}-->
<!--{% endif %}-->
