---
layout: single
title: "My Blog & Tech Stories"
permalink: /blog/
author_profile: true
header:
  overlay_image: /assets/images/minahil_coding_1.png
  overlay_filter: 0.5
---

# Welcome to My Tech Blog

I love sharing my journey as a student engineer. Here, you'll find stories, tutorials, and reflections on my favorite topics in tech.

---

### Tech Story #1: My First University Exhibition

Participating in my first technical exhibition was a transformative experience. Under the guidance of **Dr. Bilal**, I learned not only how to build a complex project like the **Kidney Disease Prediction System** but also how to effectively present it to an audience.

- **Theme**: Machine Learning for Healthcare
- **Takeaway**: Communication is just as important as technical excellence.

---

### Tech Story #2: Mastering C++ as a Beginner

C++ can be intimidating, but it is the backbone of high-performance computing. In this story, I detail my learning path—from "Hello World" to building a simple object-oriented student database.

- **Focus**: Data structures, Pointers, Memory management.
- **Goal**: Build a solid foundation in low-level programming.

---

### Tech Story #3: Why I Chose Computer Engineering

Computer Engineering combines the best of both worlds—hardware and software. My passion for understanding how hardware and software interact led me to choose this path.

- **Interest**: Embedded systems, AI hardware, Integrated circuits.

---

### Tech Story #4: Exploring the World of Data With Python

Python is incredibly versatile. Whether it's web scraping, automation, or data analysis, it is my favorite tool for rapid prototyping and research.

---

# Recent Posts

{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%B %d, %Y" }})
{% endfor %}
