# AGENTS.md

本仓库是一套**管理决策辅助知识库**，把成熟的组织行为学理论整理成「遇到问题 → 快速定位 → 匹配 1–2 个框架 → 3 步内可落地的行动」的工作流。

> 本文件供 [OpenAI Codex](https://developers.openai.com/codex)、Cursor 及其他读取 `AGENTS.md` 的 agent 使用。
> Claude 系（Claude Code / Claude.ai / Agent SDK）会自动识别 `SKILL.md`，无需本文件。

## 给 agent 的指令

当用户提出**管理类问题**（带团队、激励、授权、绩效、难管员工、向上管理、跨部门、冲突、变革、招聘、目标设定、领导风格等），请：

1. **先读 [`SKILL.md`](./SKILL.md)** —— 这是完整的使用指南、诊断路由和全部 9 个领域的框架速查。
2. **按 SKILL.md 的「诊断路由」定位问题类型**（个人 / 团队 / 组织 / 把事做成 / 我自己），不要一上来就堆框架。
3. **匹配 1–2 个最相关的框架**，需要细节时再读 [`references/`](./references/) 下对应的资料。
4. **输出结构**：问题诊断 → 推荐理论（标注来源）→ 3 步内可操作的行动建议 → 每个建议附「怎么判断奏效了」的可观察信号 + 复查时间点。

## 内容索引

- `SKILL.md` —— 主入口：诊断路由 + 9 个领域的框架速查
- `references/worked-examples.md` —— 「问题 → 诊断 → 行动」黄金范例（输出标杆）
- `references/unit1-details.md`、`unit2-situational.md`、`unit3-details.md` —— 按需加载的细分资料
- `docs/index.html` —— 配套学习手册网页（给人看，非 agent 运行所需）

## 注意

- 这是**知识/内容库**，不是可执行代码，没有构建、测试或运行步骤。
- 引用理论时遵循 SKILL.md 的「理论引用规范」：成熟理论标作者+年份，实践框架标来源。
