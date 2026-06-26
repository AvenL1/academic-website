---
layout: page
permalink: /publications/
title: Publications
description: These are the representative publications of the past two five-year periods. For an up-to-date citation report and metrics, please visit my Google Scholar profile.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

<style>
  /* 1. 极限扩大选择器范围，彻底清除乱码空格，将年份死死锁死为不透明纯黑 */
  .publications h2.year,
  h2.year,
  .publications h2,
  .year {
    color: #111111 !important;   /* 升级为更扎实高质感的纯深黑 */
    opacity: 1 !important;        /* 彻底剥离任何淡化和虚化效果 */
    font-weight: bold !important; /* 稳重加粗，让时间轴层次分明 */
  }

  /* 2. 让这一页的所有文字和列表松绑，告别紧凑 */
  p, li, .publications li {
    line-height: 1.8 !important;   /* 拉开行与行之间的距离 */
    margin-bottom: 16px !important; /* 让每一篇论文之间留出舒适的空隙 */
  }
</style>
