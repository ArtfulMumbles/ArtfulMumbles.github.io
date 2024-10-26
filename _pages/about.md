---
layout: about
title: "about"
permalink: /
subtitle: |
  "The more I read, the more I acquire, the more certain I am that I know nothing." — <cite>Voltaire</cite>
profile:
  align: right
  image: prof_pic.png
  image_circular: false
  more_info: ""
news: true
selected_papers: false
social: false
blog: false
---

<!-- Content container to ensure content is above the particles -->
<div class="post content particles-content">

  <p>I’m a third-year student at <a href="https://duke.edu" target="_blank">Duke University</a> pursuing degrees in ECE and CS. My work blends AI, robotics, and bioinformatics, where I explore applications of <a href="https://labwebsite.com" target="_blank">protein language models</a> for drug development under the guidance of <a href="https://rohitsinghlab.com" target="_blank">Dr. Rohit Singh</a>.</p>

  <p>My work has earned me a <a href="https://pratt.duke.edu/" target="_blank">Pratt Fellowship</a> and consideration for graduation with distinction in ECE. I also serve as a TA for undergraduate ECE labs.</p>

  <p>I enjoy <a href="/portfolio">photography</a>, Italian fusion cuisine, and <a href="https://spotify.com/your-podcast" target="_blank">host a podcast</a> that highlights Duke's most impressive talent.</p>

  <h2>Featured Projects</h2>
  <div class="row row-cols-1 row-cols-md-3">
    {% assign featured_projects = site.projects | sort: "importance" | slice: 0, 3 %}
    {% for project in featured_projects %}
      {% include projects.liquid project=project %}
    {% endfor %}
  </div>

  <p style="text-align: center; margin-top: 20px;">
    <a href="/projects/" class="btn btn-primary">View All Projects</a>
  </p>
</div>
