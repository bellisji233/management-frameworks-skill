# 管理框架系统 · Management Frameworks Skill

一个面向**一线管理者**的管理决策辅助 skill，把成熟的组织行为学理论整理成「遇到问题 → 快速定位 → 匹配 1–2 个框架 → 3 步内可落地的行动」的工具。**原生支持 [Claude Code](https://claude.com/claude-code)，并通过 `AGENTS.md` 兼容 OpenAI Codex、Cursor 等多 agent 平台。** 配套一份可离线浏览的学习手册网页。

> ⚠️ 本项目为**学习整理**用途。所有理论版权归原作者所有；框架解读、案例与排版为教学目的的二次创作。

## 涵盖的 9 个领域

| 领域 | 核心框架 |
|------|---------|
| 1. 管理者效能 | Drucker 管理者 5 任务、麦肯锡 7S、高潜识别 |
| 2. 授权与辅导 | 情境领导力（Hersey & Blanchard）、GROW 教练模型 |
| 3. 激励与团队建设 | Maslow、Herzberg、Skinner、Adams、Vroom、盖洛普 Q12、STAR |
| 4. 绩效与发展 | ABC 员工分层、留才、难管员工对话 |
| 5. 组织沟通与向上管理 | 信息不对称、利益相关者对齐、约束转译、跨部门影响力 |
| 6. 团队动力学 | 塔克曼团队发展 4 阶段、心理安全感（Edmondson）、团队五大障碍（Lencioni） |
| 7. 目标、决策与执行 | OKR、RACI / RAPID、艾森豪威尔矩阵 |
| 8. 冲突、变革与选才 | 托马斯-基尔曼冲突模式（TKI）、科特 8 步 + ADKAR、结构化招聘 + 30-60-90 |
| 9. 领导力进阶 | 戈尔曼 6 种领导风格、驱动力 3.0（Pink） |

> 配套学习手册（`docs/index.html`，[在线查看](https://bellisji233.github.io/management-frameworks/)）完整覆盖以上 9 个领域，并附 20 道情境自测题。

## 安装（作为 Claude Code skill 使用）

把本仓库克隆或复制到你的 Claude Code skills 目录，命名为 `management-frameworks`：

```bash
git clone https://github.com/bellisji233/management-frameworks ~/.claude/skills/management-frameworks
```

随后在 Claude Code 中：

- 直接输入 `/management-frameworks` 触发，或
- 描述你的管理问题（如「我手下一个老员工躺平了怎么办」），skill 会按描述自动触发。

> `docs/`、`README.md`、`LICENSE` 一并复制进去不影响 skill 运行。

## 多 Agent 平台适配

本 skill 的内容是纯 Markdown，完全可移植。不同平台的接入方式如下：

| 平台 | 自动触发 | 接入方式 |
|------|:--------:|---------|
| **Claude Code** | ✅ 原生 | 放进 `~/.claude/skills/`，`/management-frameworks` 或按描述自动触发 |
| **Claude.ai / Agent SDK / API** | ✅ 原生 | 同样识别 `SKILL.md`（Agent Skills 标准） |
| **OpenAI Codex** | ✅ 经 `AGENTS.md` | 读取仓库根目录 [`AGENTS.md`](./AGENTS.md)，被引导去用 `SKILL.md` + `references/` |
| **Cursor** | ⚙️ 需配置 | 把 `SKILL.md` 内容放进 `.cursor/rules/`，或在对话中 `@` 引用 |
| **其他 agent / 纯人类** | ➖ 手动 | 直接阅读 `SKILL.md`，或把内容喂进对方上下文当知识库 |

> 说明：`SKILL.md` 的「自动按描述触发」是 Claude 生态（Agent Skills 标准）专属能力；[`AGENTS.md`](./AGENTS.md) 让 Codex 等读取该约定的 agent 也能用上同一套诊断流程与框架。

## 学习手册网页

`docs/index.html` 是一份单文件、可离线浏览的管理理论学习手册，包含全部框架、职场案例、反模式提醒与「场景反查索引」。

- **在线查看**：https://bellisji233.github.io/management-frameworks/
- **本地查看**：用浏览器打开 `docs/index.html`

## 目录结构

```
.
├── SKILL.md                    # skill 主入口（使用指南 + 全部框架速查）
├── AGENTS.md                   # 供 Codex 等非 Claude agent 使用的入口
├── references/                 # 按需加载的详细资料（每单元一份，含操作步骤、职场案例、反模式）
│   ├── unit1-details.md         # 管理者效能（14 行为 / 7S / 高潜 10 维度）
│   ├── unit2-situational.md     # 情境领导力 9 种情境的详细操作
│   ├── unit3-details.md         # 激励五理论 / Q12 全 12 问 / 团队建设 10 法
│   ├── unit4-details.md         # 绩效与发展（ABC 话术 / 难管员工处理）
│   ├── unit5-details.md         # 组织沟通与向上管理（五框架）
│   ├── unit6-details.md         # 团队动力学（塔克曼 / 心理安全感 / 五大障碍）
│   ├── unit7-details.md         # 目标决策与执行（OKR / RACI-RAPID / 艾森豪威尔）
│   ├── unit8-details.md         # 冲突变革选才（TKI / 科特+ADKAR / 结构化招聘）
│   ├── unit9-details.md         # 领导力进阶（戈尔曼 6 风格 / 驱动力 3.0）
│   └── worked-examples.md      # 「问题 → 诊断 → 行动」黄金范例
└── docs/
    └── index.html              # 配套学习手册网页（GitHub Pages 来源）
```

## 理论引用规范

- 成熟学术理论：注明作者 + 年份
- 实践框架：注明来源机构或书籍
- 记忆口诀 / 整合工具：标注「实践整合」

## License

[MIT](./LICENSE)
