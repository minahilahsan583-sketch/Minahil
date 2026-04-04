---
layout: single
author_profile: false
---

<div class="hero-section">
  <p class="hero-label">Student Engineering Log</p>
  <h1 class="hero-title">Minahil Ahsan<br>Tech Practice Journal</h1>
  <p class="hero-excerpt">I am a Computer Engineering student focused on building intelligent, responsive, and user-centric software. This space serves as a log of my technical growth, research, and semester projects.</p>
  <div class="hero-buttons">
    <a href="{{ '/blog/' | relative_url }}" class="btn btn--primary">Read My Articles</a>
    <a href="{{ '/about/' | relative_url }}" class="btn btn--outline">About Me</a>
  </div>
</div>

<div class="posts-section">
  <h2 class="section-title">Latest Technical Insights</h2>
  <p class="section-subtitle">Recent notes from my weekly learning, university lab tasks, and AI research.</p>

  <div class="posts-list">
    {% for post in site.posts limit:6 %}
      <div class="post-card">
        <div class="post-card__image">
          <img src="{{ post.header.teaser | default: post.header.overlay_image | default: 'https://images.unsplash.com/photo-1517694712202-14dd9538aa97?q=80&w=600&auto=format&fit=crop' }}" alt="{{ post.title }}" loading="lazy">
        </div>
        <div class="post-card__body">
          <div class="post-card__meta">
            <span class="post-card__category">{{ post.categories | first | replace: "-", " " | capitalize }}</span>
            <span class="post-card__date">{{ post.date | date: "%d %b %Y" }}</span>
          </div>
          <h3 class="post-card__title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h3>
          <p class="post-card__excerpt">{{ post.excerpt | strip_html | truncate: 130 }}</p>
          <a href="{{ post.url | relative_url }}" class="post-card__link">Read more →</a>
        </div>
      </div>
    {% endfor %}
  </div>

  <div class="view-all">
    <a href="{{ '/blog/' | relative_url }}" class="btn btn--outline">View All Posts</a>
  </div>
</div>
