# Financial Freedom Path Skill

一个中文 AI Agent Skill Pack，把博多·舍费尔《财务自由之路》系列中的方法论整理为可按场景调用的行动框架。

本项目最初使用 Grok 辅助生成，现以开源形式分享。它不是原书替代品，也不是博多·舍费尔或相关出版方的官方项目。

## 包含内容

- 价值观与财务目标对齐
- 债务清理
- “先支付自己”的自动储蓄系统
- 提高收入
- 财务保障、财务安全与财务自由三阶段目标
- 复利与基础投资原则
- 教练及专家网络

## 安装

将 [`financial-freedom-path`](financial-freedom-path/) 目录复制到支持 `SKILL.md` 的 Agent 技能目录中。例如，在 Codex 中可放到：

```text
~/.codex/skills/financial-freedom-path/
```

重新启动或刷新 Agent 后，直接描述你的问题，例如：

```text
帮我用“先支付自己”的方法设计一个储蓄计划。
```

也可以显式调用：

```text
使用 $financial-freedom-path，帮我规划清理信用卡债务的顺序。
```

详细的子技能和推荐顺序见 [`INDEX.md`](financial-freedom-path/INDEX.md)。

## 目录结构

```text
financial-freedom-path/
├── SKILL.md
├── agents/openai.yaml
├── INDEX.md
├── BOOK_OVERVIEW.md
├── DIGEST.md
└── */SKILL.md
```

## 免责声明

本项目仅用于教育和一般信息参考，不构成个性化的投资、税务、法律或其他专业建议。任何数字、收益率或资产配置示例都需要结合所在地区法规、个人风险承受能力和实际情况独立判断；必要时请咨询持证专业人士。

本项目是对相关书籍思想的独立概括与实践化整理。书名、作者名及相关标识归各自权利人所有。若你喜欢这些方法，请购买并阅读正版原著。

## License

[MIT](LICENSE)

