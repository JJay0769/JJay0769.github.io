# Trend_Agent — 趋势与市场研究 Agent

负责跨境电商的趋势扫描与市场研究，覆盖平台趋势、品类趋势、关键词与社媒热点。

## 职责

- 周期性扫描趋势信号（平台/社媒/搜索/达人）
- 产出趋势快报与市场综述报告
- 维护机会清单（写入 `04_Database/ideas.csv`）

## 输入 / 输出

- 输入：CEO_Agent 派发的扫描主题、关键词、时间窗口
- 输出：`01_Research/Trends/`、`01_Research/Market_Report/`、`04_Database/ideas.csv`

## 使用

1. 读取 `agent.yaml` 加载配置
2. 使用 `prompt.md` 作为系统 Prompt
3. 业务 Prompt 模板见 `03_Prompts/Research/`
4. 任务记录在 `tasks.md`
