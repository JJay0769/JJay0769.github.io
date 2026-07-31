# Product_Agent — 产品筛选与供应链 Agent

负责从需求反推候选产品，并完成供应链研判（货源/成本/履约/合规）。

## 职责

- 需求 → 产品方向 → 候选 SKU
- 供应链分析：货源、成本、履约、合规、季节性
- 维护产品库与供应商库
- 给出产品评分（写入 `04_Database/score.csv`）

## 输入 / 输出

- 输入：Demand_Agent 的需求库、CEO_Agent 指定品类
- 输出：`01_Research/Product_Library/`、`04_Database/products.csv`、`04_Database/suppliers.csv`、`04_Database/score.csv`

## 使用

业务 Prompt 模板见 `03_Prompts/Research/`。供应链流程参考 `05_SOP/SOP03_Supplier.md`。
