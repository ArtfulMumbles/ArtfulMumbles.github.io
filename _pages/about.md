---
layout: about
title: "about"
permalink: /
subtitle: "The more I read, the more I acquire, the more certain I am that I know nothing." — <cite>Voltaire</cite>
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

<!-- Particles.js container -->
<div id="particles-js"></div>

<!-- Content container to ensure content is above the particles -->
<div class="content">
  <h1>Michael A. Scutari</h1>

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

<!-- Load Particles.js script -->
<script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
<script>
  particlesJS("particles-js", {
    "particles": {
      "number": {
        "value": 80,
        "density": {
          "enable": true,
          "value_area": 800
        }
      },
      "color": {
        "value": "#ffffff"
      },
      "shape": {
        "type": "circle",
        "stroke": {
          "width": 0,
          "color": "#000000"
        }
      },
      "opacity": {
        "value": 0.5,
        "random": false
      },
      "size": {
        "value": 5,
        "random": true
      },
      "line_linked": {
        "enable": true,
        "distance": 150,
        "color": "#ffffff",
        "opacity": 0.4,
        "width": 1
      },
      "move": {
        "enable": true,
        "speed": 6,
        "direction": "none",
        "random": false,
        "straight": false,
        "out_mode": "out",
        "bounce": false
      }
    },
    "interactivity": {
      "detect_on": "canvas",
      "events": {
        "onhover": { "enable": true, "mode": "repulse" },
        "onclick": { "enable": true, "mode": "push" },
        "resize": true
      },
      "modes": {
        "repulse": { "distance": 100, "duration": 0.4 },
        "push": { "particles_nb": 4 }
      }
    },
    "retina_detect": true
  });
</script>
