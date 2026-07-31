# 通用输出规范

- id: system-001
- version: v1
- owner_agent: all
- status: active
- updated: 2026-07-31

## 目标
统一所有 Agent 的产出格式，保证可被下游解析与归档。

## 指令
1. 所有文件遵循 `01_Research/` 或对应模块的命名规范。
2. Markdown 顶部含元信息块（主题/版本/日期/Agent/来源）。
3. 结论性数据同步写入 `04_Database/` 对应 CSV。
4. 引用数据须标注来源链接与采集时间。
5. 不得输出未经验证的“事实”。

## 输出格式
见各模块模板（`_template_*.md`）。
