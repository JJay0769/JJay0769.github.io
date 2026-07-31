# 投放策略制定

- id: marketing-001
- version: v1
- owner_agent: Marketing_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, assets[], kpi_targets
- outputs: 09_Analytics/Ads, 04_Database/score.csv

## 目标
基于素材与 KPI 目标，产出可执行的投放策略。

## 上下文注入
- 产品：{{product_id}}
- 素材：{{assets}}
- KPI 目标：{{kpi_targets}}

## 指令
1. 选择渠道（Meta/TikTok/Google）并说明依据。
2. 给出受众、预算分配、出价方式、止损线。
3. 设计素材 AB 测试矩阵（变量：Hook/受众/落地页）。
4. 定义观测窗口与判定指标。
5. 产出策略文档 → `09_Analytics/Ads/`。

## 输出格式
- 文件：`YYYYMMDD_产品简称_ad-strategy_vX.md`
