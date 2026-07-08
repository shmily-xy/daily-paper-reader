---
title: CFD-based Bayesian Optimization of Stirring Strategies in Stirred Tank Cultures of Pluripotent Stem Cell Spheroids
title_zh: 基于CFD的贝叶斯优化在多能干细胞球体搅拌罐培养中的搅拌策略
authors: "Horiguchi, I., Okada, K., Okano, Y."
date: 2026-07-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.735037v1.full.pdf"
tags: ["query:equipment"]
score: 7.0
evidence: CFD与贝叶斯优化搅拌策略可迁移至电池浆料混合设备
tldr: 干细胞悬浮培养需平衡分散与剪切应力。本研究用CFD-DPM模拟iPS细胞在搅拌罐中的行为，发现底部上升流和顶部下降流对稳定悬浮至关重要。使用贝叶斯优化设计了先高速后低速的搅拌协议，提升了悬浮率并降低了滑移速度，为大规模干细胞培养提供了工程优化方法。
source: biorxiv
selection_source: fresh_fetch
motivation: 干细胞悬浮培养中，搅拌需兼顾均匀分散与低剪切应力，现有方法难以兼顾。
method: CFD-DPM模拟后，使用贝叶斯优化寻找时间依赖的搅拌速度程序。
result: 优化协议实现高悬浮率与低滑移速度，机械应力显著降低。
conclusion: 贝叶斯优化可有效设计干细胞搅拌培养的时序协议，支持可放大生产。
---

## 摘要
在搅拌式生物反应器中悬浮培养多能干细胞需要在保持均匀细胞分散和避免过度剪切应力（可能损害细胞活力和多能性）之间取得精细平衡。本研究采用计算流体动力学与离散粒子方法相结合，模拟了5 mL三角叶轮搅拌罐中iPS细胞的行为。分析表明，罐底向上流和顶部向下流对于维持稳定悬浮至关重要。为了优化搅拌方案，我们应用贝叶斯优化来识别一个随时间变化的搅拌时间表，该时间表从高速重悬阶段开始，随后是低速持续悬浮阶段，以最小化流体动力应力。优化后的方案显示出更高的悬浮比和更低的滑移速度，表明细胞受到的机械应力降低。这些发现为可扩展的生物反应器操作提供了工程见解，有助于设计稳健的iPS细胞制造系统。

## Abstract
The suspension culture of pluripotent stem (PS) cells in stirred bioreactors poses a delicate balance between maintaining homogeneous cell dispersion and avoiding excessive shear stress that can compromise cell viability and pluripotency. In this study, we used computational fluid dynamics (CFD) coupled with a discrete particle method (DPM) to simulate iPS cell behavior in a 5 mL delta-impeller stirred tank. Our analysis revealed that upward flow at the tank bottom and downward flow at the top are critical for maintaining a stable suspension. To optimize the stirring protocol, we applied Bayesian optimization to identify a time-dependent stirring schedule that begins with a high-speed phase for resuspension, followed by a low-speed phase for sustained suspension with minimal hydrodynamic stress. The optimized schedule demonstrated improved suspension ratio and reduced slip velocity, indicating lower mechanical stress on cells. These findings provide engineering insights into scalable bioreactor operation, contributing to the design of robust iPS cell manufacturing systems.