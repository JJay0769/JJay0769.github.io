# 04_Database — 结构化数据库

> 跨 Agent 共享的结构化数据，统一以 CSV 存储，便于导入工具与版本管理。
> 所有 Agent 的结论性数据必须落库（见 `03_Prompts/System/system-002`）。

## 数据表

| 文件             | 用途             | 主键           | 维护 Agent                          |
| ---------------- | ---------------- | -------------- | ----------------------------------- |
| `demand.csv`     | 用户需求库       | demand_id      | Demand_Agent                        |
| `products.csv`   | 候选产品库       | product_id     | Product_Agent                       |
| `suppliers.csv`  | 供应商库         | supplier_id    | Product_Agent                       |
| `competitors.csv`| 竞品库           | competitor_id  | Competitor_Agent                    |
| `ideas.csv`      | 机会清单         | idea_id        | Trend_Agent（入）/ CEO_Agent（复核）|
| `score.csv`      | 产品多维评分     | product_id     | Product_Agent / Marketing_Agent     |

## 规则

- 每张表第一行为表头，字段不得省略。
- 写入前比对去重，新增 `append`，更新 `upsert`。
- 布尔/状态用规范枚举值，不自由发挥。
- 商业敏感数据建议加密或加入 `.gitignore`。
- 字段定义变更须同步本 README 与 `CHANGELOG.md`。

## 字段速览

详见各 CSV 文件首行表头与 `04_Database/_schema.md`。
