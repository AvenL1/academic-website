---
layout: page
permalink: /publications/
title: Publications
description: These are the representative publications of the past two five-year periods. For an up-to-date citation report and metrics, please visit my Google Scholar profile.
nav: true
nav_order: 2
---

<!-- ========================================================================== -->
<!-- 🎯 完美并排升级版：搜索框 + [图标+文字一体化]学术大链接组（左右对齐） -->
<!-- ========================================================================== -->
<div class="search-and-icons-container" style="display: flex; justify-content: space-between; align-items: center; gap: 25px; margin-top: 15px; margin-bottom: 35px; flex-wrap: wrap;">
  
  <!-- 左侧：搜索过滤框（自动占满剩余空间） -->
  <div class="search-box-wrapper" style="flex: 1; min-width: 250px;">
    {% include bib_search.liquid %}
  </div>
  
  <!-- 右侧：图标+文字一体化的学术品牌大链接（对应图五复合超链接需求） -->
  <div class="academic-icons-list" style="display: flex; gap: 22px; align-items: center; flex-wrap: wrap;">
    
    <!-- 1. Google Scholar (图标+文字一体化超链接) -->
    <a href="https://scholar.google.com/citations?hl=en&user=wT0rZAQAAAAJ" target="_blank" class="academic-icon-link google-scholar" title="Google Scholar">
      <i class="ai ai-google-scholar"></i><span class="link-label">Google Scholar</span>
    </a>
    
    <!-- 2. Scopus (图标+文字一体化超链接) -->
    <a href="https://www.scopus.com/authid/detail.uri?authorId=57040217200" target="_blank" class="academic-icon-link scopus" title="Scopus">
      <i class="ai ai-scopus"></i><span class="link-label">Scopus</span>
    </a>
    
    <!-- 3. ORCID (图标+文字一体化超链接) -->
    <a href="https://orcid.org/0000-0002-4874-141X" target="_blank" class="academic-icon-link orcid" title="ORCID">
      <i class="ai ai-orcid"></i><span class="link-label">ORCID</span>
    </a>
    
  </div>

</div>

<div class="publications">

{% bibliography %}

</div>

<style>
  /* ========================================================================== */
  /* 🎨 复合超链接美化：图标与文字完美融合、锁定品牌色与悬停动效 */
  /* ========================================================================== */
  .academic-icon-link {
    display: inline-flex;
    align-items: center;
    text-decoration: none !important;
    transition: transform 0.2s ease, opacity 0.2s ease !important;
    font-family: "Times New Roman", Times, serif !important; /* 文字无缝继承端庄正文字体 */
    font-weight: 500;
  }

  /* 放大矢量图标尺寸，使其与文字比例完美协调 */
  .academic-icon-link i {
    font-size: 1.6rem !important; 
    margin-right: 6px !important;  /* 图标和右侧文字之间留出精致微距 */
  }

  /* 定制链接文字样式，自带学术规范下划线 */
  .academic-icon-link .link-label {
    font-size: 1.1rem !important;
    text-decoration: underline !important;
  }
  
  /* 统一为三大平台的官方标准品牌色（图标与文字共享颜色） */
  .academic-icon-link.google-scholar { color: #4285F4 !important; } /* 谷歌蓝 */
  .academic-icon-link.scopus { color: #007398 !important; }         /* Scopus 蓝绿 */
  .academic-icon-link.orcid { color: #A6CE39 !important; }          /* ORCID 官方绿 */
  
  /* 鼠标悬停整体（图标+文字）同步优雅放大并带有微透明反馈 */
  .academic-icon-link:hover {
    transform: scale(1.05) !important;
    opacity: 0.8 !important;
  }

  /* 消除主题自带的搜索框底部多余间距，确保与右侧复合链接绝对齐平 */
  .search-box-wrapper input {
    margin-bottom: 0 !important;
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
