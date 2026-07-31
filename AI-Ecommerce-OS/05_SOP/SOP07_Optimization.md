# SOP07 — 优化

- 版本：v1
- 主导：Marketing_Agent
- 参与：Content_Agent、Product_Agent、CEO_Agent
- 触发：投放有数据后

## 目标
基于数据持续优化产品/内容/广告/供应链，提升 ROAS 与 LTV。

## 流程
1. Marketing_Agent 做归因分析 → `09_Analytics/Reports/`。
2. 识别优化项：关停/加预算/换素材/调受众/调价格/改页面。
3. 设计增长实验（AB），定义主指标与护栏指标。
4. Content_Agent 按数据迭代素材。
5. Product_Agent 按转化与退货反馈调整供应链/选品。
6. 投放反馈回流 `score.csv`（ad_feedback 维度）。
7. CEO_Agent 周复盘，沉淀 SOP/Prompt 更新。

## 产出
- `09_Analytics/Reports/*.md`
- 更新 `score.csv`、内容与页面资产

## 验收标准
- 优化项有数据支撑
- 实验有显著性判定
- 复盘报告归档 `01_Research/Reports/`
