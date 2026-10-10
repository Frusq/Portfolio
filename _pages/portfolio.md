---
layout: single
title: "Portfolio"
permalink: /portfolio/
author_profile: false
classes: wide
groups:
  - id: frc-6036
    name: "FRC 6036"
    blurb: "Replace with one line about the team and your role"
    projects:
      - title: "500° Turreted Ball Shooter"
        situation: "Replace with the situation: what the problem was and what you set out to build. Fully autonomous shooter firing 8 balls per second, ranked top 100 globally in 2026."
        points:
          - "Replace with what you designed or modeled"
          - "Replace with a constraint or challenge you solved"
          - "Replace with what you manufactured"
        tools: ["Onshape", "3D Printing", "CNC Router"]
        hero: /assets/images/BallKnowledge.jpg
        hero_alt: "FRC 6036 robot surrounded by yellow balls"
        links: []
        sections:
          - heading: "How it works"
            text: "Replace with a short explanation of the mechanism, like how the turret aims and how balls are fed."
          # Example of a photo row (upload the photos to assets/images first):
          # - heading: "Dev / Test"
          #   images:
          #     - { src: "/assets/images/shooter-test-1.jpg", alt: "Testing the shooter", caption: "Replace with a caption" }
          #     - { src: "/assets/images/shooter-test-2.jpg", alt: "Shooter assembly" }
  - id: purdue-electric-racing
    name: "Purdue Electric Racing"
    blurb: "Replace with one line about your drivetrain role"
    projects:
      - title: "Drivetrain Component"
        situation: "Replace with the situation: what part this is and why the drivetrain needed it."
        points:
          - "Replace with how you designed it"
          - "Replace with how it was machined (3-axis or 5-axis)"
          - "Replace with tolerances or results"
        tools: ["Siemens NX", "5-Axis Milling", "GD&T"]
        hero: /assets/images/PERPlaque.jpg
        hero_alt: "Aluminum machined part"
        links: []
        sections: []
  - id: personal-projects
    name: "Personal Projects"
    blurb: "Replace with one line about what you build on your own"
    projects:
      - title: "Folding Laptop Stand"
        situation: "Replace with the situation: what you wanted and why you made it."
        points:
          - "Replace with how you designed it"
          - "Replace with how it was made"
        tools: ["Autodesk Fusion", "3D Printing"]
        hero: /assets/images/LaptopStand.jpg
        hero_alt: "Black folding laptop stand"
        links: []
        sections: []
---

<style>
  /* Prevent sideways scrolling */
  html,
  body {
    overflow-x: hidden;
    max-width: 100%;
  }
  @supports (overflow: clip) {
    html,
    body {
      overflow-x: clip;
    }
  }

  /* Small pink uppercase label with a line, used for group headings */
  .label {
    display: flex;
    align-items: center;
    gap: 0.9em;
    margin: 0 0 1.3em;
    font-size: 0.8em;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.18em;
    color: #f48fb1;
  }
  .label::after {
    content: "";
    flex: 1;
    height: 1px;
    background: rgba(244, 143, 177, 0.35);
  }

  /* Chamfered tags */
  .tag {
    display: inline-block;
    padding: 0.35em 0.95em 0.35em 1.1em;
    font-size: 0.85em;
    font-weight: 500;
    letter-spacing: 0.02em;
    white-space: nowrap;
    background: rgba(244, 143, 177, 0.15);
    box-shadow: inset 3px 0 0 #f48fb1;
    clip-path: polygon(0 0, calc(100% - 9px) 0, 100% 9px, 100% 100%, 9px 100%, 0 calc(100% - 9px));
    transition: background 0.15s ease, box-shadow 0.15s ease;
  }
  a.tag {
    color: inherit;
    text-decoration: none;
  }
  a.tag:hover {
    background: rgba(244, 143, 177, 0.3);
    box-shadow: inset 5px 0 0 #f48fb1;
  }
  .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55em;
  }

  /* Intro and jump links */
  .lead { font-size: 1.1em; max-width: 46em; margin-bottom: 1.2em; }
  .jump { margin-bottom: 2.5em; }

  /* Overview: thumbnails of every project */
  .overview {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(190px, 1fr));
    gap: 2em 1.6em;
    margin-bottom: 4.5em;
  }
  .ov {
    display: block;
    color: inherit;
    text-decoration: none;
  }
  .ov img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border: 8px solid #fff;
    background-color: #fff;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.55);
    transition: transform 0.25s ease;
  }
  .ov:hover img { transform: translateY(-4px); }
  .ov-group {
    margin-top: 0.8em;
    font-size: 0.7em;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: #f48fb1;
  }
  .ov-title { margin-top: 0.15em; font-size: 0.95em; line-height: 1.3; }

  /* Groups and projects */
  .group { margin-bottom: 3.5em; }
  .group-blurb { margin: -0.4em 0 2.5em; opacity: 0.8; }

  .project {
    margin-bottom: 4.5em;
    scroll-margin-top: 2em;
  }
  .page__content h3.project-title {
    margin: 0 0 1.2em;
    font-size: 1.35em;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.06em;
  }

  .project-top {
    display: grid;
    grid-template-columns: 1fr 1.15fr;
    gap: 3em;
    align-items: start;
    margin-bottom: 3em;
  }
  @media (max-width: 800px) {
    .project-top { grid-template-columns: 1fr; gap: 1.5em; }
  }
  .situation { margin: 0 0 1em; }
  .situation strong { color: #f48fb1; }

  .plain-list {
    list-style: none;
    margin: 0 0 1.2em;
    padding: 0;
  }
  .plain-list li {
    position: relative;
    padding-left: 1.6em;
    margin-bottom: 0.7em;
  }
  .plain-list li:last-child { margin-bottom: 0; }
  .plain-list li::before {
    content: "\2192";
    position: absolute;
    left: 0;
    color: #f48fb1;
  }

  /* Photos: thick white border, square corners */
  .photo {
    display: block;
    width: 100%;
    border: 14px solid #fff;
    border-radius: 0;
    background-color: #fff;
    box-shadow: 0 8px 22px rgba(0, 0, 0, 0.6);
  }

  .project-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8em 1.6em;
    margin-top: 1.2em;
  }

  /* Extra sections inside a project (How it works, Dev / Test, etc.) */
  .section { margin-bottom: 3em; }
  .section-heading {
    margin: 0 0 0.8em;
    font-size: 0.85em;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.16em;
  }
  .section-text { max-width: 46em; margin: 0 0 1.4em; }
  .shots {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.6em;
  }
  .shots figure { margin: 0; }
  .shots img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border: 10px solid #fff;
    background-color: #fff;
    box-shadow: 0 8px 22px rgba(0, 0, 0, 0.6);
  }
  .shots figcaption {
    margin-top: 0.7em;
    font-size: 0.85em;
    opacity: 0.8;
  }

  /* Close the gap above the footer */
  .page__content { padding-bottom: 0 !important; margin-bottom: 0 !important; }
  .page { margin-bottom: 0 !important; padding-bottom: 0 !important; }
  .page__footer { margin-top: 2em !important; }

  /* Fall into place as you scroll (only when JavaScript is available) */
  .rv-on .rv {
    opacity: 0;
    transform: translateY(40px);
  }
  .rv-on .rv.in {
    opacity: 1;
    transform: none;
    transition: opacity 0.7s ease-out, transform 0.7s cubic-bezier(0.34, 1.3, 0.64, 1);
  }
  @media (prefers-reduced-motion: reduce) {
    .rv-on .rv { opacity: 1; transform: none; }
  }
