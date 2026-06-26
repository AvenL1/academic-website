---
layout: page
permalink: /publications/
title: Publications
description: These are the representative publications of the past two five-year periods. For an up-to-date citation report and metrics, please visit my Google Scholar profile.
nav: true
nav_order: 2
---

<!-- ========================================================================== -->
<!-- 🎯 黄金工具栏：搜索框 + [高端大尺寸图标组合]学术链接组 -->
<!-- ========================================================================== -->
<div class="search-and-icons-container" style="display: flex; justify-content: space-between; align-items: center; gap: 25px; margin-top: 15px; margin-bottom: 35px; flex-wrap: wrap;">
  
  <!-- 左侧：搜索过滤框（自动占满剩余空间） -->
  <div class="search-box-wrapper" style="flex: 1; min-width: 250px;">
    {% include bib_search.liquid %}
  </div>
  
  <!-- 右侧：图标完美放大、统一对齐的学术品牌大链接（对应图六优化需求） -->
  <div class="academic-icons-list" style="display: flex; gap: 25px; align-items: center; flex-wrap: wrap;">
    
    <!-- 1. Google Scholar -->
    <a href="https://scholar.google.com/citations?hl=en&user=wT0rZAQAAAAJ" target="_blank" class="academic-icon-link google-scholar" title="Google Scholar">
      <i class="ai ai-google-scholar"></i><span class="link-label">Google Scholar</span>
    </a>
    
    <!-- 2. Scopus -->
    <a href="https://www.scopus.com/authid/detail.uri?authorId=57040217200" target="_blank" class="academic-icon-link scopus" title="Scopus">
      <i class="ai ai-scopus"></i><span class="link-label">Scopus</span>
    </a>
    
    <!-- 3. ORCID -->
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
  /* 🎨 顶层大一统：强行让大标题 Publications 及正文全局锁定 Times New Roman */
  /* ========================================================================== */
  h1, .post-title, h1.post-title, .page-title, body, p, li, div, span, a, h2, h3, h4, h5, h6 {
    font-family: "Times New Roman", Times, serif !important;
  }

  /* ========================================================================== */
  /* 🎨 复合超链接美化：图标等比例放大、物理级齐平矫正样式 */
  /* ========================================================================== */
  .academic-icon-link {
    display: inline-flex;
    align-items: center;       /* 强行锁死：让图标与文字在任何分辨率下都绝对垂直居中 */
    justify-content: center;
    text-decoration: none !important;
    transition: transform 0.2s ease, opacity 0.2s ease, color 0.2s ease !important;
    font-weight: 500;
  }

  /* 🎯 核心修改：大幅放大矢量图标尺寸，拉满体量感，解决图六过小的问题 */
  .academic-icon-link i {
    font-size: 2.0rem !important;  /* 从 1.6rem 满血放大到 2.0rem，大小完美统一 */
    margin-right: 8px !important;  /* 稍微加宽间距，排版更加疏朗尊贵 */
    display: inline-flex;
    align-items: center;
  }

  /* 微调链接文字大小，使其与放大后的图标在视觉重量上达到黄金平衡 */
  .academic-icon-link .link-label {
    font-size: 1.1rem !important;
    text-decoration: underline !important;
    line-height: 1.0 !important;
  }
  
  /* 高级冷调学术色系 */
  .academic-icon-link.google-scholar { color: #2b6cb0 !important; } 
  .academic-icon-link.scopus { color: #2c7a7b !important; }         
  .academic-icon-link.orcid { color: #4a7c2a !important; }          
  
  /* 悬停动效 */
  .academic-icon-link:hover {
    transform: scale(1.04) !important;
    opacity: 0.8 !important;
  }

  /* 消除搜索框底部多余间距 */
  .search-box-wrapper input {
    margin-bottom: 0 !important;
  }

  /* ========================================================================== */
  /* 📊 终极三层阶梯切分样式（博雅红斜体版） */
  /* ========================================================================== */

  /* 1. 🥇 第一梯队：论文标题（Title） */
  .publications .title {
    font-weight: bold !important;      
    color: #111111 !important;         
    font-size: 1.15rem !important;     
    white-space: normal !important;    
    overflow: visible !important;      
    text-overflow: unset !important;   
    display: block !important;
    max-width: 100% !important;
    margin-bottom: 6px !important;     
  }

  /* 2. 🥈 第二梯队：作者名词群（Author） */
  .publications .author {
    color: #555555 !important;         
    font-size: 1.0rem !important;
    display: block !important;         
    margin-bottom: 5px !important;     
  }
  
  .publications .author strong, 
  .publications .author u,
  .publications .author strong u {
    color: #111111 !important;
    font-weight: bold !important;
  }

  /* 3. 🥉 第三梯队：期刊详细信息行（Periodical） */
  .publications .periodical {
    color: #941c2c !important;         
    font-size: 1.0rem !important;
    font-weight: 500 !important;       
    font-style: italic !important;     
    display: block !important;         
  }
  
  .publications .periodical *,
  .publications .periodical em,
  .publications .periodical i {
    color: #941c2c !important;         
    font-style: italic !important;
  }

  /* 4. 年份色彩 */
  .publications h2.year, h2.year, .publications h2, .year {
    color: #444444 !important;   
    opacity: 1 !important;        
    font-weight: bold !important; 
  }

  /* 5. 列表松绑 */
  .publications li {
    line-height: 1.8 !important;   
    margin-bottom: 32px !important;    
  }

  /* 6. 其他辅助组件 */
  .publications abbr.badge, .publications .badge {
    background-color: #b0129a !important; 
    color: #ffffff !important;
    padding: 4px 10px !important;
    border-radius: 4px !important;
    font-family: -apple-system, BlinkMacSystemFont, sans-serif !important; 
    font-weight: bold !important;
    display: inline-block !important;
    margin-right: 8px !important;
  }

  .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
    line-height: 1.5 !important;
    margin-bottom: 0 !important;
    margin-top: 0 !important;
  }
</style>
