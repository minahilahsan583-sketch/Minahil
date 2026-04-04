layout: single
author_profile: false
header:
  overlay_filter: 0.1
  caption: "Minahil Ahsan - Tech Journal"
excerpt: "I am a Computer Engineering student building simple and responsive systems using Modern Tech. This blog shows my practice work and weekly progress."
---

<div class="page__hero-content">
  <p style="color: var(--primary-color); font-weight: 600; font-family: 'Poppins'; margin-bottom: 0;">Student Engineering Log</p>
  <h1 class="page__hero-title">Minahil Ahsan - Tech Practice Journal</h1>
  <p class="pager__hero-excerpt">I am a Computer Engineering student focused on building intelligent, responsive, and user-centric software. This space serves as a log of my technical growth, research, and semester projects.</p>
  <div style="display: flex; gap: 15px; margin-top: 2rem;">
    <a href="/blog/" class="btn btn--primary">Read My Articles</a>
    <a href="/about/" class="btn btn--info">About Me</a>
  </div>
</div>

---

<h2 style="font-family: 'Space Grotesk'; font-size: 2rem; margin: 3rem 0 1.5rem;">Latest Technical Insights</h2>
<p style="color: var(--muted-text); margin-bottom: 3rem;">Recent notes from my weekly learning, university lab tasks, and AI research.</p>

<div class="entries-list">
  {% for post in site.posts limit:5 %}
    <div class="grid__item">
      <article class="archive__item">
        <div class="archive__item-teaser">
          <img src="{{ post.header.teaser | default: post.header.overlay_image | default: '/assets/images/minahil_coding_1.png' }}" alt="{{ post.title }}">
        </div>
        <div class="archive__item-body">
          <p style="font-size: 0.8rem; color: var(--primary-color); font-weight: 600; text-transform: uppercase; margin-bottom: 0.5rem; display: flex; justify-content: space-between;">
            <span>{{ post.categories | first | replace: "-", " " }}</span>
            <span style="color: var(--muted-text); font-weight: 400;">{{ post.date | date: "%d %b %Y" }}</span>
          </p>
          <h2 class="archive__item-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>
          <p class="archive__item-excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
        </div>
      </article>
    </div>
  {% endfor %}
</div>

<div style="text-align: center; margin-top: 3rem;">
  <a href="/blog/" class="btn btn--info">View All Practice Logs</a>
</div>
