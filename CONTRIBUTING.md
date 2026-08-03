# 贡献指南

## 基本原则

1. 不提交无公开授权的书籍全文、扫描件或图片。
2. 术语库是唯一标准来源；不要只在译文中私自改变术语。
3. 每次术语变更必须说明来源、语境、理由和影响范围。
4. 新规则应同时增加或更新一个 `examples/` 回归样例。
5. 保留原作者的不确定性，不擅自强化因果、价值判断或结论。

## 术语变更流程

- 在 `terminology/terms.yaml` 修改条目。
- 在 `notes` 写明语义边界；有依据时填写 `sources`。
- 搜索所有样例，确认首次出现形式和后续简称一致。
- 在拉取请求中列出旧译法、新译法及理由。

## 提交信息建议

```text
docs: clarify citation handling
term: add displacement_activity
test: add play-bow regression case
skill: tighten uncertainty preservation
```
