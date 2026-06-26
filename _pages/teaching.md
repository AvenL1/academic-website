---
layout: page
title: Teaching
permalink: /teaching/
nav: true
nav_order: 5
---

<div class="teaching-list" style="line-height: 1.8; margin-top: 30px;">

  <!-- 课程 1 -->
  <div class="teaching-item" style="margin-bottom: 35px; padding-bottom: 25px; border-bottom: 1px solid #e2ece9; display: flex; align-items: flex-start; gap: 25px;">
    <div style="min-width: 120px; color: #005A32; font-weight: bold; font-size: 1.05rem;">2022 — 2023</div>
    <div>
      <div style="font-weight: bold; color: #111; font-size: 1.15rem; display: flex; align-items: center; gap: 12px; flex-wrap: wrap;">
        Logic Design
        <!-- 🔗 绑定PDF：target="_blank" 确保在新标签页干净利落地打开，不影响当前网站 -->
        <a href="{{ '/assets/pdf/EIE2211_SDF_2025.pdf' | relative_url }}" target="_blank" style="background: #f0f7f4; color: #005A32; border: 1px solid #a3cbd6; padding: 2px 10px; border-radius: 4px; font-size: 0.85rem; font-weight: bold; text-decoration: none; transition: all 0.2s;" onmouseover="this.style.background='#005A32';this.style.color='#fff';" onmouseout="this.style.background='#f0f7f4';this.style.color='#005A32';">EIE2211 ↗</a>
      </div>
      <div style="color: #444; font-size: 1.05rem; margin-top: 6px;">The Hong Kong Polytechnic University</div>
      <div style="color: #666; font-size: 0.95rem; margin-top: 4px; font-style: italic;">Academic Year: 2022/23</div>
    </div>
  </div>

  <!-- 课程 2 -->
  <div class="teaching-item" style="margin-bottom: 35px; padding-bottom: 25px; display: flex; align-items: flex-start; gap: 25px;">
    <div style="min-width: 120px; color: #005A32; font-weight: bold; font-size: 1.05rem;">2023 — 2026</div>
    <div>
      <div style="font-weight: bold; color: #111; font-size: 1.15rem; display: flex; align-items: center; gap: 12px; flex-wrap: wrap;">
        Optoelectronic Devices
        <!-- 🔗 绑定PDF：target="_blank" 确保在新标签页干净利落地打开，不影响当前网站 -->
        <a href="{{ '/assets/pdf/EIE577.pdf' | relative_url }}" target="_blank" style="background: #f0f7f4; color: #005A32; border: 1px solid #a3cbd6; padding: 2px 10px; border-radius: 4px; font-size: 0.85rem; font-weight: bold; text-decoration: none; transition: all 0.2s;" onmouseover="this.style.background='#005A32';this.style.color='#fff';" onmouseout="this.style.background='#f0f7f4';this.style.color='#005A32';">EIE577 ↗</a>
      </div>
      <div style="color: #444; font-size: 1.05rem; margin-top: 6px;">The Hong Kong Polytechnic University</div>
      <div style="color: #666; font-size: 0.95rem; margin-top: 4px; font-style: italic;">Academic Years: 2023/24, 2024/25, 2025/26</div>
    </div>
  </div>

</div>

<!-- ========================================== -->
<!-- GLOBAL FONTS OVERRIDE -->
<!-- ========================================== -->
<!-- ========================================== -->
<!-- 全站导航栏尺寸死锁与内容字体对齐金装补丁 -->
<!-- ========================================== -->
<style>
  /* 1. 网页底层与导航栏：100% 锁死官方原生无衬线字体，确保换页时任务栏尺寸、高度绝对静止 */
  body, .navbar, .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
  }

  /* 2. 学术正文区：精准将各个板块内部的介绍、卡片、论文列表切换为端庄的 Times New Roman */
  p, li, h1, h2, h3, h4, h5, h6,
  .about, .about *, 
  .publications, .publications *, 
  .projects, .projects *, 
  .teaching-list, .teaching-list *, 
  .grants-list, .grants-list * {
    font-family: "Times New Roman", Times, serif !important;
  }

  /* 3. 安全防线：确保导航栏内部的任何嵌套子元素绝对不会被上面的正文规则错误污染 */
  .navbar *, .nav-link, .nav-item, .navbar-brand {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
  }
</style>
