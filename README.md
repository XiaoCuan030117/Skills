# Skills

面向 Codex 的个人技能集合，沉淀可复用的开发工作流与协作实践。

每个技能独立存放在 `skills/` 下，包含规则入口 `SKILL.md`、使用说明及必要的参考文件。按需安装具体技能即可。

## 技能目录

| 技能 | 用途 | 使用说明 |
| --- | --- | --- |
| **WQ-workflow** · `wq-workflow` | 从需求澄清、计划审查到分阶段实现、代码审查、修复及最终验收；控制范围，减少重复检查，保留清楚的交接记录。 | [README](skills/wq-workflow/README.md) · [技能规则](skills/wq-workflow/SKILL.md) |

## 安装

如果当前 Codex 环境提供技能安装器，可直接发送：

```text
使用 $skill-installer，从以下地址安装 wq-workflow：
https://github.com/XiaoCuan030117/Skills/tree/main/skills/wq-workflow
```

也可以下载仓库 ZIP，将 `skills/wq-workflow/` 整个文件夹复制到当前工具识别的技能目录。个人安装与项目安装的具体位置见 [WQ-workflow 安装说明](skills/wq-workflow/README.md#安装)。

不要把整个仓库当成一个技能安装。安装前检查是否已有同名技能，避免重复安装或覆盖自己的修改。

## 快速开始

```text
使用 $wq-workflow。我想开发一个新项目，
先帮我澄清需求并制定可分阶段验收的计划，暂不写业务代码。
```

已有计划时，可以直接指定当前环节：

```text
使用 $wq-workflow，按照 PLAN.md 完成第一阶段，
验证并汇报后停止，不提交、不推送、不创建 PR。
```

完整的计划审查、代码审查、修复、复审及收尾示例见 [使用说明](skills/wq-workflow/README.md#调用示例)。

## 仓库结构

```text
Skills/
├── README.md
└── skills/
    └── wq-workflow/
        ├── SKILL.md
        ├── README.md
        ├── agents/
        │   └── openai.yaml
        └── references/
            ├── planning.md
            ├── review.md
            └── delivery.md
```

## 使用与维护

- 技能提供工作指引，项目自身约定和用户当前要求仍需遵守。
- 小任务可以简化流程，不强制生成整套文档或重复执行所有检查。
- 安装技能不会自动创建多个 agent、提交代码或部署项目；具体操作遵循用户授权范围。
- 当前技能已完成静态结构检查，实际效果仍需通过项目使用验证，不承诺自动消除缺陷。
- 后续根据真实使用中的问题逐步调整；新技能使用独立目录，并在上方目录中登记。

Codex 的技能发现和调用方式参见 [官方技能文档](https://learn.chatgpt.com/docs/build-skills)。
