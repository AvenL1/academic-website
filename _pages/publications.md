---
layout: page
permalink: /publications/
title: Publications
description: These are the representative publications of the past two five-year periods. For an up-to-date citation report and metrics, please visit my Google Scholar profile.
nav: true
nav_order: 2
---

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

<style>
  /* 1. 大标题与正文对齐：全面锁死为优雅端庄的 Times New Roman */
  body, p, li, div, span, a, h1, h2, h3, h4, h5, h6, .post-title, .title {
    font-family: "Times New Roman", Times, serif !important;
  }

  /* 2. 绝对隔离栏：强制让顶部导航栏维持官方原生的现代无衬线字体，换页时尺寸完全静止 */
  .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
    line-height: 1.5 !important;
    margin-bottom: 0 !important;
    margin-top: 0 !important;
  }

  /* 3. 年份色彩：将右侧年份换成较柔和但清晰可见的深炭灰色 */
  .publications h2.year, h2.year, .publications h2, .year {
    color: #444444 !important;   
    opacity: 1 !important;        
    font-weight: bold !important; 
  }

  /* 4. 列表松绑：让这一页的所有论文卡片拉开舒适优雅的间距 */
  .publications p, .publications li {
    line-height: 1.8 !important;   
  }
  .publications li {
    margin-bottom: 20px !important; 
  }

  /* 5. 🎨 期刊标签满血复活：强制恢复 Nat. Comm. 等期刊的彩色背景与白字，拒绝单调 */
  .publications abbr.badge, 
  .publications .badge {
    background-color: #b0129a !important; /* 完美复原经典的学术高质感品红/紫罗兰底色 */
    color: #ffffff !important;
    padding: 4px 10px !important;
    border-radius: 4px !important;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important; /* 标签内文字用无衬线更清晰 */
    font-weight: bold !important;
    display: inline-block !important;
    margin-right: 8px !important;
  }
</style>
