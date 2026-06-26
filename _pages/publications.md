---
layout: page
permalink: /publications/
title: Publications
description: These are the representative publications of the past two five-year periods. For an up-to-date citation report and metrics, please visit my Google Scholar profile.
nav: true
nav_order: 2
---

<!-- ========================================================================== -->
<!-- 🎯 黄金工具栏：搜索框 + [高级冷调学术色合体]学术链接组 -->
<!-- ========================================================================== -->
<div class="search-and-icons-container" style="display: flex; justify-content: space-between; align-items: center; gap: 25px; margin-top: 15px; margin-bottom: 35px; flex-wrap: wrap;">
  
  <!-- 左侧：搜索过滤框（自动占满剩余空间） -->
  <div class="search-box-wrapper" style="flex: 1; min-width: 250px;">
    {% include bib_search.liquid %}
  </div>
  
  <!-- 右侧：图标+文字一体化的学术品牌大链接（色彩美化升级版） -->
  <div class="academic-icons-list" style="display: flex; gap: 22px; align-items: center; flex-wrap: wrap;">
    
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
  /* 🎨 复合超链接美化：升级为高对比度、更具活力的冷调高级学术色系 */
  /* ========================================================================== */
  .academic-icon-link {
    display: inline-flex;
    align-items: center;
    text-decoration: none !important;
    transition: transform 0.2s ease, opacity 0.2s ease, color 0.2s ease !important;
    font-weight: 500;
  }

  /* 放大矢量图标尺寸，使其与文字比例完美协调 */
  .academic-icon-link i {
    font-size: 1.6rem !important; 
    margin-right: 6px !important;  /* 图标和右侧文字之间留出精致微距 */
  }

  /* 定制链接文字样式，自带学术规范下划线 */
  .academic-icon-link .link-label {
    font-size: 1.05rem !important;
    text-decoration: underline !important;
  }
  
  /* 🎯 超链接色彩升级：比原先更亮丽适配、更具大厂设计感的冷调色 */
  .academic-icon-link.google-scholar { color: #2b6cb0 !important; } /* 深邃而高级的晴空蓝 */
  .academic-icon-link.scopus { color: #2c7a7b !important; }         /* 极其专业的深沉冷海绿 */
  .academic-icon-link.orcid { color: #4a7c2a !important; }          /* 端庄内敛的雨后松针绿 */
  
  /* 灵动交互：鼠标悬停整体同步微放大，极具现代质感 */
  .academic-icon-link:hover {
    transform: scale(1.04) !important;
    opacity: 0.8 !important;
  }

  /* 消除主题自带的搜索框底部多余间距，确保与右侧复合链接绝对齐平 */
  .search-box-wrapper input {
    margin-bottom: 0 !important;
  }

  /* ========================================================================== */
  /* 📊 终极三层阶梯切分：让标题、作者、期刊期卷页年份产生完美区分度 */
  /* ========================================================================== */

  /* 1. 🥇 第一梯队：论文标题（Title）—— 纯黑、强行加粗、突出主角地位 */
  .publications .title {
    font-weight: bold !important;      
    color: #111111 !important;         
    font-size: 1.15rem !important;     
    white-space: normal !important;    
    overflow: visible !important;      
    text-overflow: unset !important;   
    display: block !important;
    max-width: 100% !important;
    margin-bottom: 6px !important;     /* 与下方作者群留出舒适微距 */
  }

  /* 2. 🥈 第二梯队：作者名词群（Author）—— 降级为柔和烟灰色，使其内敛退后 */
  .publications .author {
    color: #555555 !important;         /* 烟灰色，让大段的合作者名字退居二线 */
    font-size: 1.0rem !important;
    display: block !important;         /* 强制作者群自成一块，绝不与下方期刊行混杂 */
    margin-bottom: 5px !important;     
  }
  
  /* 特殊保护：确保作者群里你自己的名字不受灰色影响，依然维持亮眼的纯黑和下划线 */
  .publications .author strong, 
  .publications .author u,
  .publications .author strong u {
    color: #111111 !important;
    font-weight: bold !important;
  }

  /* 3. 🥉 第三梯队：期刊详细信息行（Periodical）—— 换色为高贵绯红，全行（含年份）锁死斜体 */
  .publications .periodical {
    color: #941c2c !important;         /* 🎯 核心修改：换成极其惊艳、充满老牌名校底蕴的学术博雅红 */
    font-size: 1.0rem !important;
    font-weight: 500 !important;       
    font-style: italic !important;     /* 🎯 核心修改：强制让整行文本（包含期卷页码和末尾年份）全部化为优雅斜体 */
    display: block !important;         /* 强制这一行独立成块 */
  }
  
  /* 死锁期刊信息行内所有潜在嵌套子代、逗号及文本的色彩与斜体属性 */
  .publications .periodical *,
  .publications .periodical em,
  .publications .periodical i {
    color: #941c2c !important;         
    font-style: italic !important;
  }

  /* 4. 年份色彩：将右侧悬浮的大年份换成柔和的深炭灰色 */
  .publications h2.year, h2.year, .publications h2, .year {
    color: #444444 !important;   
    opacity: 1 !important;        
    font-weight: bold !important; 
  }

  /* 5. 列表松绑：让每篇论文之间留出极具呼吸感的空隙，拒绝拥挤 */
  .publications li {
    line-height: 1.8 !important;   
    margin-bottom: 32px !important;    
  }

  /* ========================================================================== */
  /* 🎨 其他辅助组件微调 */
  /* ========================================================================== */
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
