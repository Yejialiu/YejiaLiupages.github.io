---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download CV as PDF]({{ base_path }}/assets/Yejia_Liu_CV.pdf)

Research Interests
======
* Computer vision
* Machine learning
* Embedded AI systems

Education
======
* Ph.D. student in Computer Science and Engineering, The Hong Kong University of Science and Technology
  * Advisor: [Prof. Xiaomin Ouyang](https://seng.hkust.edu.hk/about/people/faculty/xiaomin-ouyang)
* Undergraduate studies, Global College (formerly UM-SJTU Joint Institute), Shanghai Jiao Tong University
* High School Affiliated to Shanghai Jiao Tong University

Publications
======
<ul>
{% for post in site.publications reversed %}
  {% if post.listed == false %}
    {% continue %}
  {% endif %}
  <li>
    <a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a><br />
    {% if post.citation %}
      {{ post.citation }}
    {% elsif post.status %}
      {{ post.status }}
    {% endif %}
  </li>
{% endfor %}
</ul>

Teaching
======
<ul>
{% for post in site.teaching reversed %}
  <li>
    <strong>{{ post.title }}</strong>
    {% if post.venue %}, {{ post.venue }}{% endif %}
    {% if post.term %}, {{ post.term }}{% endif %}
  </li>
{% endfor %}
</ul>

Academic & Research-related Awards
======
* UM-SJTU Joint Institute Yu Leming Scholarships, 2023-2024 and 2024-2025
* B Merit Scholarship, 2023-2024 and 2024-2025
* Undergraduate Scholarship for Academic Progress, 2023-2024

Contact
======
* Email: [wendyliuyejia@sjtu.edu.cn](mailto:wendyliuyejia@sjtu.edu.cn)
* GitHub: [Yejialiu](https://github.com/Yejialiu)
