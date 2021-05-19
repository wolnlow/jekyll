---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
{% if site.cdn.jsdelivr.enabled %}
{% assign assets_base_url = "https://cdn.jsdelivr.net/gh/wolnlow/jekyll" %}
{% endif %}
<body>
  <div class="index-wrapper">
    <div class="aside">
      <div class="info-card">
        <h1>waypig</h1>
        <h2>一只行走的猪</h2>
<a href="https://www.weibo.com/" target="_blank"><img src="{{ assets_base_url }}/js/weibo.png" alt="" width="22"/></a>
<a href="https://www.zhihu.com/" target="_blank"><img src="{{ assets_base_url }}/js/zhihu.png" alt="" width="22"/></a>
<a href="https://www.v2ex.com" target="_blank"><img src="{{ assets_base_url }}/js/v2ex.png" alt="" width="22"/></a>
<a href="https://www.bilibili.com" target="_blank"><img src="{{ assets_base_url }}/js/bilibili.png" alt="" width="22"/></a>
      </div>
      <div id="particles-js"></div>
      
    </div>
     <div class="index-content">
      <ul class="artical-list">
        {% for post in site.categories.blog %}
        <li>
          <a href="{{ post.url }}" class="title">{{ post.title }}</a>
          <div class="title-desc">{{ post.description }}</div>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</body>
