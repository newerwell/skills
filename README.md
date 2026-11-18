# Agent Skills

面向支持 Agent Skills 的编码助手（Claude Code、Codex、Cursor 等）的可复用技能集合。

## 包含的 Skills

| Skill | 说明 | 文档 | ZIP 下载 |
| --- | --- | --- | --- |
| `software-engineering-workflow` | 软件工程工作流：按风险选择代码边界、验证方式与交付步骤，复现重复错误并从真实入口检查交付结果 | [SKILL.md](software-engineering-workflow/SKILL.md) | [software-engineering-workflow.zip](https://raw.githubusercontent.com/newerwell/skills/main/dist/software-engineering-workflow.zip) |
| `ai-code-review` | AI 代码独立审查：面向需求分支与合并后发布前复核，覆盖需求正确性、系统一致性、回归与并发、误报白名单及输出契约 | [SKILL.md](ai-code-review/SKILL.md) | [ai-code-review.zip](https://raw.githubusercontent.com/newerwell/skills/main/dist/ai-code-review.zip) |

## 从 GitHub 安装

在需要使用它的项目目录中运行（需要 Node.js 和 Git）。按提示选择你的 Agent。

```sh
# 安装全部或指定 Skill
npx skills add newerwell/skills --skill software-engineering-workflow
npx skills add newerwell/skills --skill ai-code-review
```

也可在命令末尾加 `-a claude-code`、`-a codex` 或 `-a cursor` 指定目标。默认安装到当前项目。[安装器文档](https://github.com/vercel-labs/skills/blob/main/docs/commands.md)

## 从 ZIP 导入

从上方表格下载对应的 `.zip` 文件。如果客户端提供 Skill ZIP 导入，直接选择该文件。手动安装时解压一次，把整个技能文件夹（例如 `software-engineering-workflow` 或 `ai-code-review`）复制到目标项目的技能目录，确保 `SKILL.md` 就在技能文件夹的第一层。

| 目标 | 复制后的入口 |
| --- | --- |
| Claude Code | `.claude/skills/<skill-name>/SKILL.md` |
| Codex、Cursor（通过 skills CLI） | `.agents/skills/<skill-name>/SKILL.md` |

打开目标项目的新会话后，即可按需调用对应 Skill（例如输入「用 `$ai-code-review` 审查当前变更」或「用 `software-engineering-workflow` 审查这次改动」）。使用其他客户端时，按其文档选择技能目录。[Agent 目录表](https://github.com/vercel-labs/skills/blob/main/docs/agents.md) · [Agent Skills 规范](https://agentskills.io/specification)
