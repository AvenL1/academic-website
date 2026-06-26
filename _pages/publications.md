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
  /* 1. 将右侧年份换成较柔和但清晰可见的深炭灰色，并剔除虚化 */
  .publications h2.year,
  h2.year,
  .publications h2,
  .year {
    color: #444444 !important;   /* 柔和深灰色，清晰自然，告别死黑 */
    opacity: 1 !important;        /* 锁定100%不透明度，防止被系统自带的淡化效果影响 */
    font-weight: bold !important; /* 维持加粗，让时间轴层次分明 */
  }

  /* 2. 让这一页的所有文字和列表松绑，告别紧凑 */
  p, li, .publications li {
    line-height: 1.8 !important;   /* 拉开行与行之间的距离 */
    margin-bottom: 16px !important; /* 让每一篇论文之间留出舒适的空隙 */
  }
</style>
