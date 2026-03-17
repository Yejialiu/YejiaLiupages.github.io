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
* On-device efficient inference of AI models and LLMs
* Adaptive and robust deployment of AI models
* Previous experience in [3D human pose estimation]({{ base_path }}/publication/movid-view-invariant-3d-human-pose/) and related 3D vision problems such as 3D reconstruction

Education
======
* Ph.D. student in [Computer Science and Engineering](https://cse.hkust.edu.hk/), [The Hong Kong University of Science and Technology](https://hkust.edu.hk/)
  * Advisor: [Prof. Xiaomin Ouyang](https://seng.hkust.edu.hk/about/people/faculty/xiaomin-ouyang)
* Undergraduate studies, [Global College](https://gc.sjtu.edu.cn/) (formerly UM-SJTU Joint Institute), [Shanghai Jiao Tong University](https://en.sjtu.edu.cn/)
* Exchange student, [Technical University of Munich (TUM)](https://www.tum.de/en/), Apr. 2024 - Jul. 2024
* [High School Affiliated to Shanghai Jiao Tong University](https://fz.sjtu.edu.cn/)

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
      {% assign citation_text = post.citation %}
      {% if post.venue and post.venue_url %}
        {% capture linked_venue %}<a href="{{ post.venue_url }}">{{ post.venue }}</a>{% endcapture %}
        {% assign citation_text = post.citation | replace: post.venue, linked_venue %}
      {% endif %}
      {{ citation_text }}
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
    {% if post.link %}
      <strong><a href="{{ post.link }}">{{ post.title }}</a></strong>
    {% else %}
      <strong>{{ post.title }}</strong>
    {% endif %}
    {% if post.venue %}, {% if post.venue_url %}<a href="{{ post.venue_url }}">{{ post.venue }}</a>{% else %}{{ post.venue }}{% endif %}{% endif %}
    {% if post.term %}, {{ post.term }}{% endif %}
  </li>
{% endfor %}
</ul>

Academic & Research-related Awards
======
* [UM-SJTU Joint Institute](https://gc.sjtu.edu.cn/) Yu Leming Scholarships, 2023-2024 and 2024-2025
* B Merit Scholarship, 2023-2024 and 2024-2025
* Undergraduate Scholarship for Academic Progress, 2023-2024

Contact
======
* Email: [wendyliuyejia@sjtu.edu.cn](mailto:wendyliuyejia@sjtu.edu.cn)
* GitHub: [Yejialiu](https://github.com/Yejialiu)
