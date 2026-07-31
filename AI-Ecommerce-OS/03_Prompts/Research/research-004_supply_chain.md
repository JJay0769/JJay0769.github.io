# 供应链分析

- id: research-004
- version: v1
- owner_agent: Product_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, target_market
- outputs: 04_Database/suppliers.csv, 01_Research/Product_Library

## 目标
对候选产品完成供应链研判：货源、成本、履约、合规、稳定性。

## 上下文注入
- 产品：{{product_id}}
- 目标市场：{{target_market}}

## 指令
1. 寻找 ≥3 家供应商，比价（MOQ/单价/打样费/交期）。
2. 评估履约方式：直邮 / 海外仓 / FBA，匹配目标时效。
3. 合规初筛：认证、知识产权、平台政策、关税。
4. 稳定性：产能、备货周期、退换货政策。
5. 结论写入 suppliers.csv，并在产品研究卡更新供应链结论。

## 输出格式
- CSV：append suppliers.csv
- 产品卡：更新 `product-NNN-简称.md` 的供应链段落
