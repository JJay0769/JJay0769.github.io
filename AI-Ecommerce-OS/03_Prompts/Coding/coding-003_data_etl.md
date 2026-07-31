# 数据处理脚本

- id: coding-003
- version: v1
- owner_agent: CEO_Agent
- status: active
- updated: 2026-07-31
- inputs: source_data, target_schema, transformation
- outputs: 08_Automation/Workflows

## 目标
把外部原始数据清洗为 04_Database / 09_Analytics 所需结构。

## 上下文注入
- 源数据：{{source_data}}
- 目标 schema：{{target_schema}}
- 转换规则：{{transformation}}

## 指令
1. 产出清洗脚本（Python/JS），含字段映射与校验。
2. 处理缺失值、重复值、单位换算。
3. 输出前后做行数对账。
4. 脚本放 `08_Automation/Workflows/`，命名 `etl-NNN-简称.{py,js}`。

## 输出格式
- 脚本 + 说明 `etl-NNN-简称.md`
