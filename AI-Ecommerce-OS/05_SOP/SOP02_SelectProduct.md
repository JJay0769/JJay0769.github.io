# SOP02 — 选品

- 版本：v1
- 主导：Product_Agent
- 参与：Competitor_Agent、CEO_Agent
- 触发：机会立项后

## 目标
从需求反推候选 SKU，完成多维评分，选定首测产品。

## 流程
1. Product_Agent 基于 demand.csv 反推产品方向。
2. 产出候选 SKU 研究卡 → `01_Research/Product_Library/`。
3. Competitor_Agent 对每个候选做竞品矩阵 → `01_Research/Competitor/`。
4. Product_Agent 6 维评分 → `score.csv`（含竞争维度反馈）。
5. CEO_Agent 复核，选定 1-3 个首测 SKU，状态置“测试中”。
6. 重大立项走人工确认。

## 产出
- `01_Research/Product_Library/*.md`
- `01_Research/Competitor/*.md`
- `04_Database/products.csv`、`competitors.csv`、`score.csv`

## 验收标准
- 每个 SKU ≥3 家供应商比价
- 合规风险已初筛
- 评分每维给理由
