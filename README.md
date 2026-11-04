# elon-musk-perspective · 马斯克 CEO · 决策与执行

> **English:** An agent skill that applies Musk-style first-principles thinking — question the requirement, rebuild from verified facts, and the five-step algorithm — to major trade-offs, unclear premises and cost/necessity calls. The AI decides and executes within the authority it already has, keeps the user in charge of direction, vetoes and exceptions, and proves results before claiming done. Simple tasks get only a light internal check. Chinese-language skill; adapted from [alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill) (MIT).

## 它做什么

- **重大取舍时先想清楚**：五项检查——你要什么结果、这件事是否必要、什么确实成立、最小充分方案是什么、怎样证明有效。
- **AI 先拍板、再执行**：在已有授权内自己做方案选择和技术取舍，不把能自己查明的事抛回给用户；付款、新增授权、重大不可逆操作等例外仍交用户决定。
- **五步算法只是检查顺序**：质疑需求 → 排除多余环节 → 简化 → 按需加速 → 按需自动化；不设删减比例，不要求每步确认。
- **不唱反调、不编数字**：成本未知就写未知；兴趣、审美、学习类任务不强行算收益；严格格式要求优先，不加“第一性原理分析”前缀。
- 简单任务只做内部轻量检查，直接交付。

触发场景：重大方案取舍、关键前提不明、成本与必要性判断，或你明确说“用马斯克视角”“问马斯克”。

## 安装

这是一个 Agent Skill（一份写给 AI 读的工作说明，入口是 `SKILL.md`），可用于 Claude Code、Codex 等支持 skills 目录的工具。不需要额外的 API key 或后台服务。

把整个仓库放进你的 skills 目录，目录名保持 `elon-musk-perspective`：

```bash
# Claude Code（个人级）
git clone https://github.com/Samuel-Shek/elon-musk-perspective.git ~/.claude/skills/elon-musk-perspective

# Codex
git clone https://github.com/Samuel-Shek/elon-musk-perspective.git ~/.codex/skills/elon-musk-perspective
```

其他工具放进各自的 skills 目录即可。装好后重开会话，遇到重大取舍或说“用马斯克视角看一下”即可触发。

## 目录

| 文件 | 用途 |
|---|---|
| `SKILL.md` | 主说明：职责边界、五项检查、行动与输出规则 |
| `references/methods.md` | 成本拆解、五步算法、小步验证、自建与外包 |
| `references/comparison.md` | 与公开方案的比较依据 |
| `references/*调研*.md`、`research.md` | 马斯克人物调研素材（来自上游，按原样收录，仅供核对来源） |
| `agents/openai.yaml` | Codex 等工具的显示名与默认提示 |

## 来源与致谢

- 改编自 [alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill) 的 `examples/elon-musk-perspective`（花叔，MIT）。4 份人物调研参考文件与原版逐字相同，`SKILL.md` 为重写版本。
- 方法参考：[danyuchn/first-principles-skill](https://github.com/danyuchn/first-principles-skill)、[swapnildahiphale/first-principles-thinking-skill](https://github.com/swapnildahiphale/first-principles-thinking-skill)、[wezendy/elon-musk-algorithm-skills](https://github.com/wezendy/elon-musk-algorithm-skills)（均为 MIT）。
- 五步工程算法出处见 [Everyday Astronaut 访谈](https://everydayastronaut.com/starbase-tour-and-interview-with-elon-musk/)。本项目与马斯克本人及其公司无关。

详见 [NOTICE](NOTICE)。

## 许可证

[MIT](LICENSE)，保留原作者花叔的版权声明。
