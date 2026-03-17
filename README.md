# ☢️ Vibe Audit Engine: Automated Smart Contract Sandbox & Self-Healing Matrix

[![Status](https://img.shields.io/badge/Status-Private_Core_V1.0-blue.svg)]()
[![Audits](https://img.shields.io/badge/Bombardment_Tests-100%2B_Top_Protocols-red.svg)]()
[![PoC](https://img.shields.io/badge/PoC_Ground_Truth-20%2B-success.svg)]()

> "The ultimate infrastructure for Web3 security researchers."

Vibe Audit Engine 并非另一个常规的静态扫描工具。这是一个专为应对极度碎片化的链上代码、复杂的代理模式（EIP-1967/Diamond）以及 Monorepo 依赖断层而生的**自动化靶场与环境自愈系统**。

本仓库 (Showcase) 展示了 Vibe Engine 在真实世界协议中的实战切片与 PoC Ground Truth。核心引擎目前处于 Private 状态。

## 核心技术引擎 (Internal Features)

* **Deep Ingestion (多源递归摄取)**: 无视嵌套代理与复杂架构，一键穿透 EIP-1967/钻石代理，将链上碎片化源码逆向重构为标准的 Foundry 隔离沙盒 (Sandboxed Environment)。
* **$O(k)$ Dependency Self-Healing**: 基于拓扑排序与后缀匹配的批量自愈算法。针对庞大 Monorepo 编译失败、依赖缺失等痛点，实现秒级环境修复。
* **Semantic Shield (语义护盾)**: 审计级代码防篡改机制。在修复破损依赖时，确保协议核心业务逻辑的绝对完整性，仅对第三方 Lib/Interface 执行精准补丁。

## 实战火力展示 (PoC Ground Truth)

Vibe 引擎已完成对全球 100+ Top 协议（Aave, Uniswap 等）的自动化轰炸测试环境构建，并累计发掘/复现 20+ 处真实高危漏洞。

## 🚀 Phase 1: The 100-Protocol Sandbox Matrix (Current Milestone)

在复杂的 Web3 安全审计中，环境配置往往消耗了研究员大量的时间。Vibe Engine 的第一阶段目标，是彻底消除“本地编译失败”与“依赖断层”的痛点。

目前，Vibe 引擎已成功对全球 100+ 个顶级协议（涵盖复杂的 Monorepo 与 EIP-1967/钻石代理模式）进行了自动化摄取与 $O(k)$ 依赖自愈，并重构为可直接执行的独立沙盒。

📂 **[探索自动化靶场矩阵](./ingested-sandboxes)**

*在 `ingested-sandboxes` 目录中，你可以看到由 Vibe 引擎全自动生成的 Foundry 结构。每个靶场均已剥离冗余依赖，保留了最纯净的 `src` 与 `test` 骨架，完美支持后续的 Fuzzing 或静态分析接入。*

## ⏳ Phase 2: PoC Ground Truth (Upcoming)

基于上述 100+ 个高度可用、语义完整的沙盒环境，Vibe 引擎的自动化漏洞挖掘模块正在持续运转。首批 20+ 个真实漏洞的 PoC (Proof of Concept) 将在脱敏后陆续开源。

*(关注 🐦 [Twitter/X: @j427467] 获取最新的漏洞拆解与 OOB Bypass 技术分享)*