</style>

<p class="lead">A selection of things I've designed and built, grouped by where I made them.</p>

<div class="tags jump">
  {% for g in page.groups %}<a class="tag" href="#{{ g.id }}">{{ g.name }}</a>{% endfor %}
</div>

<div class="overview">
  {% for g in page.groups %}
    {% for p in g.projects %}
      <a class="ov rv" href="#{{ g.id }}-{{ p.title | slugify }}">
        <img src="{{ p.hero }}" alt="{{ p.hero_alt }}">
        <div class="ov-group">{{ g.name }}</div>
        <div class="ov-title">{{ p.title }}</div>
      </a>
    {% endfor %}
  {% endfor %}
</div>

{% for g in page.groups %}
<div class="group" id="{{ g.id }}">
  <h2 class="label rv">{{ g.name }}</h2>
  {% if g.blurb %}<p class="group-blurb">{{ g.blurb }}</p>{% endif %}

  {% for p in g.projects %}
  <div class="project" id="{{ g.id }}-{{ p.title | slugify }}">
    <h3 class="project-title rv">{{ p.title }}</h3>

    <div class="project-top">
      <div class="rv">
        <p class="situation"><strong>Situation:</strong> {{ p.situation }}</p>
        <ul class="plain-list">
          {% for pt in p.points %}<li>{{ pt }}</li>{% endfor %}
        </ul>
        {% if p.tools %}
        <div class="tags">
          {% for t in p.tools %}<span class="tag">{{ t }}</span>{% endfor %}
        </div>
        {% endif %}
        {% if p.links and p.links.size > 0 %}
        <div class="project-links">
          {% for l in p.links %}<a href="{{ l.url }}" target="_blank" rel="noopener">{{ l.label }} &rarr;</a>{% endfor %}
        </div>
        {% endif %}
      </div>
      <div class="rv">
        <img class="photo" src="{{ p.hero }}" alt="{{ p.hero_alt }}">
      </div>
    </div>

    {% for s in p.sections %}
    <div class="section rv">
      <h4 class="section-heading">{{ s.heading }}</h4>
      {% if s.text %}<p class="section-text">{{ s.text }}</p>{% endif %}
      {% if s.images %}
      <div class="shots">
        {% for im in s.images %}
        <figure>
          <img src="{{ im.src }}" alt="{{ im.alt }}">
          {% if im.caption %}<figcaption>{{ im.caption }}</figcaption>{% endif %}
        </figure>
        {% endfor %}
      </div>
      {% endif %}
    </div>
    {% endfor %}
  </div>
  {% endfor %}
</div>
{% endfor %}

<script>
  (function () {
    var els = document.querySelectorAll('.rv');
    if (!('IntersectionObserver' in window)) return;
    if (window.matchMedia('(prefers-reduced-motion: reduce)').matches) return;
    document.documentElement.classList.add('rv-on');
    var io = new IntersectionObserver(function (entries) {
      entries.forEach(function (e) {
        if (e.isIntersecting) {
          e.target.classList.add('in');
          io.unobserve(e.target);
        }
      });
    }, { threshold: 0.12 });
    els.forEach(function (el) { io.observe(el); });
  })();
</script>
