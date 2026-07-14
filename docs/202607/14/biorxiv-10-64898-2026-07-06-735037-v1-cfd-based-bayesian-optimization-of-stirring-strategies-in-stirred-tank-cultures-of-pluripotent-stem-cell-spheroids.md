---
title: CFD-based Bayesian Optimization of Stirring Strategies in Stirred Tank Cultures of Pluripotent Stem Cell Spheroids
title_zh: 基于CFD的多能干细胞球体搅拌罐培养中搅拌策略的贝叶斯优化
authors: "Horiguchi, I., Okada, K., Okano, Y."
date: 2026-07-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.735037v1.full.pdf"
tags: ["query:equipment"]
score: 6.0
evidence: CFD优化搅拌策略方法可迁移至双行星搅拌器混合机理分析
tldr: 多能干细胞球在搅拌罐中悬浮培养需平衡分散性与低剪切应力。本研究采用CFD-DPM模拟iPS细胞球运动，并通过贝叶斯优化设计两阶段搅拌策略：先高速重悬，后低速维持悬浮。优化策略提高了浮动率并降低了滑移速度，减少机械应力。为可放大的iPS细胞制造提供了工程见解。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 711, \"height\": 502, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 709, \"height\": 559, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 704, \"height\": 608, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1359, \"height\": 590, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1378, \"height\": 452, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1384, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 123, \"height\": 94, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 535, \"height\": 376, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 488, \"height\": 425, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 474, \"height\": 196, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 392, \"height\": 244, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 388, \"height\": 240, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 399, \"height\": 296, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 394, \"height\": 294, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-735037-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1268, \"height\": 329, \"label\": \"Table\"}]"
motivation: 搅拌罐中iPS细胞球悬浮培养需同时保证均匀分散与低剪切应力，现有搅拌策略难以兼顾。
method: 将CFD-DPM模拟与贝叶斯优化结合，以粒子浮动率和滑移速度为优化目标，搜索时间依赖的搅拌速度曲线。
result: 优化得到两阶段策略：初始高转速快速重悬，后续低转速维持悬浮，浮动率提升且滑移速度降低。
conclusion: 贝叶斯优化可有效设计搅拌方案，为大规模iPS细胞培养提供低应力悬浮策略。
---

## 摘要
在搅拌式生物反应器中悬浮培养多能干细胞需要在保持细胞均匀分散和避免过高剪切应力（可能损害细胞活力和多能性）之间取得精细平衡。本研究采用计算流体动力学（CFD）结合离散颗粒法（DPM）模拟iPS细胞在5 mL三角叶轮搅拌罐中的行为。分析表明，罐底的向上流和罐顶的向下流对于维持稳定悬浮至关重要。为了优化搅拌方案，我们应用贝叶斯优化确定了一个时间依赖的搅拌时间表，该时间表从高速重悬阶段开始，随后转为低速持续悬浮阶段，以最小化流体动力学应力。优化后的方案显示出更高的漂浮率和更低的滑移速度，表明细胞受到的机械应力降低。这些发现为可放大生物反应器操作提供了工程见解，有助于设计稳健的iPS细胞制造系统。

亮点
- CFD-DPM模拟预测了搅拌罐中iPS球体的运动。
- 贝叶斯优化确定了两步搅拌策略。
- 初始高搅拌促进了颗粒快速重悬。
- 后续低搅拌以较低的下向流维持悬浮。
- 颗粒雷诺数与漂浮率相关。

## Abstract
The suspension culture of pluripotent stem (PS) cells in stirred bioreactors poses a delicate balance between maintaining homogeneous cell dispersion and avoiding excessive shear stress that can compromise cell viability and pluripotency. In this study, we used computational fluid dynamics (CFD) coupled with a discrete particle method (DPM) to simulate iPS cell behavior in a 5 mL delta-impeller stirred tank. Our analysis revealed that upward flow at the tank bottom and downward flow at the top are critical for maintaining a stable suspension. To optimize the stirring protocol, we applied Bayesian optimization to identify a time-dependent stirring schedule that begins with a high-speed phase for resuspension, followed by a low-speed phase for sustained suspension with minimal hydrodynamic stress. The optimized schedule demonstrated improved floating rate and reduced slip velocity, indicating lower mechanical stress on cells. These findings provide engineering insights into scalable bioreactor operation, contributing to the design of robust iPS cell manufacturing systems.

HighlightsO_LICFD-DPM simulations predicted iPS spheroid motion in a stirred tank.
C_LIO_LIBayesian optimization identified a two-step agitation strategy.
C_LIO_LIHigh initial agitation promoted rapid particle resuspension.
C_LIO_LILow subsequent agitation maintained suspension with lower downflow.
C_LIO_LIParticle Reynolds number correlated with the floating rate.
C_LI