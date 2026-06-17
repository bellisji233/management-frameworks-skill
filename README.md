# 管理框架系统 · Management Frameworks Skill

一个面向**一线管理者**的 [Claude Code](https://claude.com/claude-code) skill，把成熟的组织行为学理论整理成「遇到问题 → 快速定位 → 匹配 1–2 个框架 → 3 步内可落地的行动」的决策辅助工具。配套一份可离线浏览的学习手册网页。

> ⚠️ 本项目为**学习整理**用途。所有理论版权归原作者所有；框架解读、案例与排版为教学目的的二次创作。

## 涵盖的 5 个领域

| 领域 | 核心框架 |
|------|---------|
| 管理者效能 | Drucker 管理者 5 任务、麦肯锡 7S、高潜识别 |
| 授权与辅导 | 情境领导力（Hersey & Blanchard）、GROW 教练模型 |
| 激励与团队建设 | Maslow、Herzberg、Skinner、Adams、Vroom、盖洛普 Q12、STAR |
| 绩效与发展 | ABC 员工分层、留才、难管员工对话 |
| 组织沟通与向上管理 | 信息不对称、利益相关者对齐、约束转译、跨部门影响力 |

## 安装（作为 Claude Code skill 使用）

把本仓库克隆或复制到你的 Claude Code skills 目录，命名为 `management-frameworks`：

```bash
git clone <this-repo-url> ~/.claude/skills/management-frameworks
```

随后在 Claude Code 中：

- 直接输入 `/management-frameworks` 触发，或
- 描述你的管理问题（如「我手下一个老员工躺平了怎么办」），skill 会按描述自动触发。

> `handbook/`、`README.md`、`LICENSE` 一并复制进去不影响 skill 运行。

## 学习手册网页

`handbook/index.html` 是一份单文件、可离线浏览的管理理论学习手册，包含全部框架、职场案例、反模式提醒与「场景反查索引」。

- **本地查看**：用浏览器打开 `handbook/index.html`
- **在线查看**：在仓库 Settings → Pages 中将来源设为 `main` 分支的 `/handbook` 目录（或 `/docs`），即可通过 GitHub Pages 访问。

## 目录结构

```
.
├── SKILL.md                    # skill 主入口（使用指南 + 全部框架速查）
├── references/                 # 按需加载的详细资料
│   ├── unit1-details.md
│   ├── unit2-situational.md
│   ├── unit3-details.md
│   └── worked-examples.md      # 「问题 → 诊断 → 行动」黄金范例
└── handbook/
    └── index.html              # 配套学习手册网页
```

## 理论引用规范

- 成熟学术理论：注明作者 + 年份
- 实践框架：注明来源机构或书籍
- 记忆口诀 / 整合工具：标注「实践整合」

## License

[MIT](./LICENSE)
