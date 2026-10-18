# code-mentor · AI Coding Mentor

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-blue.svg)](SKILL.md)
[![Category](https://img.shields.io/badge/category-education-8a2be2.svg)](#)
[![Version](https://img.shields.io/badge/version-1.0.0-informational.svg)](#)
[![llms.txt](https://img.shields.io/badge/AI--friendly-llms.txt-101E2C.svg)](llms.txt)
[![中文](https://img.shields.io/badge/%E4%B8%AD%E6%96%87-README.md-blue.svg)](README.md)

> An all-around AI coding mentor using the Socratic method for interactive learning, code review, debugging guidance, algorithm drills, project coaching and design-pattern walkthroughs, supporting Python / JavaScript.

**Keywords**: 编程教学 · code review · 调试指导 · 算法练习 · 设计模式 · 面试准备 · 苏格拉底教学 · teach me · python · javascript

This repository is an **Agent Skill distribution package**. The core file `SKILL.md` follows the Agent Skills spec (YAML frontmatter) and packages the method of "用苏格拉底式引导学编程、过代码、练算法，不直接给答案" into a skill an AI agent can load directly. Drop it into your agent's skills directory (e.g. `~/.workbuddy/skills/`).

- **Category**: 编程教学 / Education
- **Version**: 1.0.0
- **Author**: 诺声(Logos)@SynomosAI
- **License**: MIT (see [LICENSE](LICENSE))

---

## Features

- 苏格拉底式教学：渐进提示（Hint 1→3）引导思考，不直接给答案
- 覆盖广：交互式学习、代码审查、调试指导、算法练习、项目指导、设计模式
- 语言：Python / JavaScript 为主
- 真实参照法：审查与讲解挂到语言规范、官方文档或可运行验证，不凭感觉断言
- 学员进度：内置 references/user-progress/learning_log.md 记录学习路线与掌握情况
- 多语种：中 / 英 / 日 / 韩 / 西 / 法 / 德 / 阿（核心 8 种）

---

## Quick Start

Prerequisite: an AI coding assistant / skill runtime that can load Agent Skills. 无独立可执行服务；本包为教学方法论 + 学习记录模板.

```bash
# 1. 克隆本仓库
git clone https://github.com/zhaoxinghua09-cell/code-mentor.git
cd code-mentor

# 2. 查看技能主文件（教学法、提示阶梯、代码审查口径）
cat SKILL.md

# 3. 查看 / 续接学员学习日志（画像、路线、已掌握主题）
cat references/user-progress/learning_log.md
```

Then invoke it in natural language, e.g.:

```text
「这段代码为什么错」
「怎么从零学 Python」
「面试算法怎么练 / 给我一道题」
```

---

## Usage

1. Clone this repo, or copy the skill directory into your agent's skills folder.
2. Call the capability via the trigger keywords described in `SKILL.md`.
3. See `SKILL.md` for the full method, boundaries and provenance.

---

## Repository layout

```text
code-mentor/
├── README.md            # 本文件（双语）
├── README.en.md         # 英文版说明
├── SKILL.md             # 技能主文件（Agent Skills 规范 · YAML frontmatter）
├── manifest.json        # 技能元数据（名称 / 版本 / 许可 / 描述）
├── references/
│   └── user-progress/
│       └── learning_log.md   # 学员学习日志与进度
├── LICENSE              # MIT 许可全文
├── SECURITY.md          # 安全策略
├── CONTRIBUTING.md      # 贡献指南
├── AGENTS.md            # 给 AI Agent 的工作指引
├── llms.txt             # 给 AI 的最小索引（llms.txt 标准）
└── llms-full.txt        # 给 AI 的完整文本
```

---

## License

Released under the **MIT** license. See [LICENSE](LICENSE) for the full text. Attribution: cite this repository `https://github.com/zhaoxinghua09-cell/code-mentor` and the rights holder "赵兴华 / Steven Zhao·China". Contact: zhaoxinghua06@126.com ｜ ORCID 0009-0001-0512-1237.

---

## Security

If you find a security issue, report it privately per [SECURITY.md](SECURITY.md); do not disclose it in a public issue.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Keep the `SKILL.md` YAML frontmatter fields compatible when changing this skill.

## Disclaimer

This repository content is a **theoretical stance and tooling exploration**. It does not represent any certified, commercially delivered, or client-served claim. External standards, certifications and clause information are restatements of public sources; independently verify before formal citation. APIs, authorization codes and ambassadors are roadmap items, not yet live.
