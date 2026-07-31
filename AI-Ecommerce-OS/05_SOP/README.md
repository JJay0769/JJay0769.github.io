# 05_SOP — 标准操作流程

> 跨 Agent 协作的标准流程，确保产出一致、可复用、可审计。
> 每个 SOP 定义：触发条件、参与 Agent、步骤、产出、验收标准。

## SOP 索引

| 编号   | 名称           | 触发               | 主导 Agent            |
| ------ | -------------- | ------------------ | --------------------- |
| SOP01  | 市场研究       | 周期/任务          | Trend_Agent           |
| SOP02  | 选品           | 机会立项后         | Product_Agent         |
| SOP03  | 供应商         | 候选 SKU 确定      | Product_Agent         |
| SOP04  | 内容生产       | 选品立项后         | Content_Agent         |
| SOP05  | 上线           | 内容与站点就绪     | CEO_Agent             |
| SOP06  | 投放           | 上线后             | Marketing_Agent       |
| SOP07  | 优化           | 投放有数据后       | Marketing_Agent       |

## 通用约定

- 每个 SOP 产出物归位到对应模块目录
- 数据落库遵循 `03_Prompts/System/system-002`
- 关键节点由 CEO_Agent 验收
- 任何偏差记录在 `CHANGELOG.md`
