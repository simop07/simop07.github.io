---
layout: cv-layout
title: "Curriculum Vitae"
permalink: /cv/
---

# {{ site.data.cv.name }}
**{{ site.data.cv.title }}**

{{ site.data.cv.summary }}

## Contact
- Email: [{{ site.data.cv.contacts.email }}](mailto:{{ site.data.cv.contacts.email }})
- LinkedIn: [{{ site.data.cv.contacts.linkedin }}](https://www.linkedin.com/in/{{ site.data.cv.contacts.linkedin }})
- GitHub: [{{ site.data.cv.contacts.github }}](https://github.com/{{ site.data.cv.contacts.github }})

## Education
{% for edu in site.data.cv.education %}
- **{{ edu.degree }}**, {{ edu.institution }} ({{ edu.period }}), {{ edu.location }}
{% endfor %}

## Selected Projects
{% for p in site.data.cv.projects %}
- **[{{ p.title }}]({{ p.link }})** – {{ p.description }}
{% endfor %}

## Languages
{% for lang in site.data.cv.languages %}
- {{ lang.name }}: {{ lang.level }}
{% endfor %}

## Skills
{% for s in site.data.cv.skills %}
- {{ s }}
{% endfor %}
