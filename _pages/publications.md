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
  /* 1. 精准控制：将右侧年份换成较柔和但清晰可见的深炭灰色，并剔除虚化 */
  .publications h2.year,
  h2.year,
  .publications h2,
  .year {
    color: #444444 !important;   /* 柔和深灰色，清晰自然，告别死黑 */
    opacity: 1 !important;        /* 锁定100%不透明度，防止被系统自带的淡化效果影响 */
    font-weight: bold !important; /* 维持加粗，让时间轴层次分明 */
  }

  /* 2. 呼吸间距：让这一页的所有文字和列表松绑，告别紧凑 */
  p, li, .publications li {
    line-height: 1.8 !important;   /* 拉开行与行之间的距离 */
    margin-bottom: 16px !important; /* 让每一篇论文之间留出舒适的空隙 */
  }

  /* 3. 尺寸死锁：网页底层与导航栏 100% 锁死官方原生无衬线字体，确保换页时任务栏尺寸、高度绝对静止 */
  body, .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
  }

  /* 4. 学术正文区：精准将各个板块内部的介绍、卡片、论文列表切换为端庄的 Times New Roman */
  p, li, h1, h2, h3, h4, h5, h6,
  .about, .about *, 
  .publications, .publications *, 
  .projects, .projects *, 
  .teaching-list, .teaching-list *, 
  .grants-list, .grants-list * {
    font-family: "Times New Roman", Times, serif !important;
  }

  /* 5. 安全防线：确保导航栏内部的任何嵌套子元素绝对不会被上面的正文规则错误污染 */
  .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
  }
</style>
