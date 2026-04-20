---
layout: default
title: Accounting Issues
---

<section class="section">
    <div class="container">
        <h2 class="section-title">Accounting Issues</h2>
        <div class="content-card">
            <p>Discussions and analyses of current accounting issues, regulatory changes, and industry developments.</p>
        </div>
        
        {% if site.posts.size > 0 %}
        <div class="posts-list">
            {% for post in site.posts %}
            <article class="post-item">
                <h3 class="post-item-title">
                    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
                </h3>
                <p class="post-item-meta">
                    <time datetime="{{ post.date | date_to_xmlschema }}">
                        {{ post.date | date: "%B %d, %Y" }}
                    </time>
                </p>
                {% if post.excerpt %}
                <p class="post-item-excerpt">{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
                {% endif %}
            </article>
            {% endfor %}
        </div>
        {% else %}
        <div class="content-card">
            <p style="color: var(--text-light); font-style: italic;">No posts yet. Check back soon for updates!</p>
        </div>
        {% endif %}
        
        <!-- AdSense Placeholder -->
        <div class="ad-placeholder">
            <p>📢 Ad Space</p>
        </div>
    </div>
</section>

<style>
.posts-list {
    max-width: 800px;
}

.post-item {
    padding: 2rem 0;
    border-bottom: 1px solid var(--border-color);
}

.post-item:first-child {
    padding-top: 0;
}

.post-item-title {
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
}

.post-item-title a {
    color: var(--primary-color);
    text-decoration: none;
    border-bottom: 2px solid transparent;
    transition: border-color 0.2s ease;
}

.post-item-title a:hover {
    border-bottom-color: var(--accent-color);
}

.post-item-meta {
    color: var(--text-light);
    font-size: 0.9rem;
    margin-bottom: 0.75rem;
}

.post-item-excerpt {
    color: var(--text-dark);
    font-size: 0.95rem;
    line-height: 1.6;
}
</style>
