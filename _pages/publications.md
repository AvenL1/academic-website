---
layout: page
permalink: /publications/
title: Publications
description: These are the representative publications of the past two five-year periods. For an up-to-date citation report and metrics, please visit my Google Scholar profile.
nav: true
nav_order: 2
---

<div class="academic-profiles" style="margin-top: -10px; margin-bottom: 30px; font-size: 1.05rem; color: #222; font-family: 'Times New Roman', Times, serif;">
  Find me on 
  <a href="https://scholar.google.com/citations?user=https://scholar.google.com/citations?hl=en&user=wT0rZAQAAAAJ" target="_blank" class="academic-link">Google Scholar</a>, 
  <a href="https://www.scopus.com/authid/detail.uri?authorId=57040217200" target="_blank" class="academic-link">Scopus</a>, and 
  <a href="https://orcid.org/0000-0002-4874-141X" target="_blank" class="academic-link">ORCID</a>.
</div>

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

<style>
  /* 🔗 链接美化：定制学术超链接的专属蓝色、下划线与悬停变色动效 */
  .academic-link {
    color: #106ba3 !important;
    text-decoration: underline !important;
    transition: color 0.2s ease-in-out;
  }
  .academic-link:hover {
    color: #005A32 !important; /* 鼠标悬停时呈现优雅的学术绿 */
  }

  /* 1. 🎯 核心修复：让论文标题（Title）变明显，并彻底解决名字“残缺/截断”问题 */
  .publications .title {
    font-family: "Times New Roman", Times, serif !important;
    font-weight: bold !important;      /* 强行加粗，让论文题目极为醒目、突出 */
    color: #111111 !important;         /* 采用更深、更有高质感的纯深黑色 */
    font-size: 1.15rem !important;     /* 字号稍微放大，建立完美学术主次层级 */
    
    /* 强行解除任何潜在的单行截断和溢出隐藏，确保论文名字 100% 完整完整展现 */
    white-space: normal !important;    
    overflow: visible !important;      
    text-overflow: unset !important;   
    display: block !important;
    max-width: 100% !important;
    margin-bottom: 6px !important;     /* 与下方的作者名字留出舒适的微距 */
  }

  /* 2. 辅助烘托：使作者与期刊名字稍显低调，以衬托上方论文标题的绝对主角地位 */
  .publications .author,
  .publications .periodical {
    font-family: "Times New Roman", Times, serif !important;
    color: #444444 !important;         /* 使用柔和的深灰色 */
    font-size: 1.0rem !important;
  }

  /* 3. 年份色彩：将右侧年份换成较柔和但清晰可见的深炭灰色 */
  .publications h2.year,
  h2.year,
  .publications h2,
  .year {
    color: #444444 !important;   
    opacity: 1 !important;        
    font-weight: bold !important; 
    font-family: "Times New Roman", Times, serif !important;
  }

  /* 4. 列表松绑：让这一页的所有文字和论文列表留出舒适优雅的空隙 */
  p, li, .publications li {
    line-height: 1.8 !important;   
    margin-bottom: 16px !important; 
    font-family: "Times New Roman", Times, serif !important;
  }

  /* 5. 🎨 期刊彩色标签复原：确保 Nat. Comm. 等期刊徽章背景与颜色醒目闪亮 */
  .publications abbr.badge, 
  .publications .badge {
    background-color: #b0129a !important; /* 完美复原经典的学术高质感品红/紫罗兰底色 */
    color: #ffffff !important;
    padding: 4px 10px !important;
    border-radius: 4px !important;
    font-family: -apple-system, BlinkMacSystemFont, sans-serif !important; 
    font-weight: bold !important;
    display: inline-block !important;
    margin-right: 8px !important;
  }

  /* 6. 顶栏绝对死锁：确保换页时顶部任务栏在尺寸、字体和高度上绝对静止，坚决不发生任何抖动 */
  .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
    line-height: 1.5 !important;
    margin-bottom: 0 !important;
    margin-top: 0 !important;
  }
</style>
