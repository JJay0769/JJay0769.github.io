# SOP03 — 供应商

- 版本：v1
- 主导：Product_Agent
- 参与：CEO_Agent
- 触发：候选 SKU 确定

## 目标
完成供应链研判，确定可合作供应商与履约方式。

## 流程
1. Product_Agent 寻找 ≥3 家供应商，比价（MOQ/单价/打样/交期）。
2. 评估履约方式（直邮/海外仓/FBA）匹配目标时效。
3. 合规初筛：认证、知识产权、平台政策、关税。
4. 稳定性评估：产能、备货、退换货。
5. 写入 `suppliers.csv`，产品卡更新供应链结论。
6. CEO_Agent 复核，确定合作供应商并打样。

## 产出
- `04_Database/suppliers.csv`
- `01_Research/Product_Library/product-NNN-*.md`（供应链段）

## 验收标准
- 供应商 ≥3 家比价记录
- 履约时效达标
- 合规风险标注
