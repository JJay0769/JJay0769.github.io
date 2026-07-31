# Cron — 定时任务

存放定时任务清单与配置。

## 任务清单（cron.md）

| 任务 | Cron | 用途 | 触发对象 | 状态 |
| ---- | ---- | ---- | -------- | ---- |
| 晨会派发 | 0 7 * * * | 每日派发 | CEO_Agent | draft |
| 趋势扫描 | 0 9 * * 1 | 每周趋势 | Trend_Agent | draft |
| 竞品更新 | 0 9 * * 1 | 双周竞品 | Competitor_Agent | draft |
| 数据简报 | 0 8 * * * | 每日数据 | Marketing_Agent | draft |
| 周复盘 | 0 18 * * 5 | 每周复盘 | CEO_Agent | draft |

> 时区：Asia/Shanghai。状态 draft → active 需 dry-run 通过。
