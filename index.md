---
layout: default
title: Inicio
---

# 👋 Hola, Soy Gustavo Martinez

## 🧮 Científico de Datos & Matemático

Estudiante de Matemáticas apasionado por la ciencia de datos e inteligencia artificial. Experiencia en extracción de insights valiosos a partir de grandes conjuntos de datos, como lo demuestran mis proyectos.

---

## 📊 Proyectos Destacados

{% for post in site.posts limit:3 %}
<div class="project-card">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt }}</p>
  <div class="project-meta">
    <span class="tech-stack">{{ post.technologies }}</span>
    {% if post.github %}
    <a href="{{ post.github }}" class="github-link">📁 GitHub</a>
    {% endif %}
  </div>
</div>
{% endfor %}

<div class="view-all">
  <a href="/proyectos" class="btn-primary">Ver Todos los Proyectos →</a>
</div>

---

## 🛠️ Habilidades Técnicas

<div class="skills-grid">
  <div class="skill-category">
    <h3> Lenguajes</h3>
    <ul>
      <li>Python (Pandas, NumPy, Scikit-learn)</li>
      <li>R (Tidyverse, ggplot2)</li>
      <li>SQL (PostgreSQL, MySQL)</li>
      <li>JavaScript (D3.js)</li>
    </ul>
  </div>
  
  <div class="skill-category">
    <h3> Machine Learning</h3>
    <ul>
      <li>Scikit-learn, TensorFlow, PyTorch</li>
      <li>Análisis Supervisado y No Supervisado</li>
      <li>Deep Learning (CNN, RNN)</li>
      <li>NLP y Computer Vision</li>
    </ul>
  </div>
  
  <div class="skill-category">
    <h3>📊 Visualización</h3>
    <ul>
      <li>Matplotlib, Seaborn, Plotly</li>
      <li>Tableau, Power BI</li>
      <li>Streamlit, Dash</li>
      <li>D3.js, Chart.js</li>
    </ul>
  </div>
</div>

---

## 💼 Experiencia

<div class="experience-timeline">
  <div class="exp-item">
    <h3>🧮 Científico de Datos Jr.</h3>
    <p class="company">[Empresa] | 2023 - Presente</p>
    <ul>
      <li>Desarrollo de modelos de ML para predicción</li>
      <li>Análisis de datos de clientes</li>
      <li>Creación de dashboards interactivos</li>
    </ul>
  </div>
  
  <div class="exp-item">
    <h3>📊 Analista de Datos</h3>
    <p class="company">[Empresa] | 2022 - 2023</p>
    <ul>
      <li>Limpieza y preparación de datos</li>
      <li>Análisis estadístico descriptivo</li>
      <li>Generación de reportes automatizados</li>
    </ul>
  </div>
</div>

---

## 📧 Contacto

<div class="contact-info">
  <div class="contact-item">
    <strong>📧 Email:</strong> gustavo.martinez@email.com
  </div>
  <div class="contact-item">
    <strong> LinkedIn:</strong> <a href="[Tu LinkedIn]">Perfil de LinkedIn</a>
  </div>
  <div class="contact-item">
    <strong> GitHub:</strong> <a href="[Tu GitHub]">Perfil de GitHub</a>
  </div>
  <div class="contact-item">
    <strong> Ubicación:</strong> Ciudad, País
  </div>
</div> 