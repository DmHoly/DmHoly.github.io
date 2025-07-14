---
layout: default
title: "Projects"
permalink: /projects/
---

<h1 style="text-align:center;margin-bottom:30px;">Discover some of my Projects</h1>

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  margin: 0 auto 40px auto;
  padding: 0 32px;
  max-width: 1600px;
}
.project-card {
  background: #fff;
  border-radius: 18px;
  box-shadow: 0 4px 20px #0002;
  padding: 0 0 22px 0;
  transition: box-shadow 0.18s;
  display: flex;
  flex-direction: column;
  overflow: hidden;
  min-height: 400px;
}
.project-card:hover {
  box-shadow: 0 8px 30px #0003;
}
.project-img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  border-top-left-radius: 18px;
  border-top-right-radius: 18px;
  background: #eef4f7;
}
.project-title {
  font-size: 1.22em;
  color: #25798a;
  font-weight: 700;
  margin: 20px 22px 8px 22px;
}
.project-desc {
  font-size: 1em;
  color: #4e5865;
  margin: 0 22px 14px 22px;
}
.project-link {
  margin: 0 22px;
  align-self: flex-start;
  background: #2d9cbf;
  color: #fff;
  border-radius: 8px;
  padding: 7px 18px;
  font-size: 0.98em;
  text-decoration: none;
  font-weight: 500;
  transition: background 0.18s;
}
.project-link:hover {
  background: #176e8c;
}
</style>

<div class="projects-grid">
{% for project in site.data.portfolio %}
  <div class="project-card">
    {% if project.image %}
      <img class="project-img" src="{{ project.image }}" alt="{{ project.title }}">
    {% endif %}
    <div class="project-title">{{ project.title }}</div>
    <div class="project-desc">{{ project.description }}</div>
    {% if project.url %}
      <a class="project-link" href="{{ project.url }}" target="_blank">See the project</a>
    {% endif %}
  </div>
{% endfor %}
</div>
