---
layout: home
title: 技术随笔
description: 分享编程知识和技术思考
---

# 欢迎来到草稿小站

![技术随笔封面](https://images.unsplash.com/photo-1555066931-4365d14bab8c?auto=format&fit=crop&w=1200&h=400&q=80)

## 最新文章

<div class="post-grid">
  {% for post in site.posts limit:3 %}
  <div class="post-card">
    <h3>{{ post.title }}</h3>
    <p class="post-date">{{ post.date | date: "%Y年%m月%d日" }}</p >
    <p>{{ post.excerpt | strip_html | truncate: 100 }}</p >
    阅读全文 →
  </div>
  {% endfor %}
</div>

<p>查看所有文章</p >

## 热门分类

- [Java 编程](/categories/java)
- [Web 开发](/categories/web)
- [数据库](/categories/database)
- [算法与数据结构](/categories/algorithms)
- [DevOps](/categories/devops)

## 关于本站

这个博客旨在分享实用的编程技术和开发经验。所有内容基于MIT协议开源，欢迎在提交改进建议。

**写作原则**：
1. 每篇文章解决一个具体问题
2. 提供可运行的代码示例
3. 保持内容定期更新

## 联系我

有技术问题想讨论？欢迎通过以下方式联系：

📧 电子邮件：3454812161@qq.com

<div class="newsletter">
  <h3>订阅更新</h3>
  <p>每月接收精选文章和技术动态</p >
  <form action="https://formspree.io/f/xanjrnpk" method="POST">
    <input type="email" name="email" placeholder="输入您的邮箱" required>
    <button type="submit">订阅</button>
  </form>
</div>

<link rel="stylesheet" href="/assets/css/main.css">
