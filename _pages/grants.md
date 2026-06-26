---
layout: page
title: Research Grants
permalink: /grants/
nav: true
nav_order: 4     # 🛠️ 导航栏排序，4 代表它会排在 Patents 和 Teaching 之间
---

<div class="grants-list" style="line-height: 1.8; margin-top: 30px;">

  <div style="background: #f4f9fc; border-left: 5px solid #3182ce; padding: 16px 20px; border-radius: 0 6px 6px 0; box-shadow: 0 1px 4px rgba(0,0,0,0.04); margin-bottom: 20px;">
    <div style="display: flex; flex-direction: column; gap: 8px; align-items: flex-start;">
      <span style="font-weight: bold; color: #111; font-size: 1.1rem;">Quasi-Single-Crystalline Perovskite Photovoltaic Modules</span>
      <span style="background: #e1f5fe; color: #0288d1; border: 1px solid #b3e5fc; padding: 3px 10px; border-radius: 4px; font-size: 0.85em; font-weight: bold; letter-spacing: 0.5px;">1.07M | ITF-ITSP</span>
    </div>
    <div style="color: #666; font-size: 0.95rem; margin-top: 8px;"><i class="far fa-calendar-alt" style="margin-right: 5px;"></i> Timeline: 01/2026 - 06/2027</div>
  </div>

  <div style="background: #f4f9fc; border-left: 5px solid #3182ce; padding: 16px 20px; border-radius: 0 6px 6px 0; box-shadow: 0 1px 4px rgba(0,0,0,0.04); margin-bottom: 20px;">
    <div style="display: flex; flex-direction: column; gap: 8px; align-items: flex-start;">
      <span style="font-weight: bold; color: #111; font-size: 1.1rem;">Investigation on Ionic Liquids based Green Solvent System for Environmentally Friendly Printing of stable perovskite solar modules</span>
      <span style="background: #e1f5fe; color: #0288d1; border: 1px solid #b3e5fc; padding: 3px 10px; border-radius: 4px; font-size: 0.85em; font-weight: bold; letter-spacing: 0.5px;">0.3M | NSFC Young Scientists</span>
    </div>
    <div style="color: #666; font-size: 0.95rem; margin-top: 8px;"><i class="far fa-calendar-alt" style="margin-right: 5px;"></i> Timeline: 01/2025 - 12/2027</div>
  </div>

  <div style="background: #f4f9fc; border-left: 5px solid #3182ce; padding: 16px 20px; border-radius: 0 6px 6px 0; box-shadow: 0 1px 4px rgba(0,0,0,0.04); margin-bottom: 20px;">
    <div style="display: flex; flex-direction: column; gap: 8px; align-items: flex-start;">
      <span style="font-weight: bold; color: #111; font-size: 1.1rem;">Multifunctional Surfactant-Assisted Printing of Large-Area High-Efficiency and Stable Perovskite Solar Cells and Modules</span>
      <span style="background: #e1f5fe; color: #0288d1; border: 1px solid #b3e5fc; padding: 3px 10px; border-radius: 4px; font-size: 0.85em; font-weight: bold; letter-spacing: 0.5px;">0.1M | Guangdong Regional Joint Fund</span>
    </div>
    <div style="color: #666; font-size: 0.95rem; margin-top: 8px;"><i class="far fa-calendar-alt" style="margin-right: 5px;"></i> Timeline: 01/2021 - 12/2023</div>
  </div>

  <div style="background: #f4f9fc; border-left: 5px solid #3182ce; padding: 16px 20px; border-radius: 0 6px 6px 0; box-shadow: 0 1px 4px rgba(0,0,0,0.04); margin-bottom: 20px;">
    <div style="display: flex; flex-direction: column; gap: 8px; align-items: flex-start;">
      <span style="font-weight: bold; color: #111; font-size: 1.1rem;">Investigation for the ambient air blade coating of large-area printable perovskite photovoltaics modules</span>
      <span style="background: #e1f5fe; color: #0288d1; border: 1px solid #b3e5fc; padding: 3px 10px; border-radius: 4px; font-size: 0.85em; font-weight: bold; letter-spacing: 0.5px;">0.25M | PolyU Start-up Fund</span>
    </div>
    <div style="color: #666; font-size: 0.95rem; margin-top: 8px;"><i class="far fa-calendar-alt" style="margin-right: 5px;"></i> Timeline: 07/2022 - 06/2024</div>
  </div>

</div>

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
