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
  /* 1. 年份色彩：将右侧年份换成较柔和但清晰可见的深炭灰色，并剔除虚化 */
  .publications h2.year,
  h2.year,
  .publications h2,
  .year {
    color: #444444 !important;   /* 柔和深灰色，清晰自然，告别死黑 */
    opacity: 1 !important;        /* 锁定100%不透明度，防止被系统自带的淡化效果影响 */
    font-weight: bold !important; /* 维持加粗，让时间轴层次分明 */
  }

  /* 2. 严格局部隔离：🛠️ 只拉开论文主内容区（.publications）内的文字和列表间距，绝对不外泄给导航栏的 li */
  .publications p, 
  .publications li, 
  .publications a {
    line-height: 1.8 !important;   
  }
  
  .publications li {
    margin-bottom: 20px !important; /* 让每篇论文卡片之间留出舒适优雅的空隙 */
  }

  /* 3. 基础死锁：网页底层与导航栏 100% 锁死官方原生无衬线字体 */
  body, .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
  }

  /* 4. 精准正文替换：仅将论文卡片及列表内部的所有文本切换为端庄的 Times New Roman */
  .publications, 
  .publications * {
    font-family: "Times New Roman", Times, serif !important;
  }

  /* 5. 终极免疫防线：🛠️ 强行重置导航栏的行高与外边距，彻底粉碎任何潜在的排版渗透与变形 */
  .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
    line-height: 1.5 !important;      /* 强行让导航栏回归标准高度 */
    margin-bottom: 0 !important;      /* 彻底抹除论文列表带来的下边距污染 */
    margin-top: 0 !important;
  }
</style>
