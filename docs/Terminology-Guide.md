# 术语库规范

`terminology/terms.yaml` 是项目的唯一术语源。文档、Skill、提示词和测试样例都引用它，不各自维护副本。

## 字段

- `zh`：批准的简体中文译名
- `en` / `de`：英文、德文原词；未知时使用 `null`
- `category`：稳定的学科分类
- `definition_zh`：中性、简短的工作定义
- `first_use`：首次纳入本项目的来源，不等同于术语首创来源
- `notes`：语义边界、禁用译法或使用提示
- `sources`：可核验的书目或公开链接
- `status`：`approved`、`provisional` 或 `deprecated`

## 键名规则

使用小写英文 `snake_case`。一个概念只有一个主条目；同义词写入 `aliases`，不要复制条目。

## 审核标准

优先参考权威教材、同行评审文献和学科惯例。出现多个合理译法时，记录语境差异，不用简单投票代替论证。
