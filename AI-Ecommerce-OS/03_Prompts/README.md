# 03_Prompts — Prompt 管理系统

> 所有业务 Prompt 集中管理、版本化、可复用。
> Agent 的系统级人设放在 `02_Agents/<Agent>/prompt.md`，业务场景 Prompt 放在这里。

---

## 分类

| 目录          | 用途                                   | 主要使用 Agent                |
| ------------- | -------------------------------------- | ----------------------------- |
| `System/`     | 系统级 Prompt（通用规则、输出规范）    | 全部                          |
| `Research/`   | 研究类（趋势/需求/产品/竞品/供应链）   | Trend / Demand / Product / Competitor |
| `Marketing/`  | 投放/数据/增长                          | Marketing                     |
| `Content/`    | 内容生产（Hook/脚本/文案/UGC）         | Content                       |
| `Coding/`     | 代码/脚本/API/工作流开发               | CEO / 自动化开发              |
| `Workflow/`   | 跨 Agent 编排与调度                    | CEO                           |

---

## Prompt 规范（必须遵守）

每个 Prompt 文件采用统一结构：

```markdown
# <Prompt 名称>

- id: <分类-编号>            例：research-001
- version: vX                例：v1
- owner_agent: <Agent>       例：Trend_Agent
- inputs: <所需输入字段>
- outputs: <产出目标>
- status: draft | active | deprecated

## 目标
...

## 上下文注入
{{变量名}}     # 运行时由编排器替换

## 指令
...

## 输出格式
...
```

---

## 版本与状态规则

- 新增 Prompt：`status: draft`
- 通过验收：`status: active`
- 不再使用：`status: deprecated`（保留不删除，便于回溯）
- 任何修改递增 `version`，并在文件顶部记录变更日期

## 索引

各分类 README 维护本类 Prompt 清单（id / 名称 / 状态 / 版本）。
