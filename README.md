# Canine Academic Studio｜犬类学术工作室

一个面向犬行为学、动物行为学及相关生命科学文献的开源中文学术翻译工作流。

项目的核心不是堆叠提示词，而是逐步建立一套可追溯、可测试、可协作的中文动物行为学术语标准。当前版本为 **V0.1 MVP**：英文/德文到中文的学术翻译规范、术语库、单一翻译 Skill、回归测试样例和 Obsidian 模板。

## V0.1 能做什么

- 统一术语及首次出现形式，例如 `游戏鞠躬（Play Bow）`
- 指导 AI 按同一套规则翻译英文或德文学术文本
- 用标准样例检查 Skill 升级是否引发术语漂移
- 统一书籍、章节、图表、参考文献和译者注的 Obsidian 记录格式
- 为 V0.2 的图注与图片翻译预留清晰边界

## 快速开始

1. 阅读 [`docs/Workflow.md`](docs/Workflow.md)。
2. 将待翻译原文放入本地工作区（受版权保护的书籍原文不要提交到公共仓库）。
3. 让模型读取 [`skills/academic-translator/SKILL.md`](skills/academic-translator/SKILL.md)、`docs/` 下的规范和 [`terminology/terms.yaml`](terminology/terms.yaml)。
4. 按 [`templates/Obsidian-Book-Template.md`](templates/Obsidian-Book-Template.md) 保存译文。
5. 对照 `examples/` 中的标准答案做回归检查。

## 项目结构

```text
canine-academic-studio/
├── docs/                  # 翻译、文风、术语与工作流规范
├── skills/                # 单一职责的 AI Skill
├── prompts/               # 可复用的任务入口提示
├── terminology/           # 唯一术语源（YAML）
├── templates/             # Obsidian 等输出模板
├── examples/              # 可公开的短篇测试样例
└── output/                # 本地生成结果（默认不提交）
```

## 版本路线

- **V0.1**：项目骨架、规范、术语库、翻译 Skill、测试集与 Obsidian 模板
- **V0.2**：图片分类、图注翻译和人工复核流程
- **V0.3**：OCR 校正与导出
- **V1.0**：稳定的端到端学术翻译系统
- **V2.0**：知识图谱、跨书关联和 Obsidian 自动链接

## 版权与贡献

只提交有权公开的原文片段、译文和图片。书籍全文、扫描件和受版权保护的图像必须保留在本地。术语修改请附来源、语境和受影响测试样例，详见 [`CONTRIBUTING.md`](CONTRIBUTING.md)。

本项目采用 [MIT License](LICENSE)。
