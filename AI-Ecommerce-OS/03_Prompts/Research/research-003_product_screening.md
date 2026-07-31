# 选品研判

- id: research-003
- version: v1
- owner_agent: Product_Agent
- status: active
- updated: 2026-07-31
- inputs: demand_id[], category, budget
- outputs: 01_Research/Product_Library, 04_Database/products.csv, score.csv

## 目标
从需求反推候选 SKU，完成 6 维评分。

## 上下文注入
- 关联需求：{{demand_id}}
- 品类：{{category}}
- 预算上限：{{budget}}

## 指令
1. 反推产品方向，给出候选 SKU 列表。
2. 每个 SKU 关联 demand_id，明确 USP 与差异化点。
3. 测算成本/零售/毛利（≥3 家供应商比价）。
4. 评估履约方式、合规风险、季节性。
5. 按 6 维评分模型（见 agent.yaml）打分，写入 score.csv。
6. 按 `_template_product.md` 产出研究卡。

## 输出格式
- 文件：`product-NNN-简称.md`
- CSV：append products.csv / suppliers.csv；upsert score.csv
