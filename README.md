# gpt55-prompt-orchestration

这是一个面向 Codex / GPT-5.x 提示词编排的技能仓库。

当前提供的核心技能是：

- `gpt55-prompt-orchestration`：用于编写或改写 GPT-5.5 风格提示词、Codex 执行提示词、主代理编排提示词，以及 GPT-5.x 子代理交接提示词。

## 它能帮你做什么

### `gpt55-prompt-orchestration`

这个技能适合你在下面几类场景里使用：

- 你要把自然语言需求改写成更稳的 Codex 执行提示词。
- 你要为 GPT-5.x 子代理编写可执行的交接提示词。
- 你要把已有实施计划、Task 拆分或规格文档，整理成结果优先的提示词合同。
- 你要约束主代理只做顾问、调度、验收，不让主代理越界自己下场实现。
- 你要统一子代理的模型选择、推理强度、交付格式和轻量日志规则。

## 你会得到什么

使用这个技能后，产出通常会是下面这些内容之一：

- 中文、结果优先的 Codex 执行提示词。
- 带明确身份背景的 GPT-5.x 子代理交接提示词。
- 清晰的完成标准、约束、检查方式、交付格式和停止规则。
- 按既有 Task 边界整理好的执行口径，而不是另一套被重新发明的任务体系。
- 大任务稳定开发

## 什么时候不要用

下面这些场景不属于它的范围：

- 你只是要做普通代码实现，而不是提示词编排。
- 不是大任务建议不要用，因为开发时长非常慢

## 前置技能

这个技能在某些任务里会引用到下面两个前置技能。
具体安装或接入方式请直接看各自原仓库文档。

### 1. `web-design-engineer`

适用场景：

- 当子代理涉及 UI 实现、前端视觉调整、截图后修正、设计系统对齐或视觉审查时使用。

GitHub 原技能地址：

- 仓库首页：[ConardLi/garden-skills](https://github.com/ConardLi/garden-skills)
- 技能目录：[skills/web-design-engineer](https://github.com/ConardLi/garden-skills/tree/main/skills/web-design-engineer)

### 2. `karpathy-guidelines`

适用场景：

- 当子代理需要写代码、改代码、重构或修复问题时使用，用来约束实现范围和可验证交付。

GitHub 原技能地址：

- 仓库首页：[forrestchang/andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills)
- 技能目录：[skills/karpathy-guidelines](https://github.com/forrestchang/andrej-karpathy-skills/tree/main/skills/karpathy-guidelines)

## 使用特点

- 默认使用中文来生成和整理提示词。
- 优先以当前用户消息、当前点名计划、规格和代码为真源。
- 不会把旧记忆、旧模板或过期路线放在当前真源之前。

## 想看具体规则

- 技能主规则：[`gpt55-prompt-orchestration/SKILL.md`](./gpt55-prompt-orchestration/SKILL.md)
- 默认展示配置：[`gpt55-prompt-orchestration/agents/openai.yaml`](./gpt55-prompt-orchestration/agents/openai.yaml)
- 子代理日志规范：[`gpt55-prompt-orchestration/references/subagent-log.md`](./gpt55-prompt-orchestration/references/subagent-log.md)
