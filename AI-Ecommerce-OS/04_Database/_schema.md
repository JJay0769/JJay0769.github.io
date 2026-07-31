# 04_Database 字段定义（Schema）

> 所有 CSV 的字段权威定义。变更须同步本文件与 CHANGELOG。

## demand.csv（需求库）
| 字段 | 说明 | 示例 |
| ---- | ---- | ---- |
| demand_id | 需求编号 | demand-001 |
| short_name | 简称 | pet-hair |
| persona | 人群 | 养猫家庭 |
| scenario | 场景 | 沙发除毛 |
| source | 来源 | amazon_review |
| source_url | 来源链接 | https://... |
| evidence | 原文片段 | "粘不干净" |
| frequency | 出现频次 | 23 |
| severity | 严重度1-5 | 4 |
| current_solution | 当前解决方式 | 滚筒 |
| pain_point | 不满点 | 耗材贵 |
| desired_outcome | 期望结果 | 一次净 |
| keywords | 关联关键词 | cat hair\|sofa |
| product_direction | 关联产品方向 | 静电除毛器 |
| status | 状态 | 待验证/已验证/已转化/已放弃 |
| created_at | 创建日期 | 2026-07-31 |

## products.csv（产品库）
| 字段 | 说明 |
| ---- | ---- |
| product_id | product-001 |
| name | 产品名称 |
| category | 品类 |
| demand_id | 关联需求 |
| persona | 目标人群 |
| usp | 核心卖点 |
| differentiation | 差异化点 |
| cost_usd | 预估成本价 |
| price_usd | 建议零售价 |
| margin_pct | 预估毛利率% |
| fulfillment | 直邮/海外仓/FBA |
| weight_g | 重量 |
| compliance_risk | 合规风险 |
| seasonality | 季节性 |
| competition_level | 竞争强度1-5 |
| status | 候选/测试中/已上架/已下架 |
| created_at | 创建日期 |

## suppliers.csv（供应商库）
| 字段 | 说明 |
| ---- | ---- |
| supplier_id | supplier-001 |
| product_id | 关联产品 |
| name | 供应商名称 |
| platform | 1688/Alibaba/工厂 |
| moq | 起订量 |
| unit_price_usd | 单价 |
| sample_fee_usd | 打样费 |
| lead_time_days | 交期 |
| rating | 评分 |
| compliance | 合规资质 |
| return_policy | 退换货 |
| status | 候选/已合作/已淘汰 |

## competitors.csv（竞品库）
| 字段 | 说明 |
| ---- | ---- |
| competitor_id | competitor-001 |
| product_id | 关联产品 |
| store_name | 店铺名称 |
| platform | 平台 |
| category | 品类 |
| price_band | 价格带 |
| traffic_source | 流量来源 |
| monthly_visitors | 月访客(估) |
| content_intensity | 内容强度1-5 |
| fulfillment | 履约 |
| review_keywords | 口碑关键词 |
| strength | 优势 |
| weakness | 弱点 |
| attack_angle | 可攻击点 |
| competition_level | 竞争强度1-5 |
| updated_at | 更新日期 |

## ideas.csv（机会清单）
| 字段 | 说明 |
| ---- | ---- |
| idea_id | idea-001 |
| source_trend | 来源趋势 |
| market | 目标市场 |
| tam | TAM |
| growth_rate | 增长率% |
| audience | 人群 |
| window | 窗口期 |
| confidence | 高/中/低 |
| priority | 1-5 |
| action | 建议下一步 |
| status | 待评估/已立项/已放弃 |
| created_at | 创建日期 |

## score.csv（产品评分）
| 字段 | 说明 |
| ---- | ---- |
| product_id | product-001 |
| market_demand | 市场需求 /25 |
| competition | 竞争(低分优) /20 |
| margin | 毛利 /20 |
| supply | 供应链 /15 |
| compliance | 合规(低风险优) /10 |
| seasonality | 季节平稳 /10 |
| total | 总分 /100 |
| ad_feedback | 投放反馈 /10（Marketing回流，可选） |
| decision | 立项/测试/放弃 |
| updated_at | 更新日期 |
