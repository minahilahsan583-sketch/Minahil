---
layout: single
author_profile: true
header:
  overlay_image: /assets/images/minahil_intro_1.png
  overlay_filter: 0.6
  caption: "Computer Engineering Student & ML Enthusiast"
  actions:
    - label: "View Portfolio"
      url: "/portfolio/"
    - label: "Read Blog"
      url: "/blog/"
excerpt: "Transforming complex problems into elegant software solutions. Passionate about AI, Machine Learning, and Modern Web Technologies."
---

# 🚀 Welcome to My Digital Space

I'm **Minahil Ahsan**, a Computer Engineering student dedicated to mastering the art of software development and artificial intelligence. My work sits at the intersection of rigorous engineering and creative problem-solving.

---

## 🌟 Featured Insights

Explore some of my recent thoughts and technical deep-dives.

<div class="grid__wrapper">
  {% for post in site.posts limit:3 %}
    <div class="grid__item">
      <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork">
        <div class="archive__item-teaser">
          <img src="{{ post.header.teaser | default: post.header.overlay_image | default: '/assets/images/minahil_coding_1.png' }}" alt="{{ post.title }}">
        </div>
        <h2 class="archive__item-title no_toc" itemprop="headline">
          <a href="{{ post.url | relative_url }}" rel="permalink">{{ post.title }}</a>
        </h2>
        <p class="archive__item-excerpt" itemprop="description">{{ post.excerpt | strip_html | truncate: 120 }}</p>
      </article>
    </div>
  {% endfor %}
</div>

<div style="text-align: center; margin-top: 1em;">
  <a href="/blog/" class="btn btn--primary">View All Posts</a>
</div>

---

## 👩‍💻 About Me

I am currently pursuing my degree in Computer Engineering, where I specialize in **Software Engineering** and **Machine Learning**. My journey is driven by a desire to build intelligent systems that serve the community and advance technological frontiers.

### My Core Mission
> "To innovate and implement technology that simplifies life, empowers individuals, and contributes to the progress of my country."

<div style="text-align: center;">
  <a href="/about/" class="btn btn--info">Read My Story</a>
</div>

---

## 🛠️ Technical Toolkit

A glimpse into the technologies and tools I work with:

| Category | Skills |
| :--- | :--- |
| **Languages** | C++, Python, JavaScript, SQL |
| **AI/ML** | TensorFlow, Scikit-learn, Data Analysis |
| **Web Dev** | Jekyll, HTML5, CSS3, Modern UI/UX |
| **Tools** | Git, VS Code, MATLAB, Linux |

---

## 🤝 Let's Collaborate

Whether you have a question about my projects or just want to say hi, I'm always open to connecting with fellow tech enthusiasts and professionals.

<div style="display: flex; gap: 10px; justify-content: center; flex-wrap: wrap;">
  <a href="/contact/" class="btn btn--primary">Get in Touch</a>
  <a href="/portfolio/" class="btn btn--inverse">Explore Portfolio</a>
</div>
