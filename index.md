---
layout: default
title: 技术知识库
description: 计算机科学与交通工程专业技术文章
nav_order: 1
---

# 欢迎访问技术知识库

本知识库专注于分享计算机科学与交通工程领域的前沿技术文章和实践经验。

<div class="row">
  <div class="col">
    <div class="card computer-science">
      <h2><i class="fas fa-laptop-code"></i> 计算机科学</h2>
      <ul>
        <li><a href="/docs/computer-science/algorithms">算法与数据结构</a></li>
        <li><a href="/docs/computer-science/system-design">系统设计</a></li>
        <li><a href="/docs/computer-science/programming">编程语言</a></li>
        <li><a href="/docs/computer-science/database">数据库技术</a></li>
        <li><a href="/docs/computer-science/cloud">云计算</a></li>
      </ul>
    </div>
  </div>
  
  <div class="col">
    <div class="card transportation">
      <h2><i class="fas fa-traffic-light"></i> 交通工程</h2>
      <ul>
        <li><a href="/docs/transportation/traffic-flow">交通流理论</a></li>
        <li><a href="/docs/transportation/transportation-planning">交通规划</a></li>
        <li><a href="/docs/transportation/intelligent-transport">智能交通系统</a></li>
        <li><a href="/docs/transportation/simulation">交通仿真技术</a></li>
        <li><a href="/docs/transportation/safety">交通安全</a></li>
      </ul>
    </div>
  </div>
</div>

<div class="card">
  <h2><i class="fas fa-newspaper"></i> 最新文章</h2>
  

{% for post in site.posts limit:5 %}
<div class="article">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <div class="meta">
    <span class="category {{ post.category | downcase | replace: ' ', '-' }}">{{ post.category }}</span>
    <span class="date">{{ post.date | date: "%Y年%m月%d日" }}</span>
  </div>
  <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
</div>
{% endfor %}
  
  <div class="article">
    <h3><a href="/docs/transportation/v2x">V2X通信技术在智能交通系统中的应用</a></h3>
    <div class="meta">
      <span class="category transportation">交通工程</span>
      <span class="date">2023年10月10日</span>
    </div>
    <p>深入分析车路协同(V2X)技术的通信协议、安全机制及其在拥堵缓解中的应用...</p>
  </div>
  
  <div class="article">
    <h3><a href="/docs/computer-science/gis">GIS技术在交通工程中的应用实践</a></h3>
    <div class="meta">
      <span class="category hybrid">交叉领域</span>
      <span class="date">2023年10月5日</span>
    </div>
    <p>地理信息系统(GIS)在交通需求分析、路网规划和事故热点识别中的应用案例研究...</p>
  </div>
</div>

<h2>资源下载</h2>
<div class="resources">
  <a href="#" class="resource">
    <i class="fas fa-file-pdf"></i>
    <span>交通工程计算工具包</span>
  </a>
  <a href="#" class="resource">
    <i class="fas fa-code"></i>
    <span>Python交通分析库</span>
  </a>
  <a href="#" class="resource">
    <i class="fas fa-book"></i>
    <span>计算机算法手册</span>
  </a>
</div>
