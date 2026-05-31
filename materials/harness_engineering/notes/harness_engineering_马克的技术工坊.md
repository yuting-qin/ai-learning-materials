## Prompt Engineering

解决怎么问问题

调整大模型提示词

## Context Engineering

解决怎么给信息

Context 包括

- prompt
- 对话历史
- 工具列表
- 技能列表
- ...

Context Engineer 方法

- 上下文压缩
- 动态检索外部资料
- 渐进式披露
- ...

## Harness Engineering

解决怎么搭建系统

构建与设计harness的技术
Harness = Agent - Model

### Open AI practice

[Harness engineering: leveraging Codex in an agent-first world](https://openai.com/index/harness-engineering)

1. 上下文管理

- Small agent.md
- structured docs
- Docs, decisions, knowledge lives with code

2. 验证与反馈

- 可观测
- Strict layers

3. 技术债清理

- 定期扫描代码库，修正错误代码
- 定期扫描更新修正错误或者过期文档

### Anthropic practice

[Effective harnesses for long-running agents](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents)
[Harness design for long-running application development](https://www.anthropic.com/engineering/harness-design-long-running-apps)

1. 任务规划
   任务： clone claude.ai
   问题： 需求工作量太大，Agent急于求成，无法保证效果
   解法： initializer，拆解用户需求，编写启动脚本，添加进度文件...
   演进：planner，拆解用户需求

2. 质量评估
   生成代码 -> 质量评估 -> 问题列表 循环

   独立的评估Agent做质量评估

Full Harness

- Planner
- Generator
- Evaluator

## Reference

[Harness engineering: leveraging Codex in an agent-first world](https://openai.com/index/harness-engineering)
