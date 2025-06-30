---
layout: page
title: Proyectos
permalink: /proyectos/
---

# �� Mis Proyectos de Ciencia de Datos

<div class="project-filters">
  <button class="filter-btn active" data-filter="all">Todos</button>
  <button class="filter-btn" data-filter="ml">Machine Learning</button>
  <button class="filter-btn" data-filter="eda">Análisis de Datos</button>
  <button class="filter-btn" data-filter="viz">Visualización</button>
  <button class="filter-btn" data-filter="nlp">NLP</button>
</div>

<div class="projects-grid">
  {% for post in site.posts %}
  <div class="project-card" data-category="{{ post.category }}">
    <div class="project-image">
      {% if post.image %}
      <img src="{{ post.image }}" alt="{{ post.title }}">
      {% endif %}
    </div>
    <div class="project-content">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
      <div class="project-meta">
        <span class="category">{{ post.category | upcase }}</span>
        <span class="tech">{{ post.technologies }}</span>
      </div>
      <div class="project-links">
        {% if post.github %}
        <a href="{{ post.github }}" class="btn-secondary">�� Código</a>
        {% endif %}
        {% if post.demo %}
        <a href="{{ post.demo }}" class="btn-primary">🚀 Demo</a>
        {% endif %}
      </div>
    </div>
  </div>
  {% endfor %}
</div> 