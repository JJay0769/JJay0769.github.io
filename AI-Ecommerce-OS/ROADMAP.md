# ROADMAP — 30 天计划

> 目标：30 天内跑通「市场研究 → 选品 → 内容 → 上线 → 投放 → 优化」最小闭环。
> 每个阶段产出明确交付物，写入对应目录并在 `CHANGELOG.md` 记录。

---

## 阶段总览

| 阶段 | 天数    | 主题           | 负责 Agent                 | 关键交付                       |
| ---- | ------- | -------------- | -------------------------- | ------------------------------ |
| P0   | Day 1-3 | 立项与基线     | CEO_Agent                  | 项目骨架、数据基线、SOP 评审   |
| P1   | Day 4-9 | 市场与需求     | Trend_Agent, Demand_Agent  | 趋势报告、需求库、机会清单     |
| P2   | Day 10-15 | 选品与供应链 | Product_Agent, Competitor_Agent | 产品库、竞品矩阵、供应商短名单 |
| P3   | Day 16-21 | 内容与站点  | Content_Agent, Marketing_Agent | 内容包、落地页、SEO 基线       |
| P4   | Day 22-26 | 上线与投放  | Marketing_Agent, CEO_Agent | 上线、首批广告、KPI 看板       |
| P5   | Day 27-30 | 数据与优化  | 全体 Agent                 | 归因分析、优化清单、复盘报告   |

---

## P0 — 立项与基线（Day 1-3）

- [ ] 评审目录结构与 SOP
- [ ] 初始化 `04_Database/` 基线数据
- [ ] 配置 7 个 Agent 的 `agent.yaml`
- [ ] 建立每日站会与周复盘节奏

## P1 — 市场与需求（Day 4-9）

- [ ] Trend_Agent 产出 3 份趋势报告 → `01_Research/Trends/`
- [ ] Demand_Agent 建立 50 条需求 → `04_Database/demand.csv`
- [ ] 输出机会清单 → `01_Research/Reports/`

## P2 — 选品与供应链（Day 10-15）

- [ ] Product_Agent 产出 30 个候选产品 → `04_Database/products.csv`
- [ ] Competitor_Agent 完成竞品矩阵 → `01_Research/Competitor/`
- [ ] 完成供应商短名单 → `04_Database/suppliers.csv`
- [ ] 选定 1-3 个首测 SKU

## P3 — 内容与站点（Day 16-21）

- [ ] Content_Agent 产出内容包（图/视频/脚本/Hook/CTA）
- [ ] 完成 1 个落地页 → `07_Website/LandingPage/`
- [ ] SEO 基线文档 → `07_Website/SEO/`

## P4 — 上线与投放（Day 22-26）

- [ ] Shopify/独立站上线
- [ ] 首批广告投放（Meta/TikTok/Google）
- [ ] KPI 看板上线 → `09_Analytics/Dashboard/`

## P5 — 数据与优化（Day 27-30）

- [ ] 归因分析报告 → `09_Analytics/Reports/`
- [ ] 优化清单（产品/内容/广告/供应链）
- [ ] 30 天复盘报告 → `01_Research/Reports/`
- [ ] 更新 `ROADMAP` 进入下一周期

---

## 验收标准

- 每个阶段交付物齐全且归位
- `TODO.md` 实时反映当前任务状态
- `CHANGELOG.md` 每阶段至少 1 条记录
- 数据库 CSV 字段完整、无空缺关键字段
