# 软件工程工作流 Skill

面向支持 Agent Skills 的编码助手。可用于学习工程实践、审查改动、实现和修复功能。它指导 Agent 按风险选择验证方式，复现重复错误，并从真实入口检查交付结果。[查看 Skill](software-engineering-workflow/SKILL.md)

## 从 GitHub 安装

在需要使用它的项目目录中运行（需要 Node.js 和 Git）。按提示选择你的 Agent。

```sh
npx skills add newerwell/skills --skill software-engineering-workflow
```

也可在命令末尾加 `-a claude-code`、`-a codex` 或 `-a cursor` 指定目标。默认安装到当前项目。[安装器文档](https://github.com/vercel-labs/skills/blob/main/docs/commands.md)

## 从 ZIP 导入

[下载 software-engineering-workflow.zip](https://raw.githubusercontent.com/newerwell/skills/main/dist/software-engineering-workflow.zip)。如果客户端提供 Skill ZIP 导入，直接选择该文件。手动安装时解压一次，把整个 `software-engineering-workflow` 文件夹复制到目标项目的技能目录，确保 `SKILL.md` 就在技能文件夹的第一层。

| 目标 | 复制后的入口 |
| --- | --- |
| Claude Code | `.claude/skills/software-engineering-workflow/SKILL.md` |
| Codex、Cursor（通过 skills CLI） | `.agents/skills/software-engineering-workflow/SKILL.md` |

打开目标项目的新会话后，可以输入「用 software-engineering-workflow 审查这次改动，列出最可能影响用户的行为和复查方法」。使用其他客户端时，按其文档选择技能目录。[Agent 目录表](https://github.com/vercel-labs/skills/blob/main/docs/agents.md) · [Agent Skills 规范](https://agentskills.io/specification)
