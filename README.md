# agent-skills

建立自己的 Skills 工作流，将常用的 AI 协作方法沉淀为可复用的 `SKILL.md`，并在实际任务中持续迭代。

## 工作流

1. **选择**：根据任务挑选合适的 Skill，将对应的 `SKILL.md` 提供给 AI。
2. **执行**：遵循 Skill 的指导完成任务，并验证结果。
3. **沉淀**：将有效做法补充到已有 Skill，或整理为新的 Skill。

## 当前 Skills

- [karpathy-guidelines](karpathy-guidelines/SKILL.md)：AI 编程行为准则，强调先思考、保持简单、精准修改和结果验证。
- [pstack](pstack/README.md)：来自 Cursor 的工程工作流集合，涵盖代码理解、架构设计、并行评审、测试验证和交付。
  - [poteto-mode](pstack/skills/poteto-mode/SKILL.md)：主入口，根据任务选择工作流。
  - [poteto-help](pstack/skills/poteto-help/SKILL.md)：了解和选择适合的 Skill。
  - [setup-pstack](pstack/skills/setup-pstack/SKILL.md)：在 Cursor 中配置各角色使用的模型。
  - [来源及使用说明](pstack/UPSTREAM.md)：固定版本、许可证和环境依赖。

## 维护约定

- 每个 Skill 使用独立目录：`<skill-name>/SKILL.md`。
- 第三方 Skill 集合保留上游目录结构，例如 `pstack/skills/<skill-name>/SKILL.md`，以及配套依赖和许可证。
- 按实际需求收录，保留核心指南和必要来源，避免冗余内容。
