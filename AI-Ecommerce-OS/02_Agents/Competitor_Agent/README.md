# Competitor_Agent — 竞争分析 Agent

负责竞品监控、单店分析与差异化矩阵，验证所选品类的竞争强度与差异化空间。

## 职责

- 竞品店铺发现与监控
- 单店深度分析（流量/价格/内容/口碑/履约）
- 多店差异化矩阵，输出可攻击缝隙

## 输入 / 输出

- 输入：Product_Agent 候选产品、CEO_Agent 指定竞品范围
- 输出：`01_Research/Competitor/`、`04_Database/competitors.csv`

## 使用

业务 Prompt 模板见 `03_Prompts/Research/`。
