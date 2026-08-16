# Financial Freedom Path Skill

一个中文 AI Agent Skill Pack，把博多·舍费尔《财务自由之路》系列中的方法论整理为可按场景调用的行动框架。

本项目最初使用 Grok 辅助生成，现以开源形式分享。它不是原书替代品，也不是博多·舍费尔或相关出版方的官方项目。

## 包含的 Skills

| Skill | 它解决什么问题 | 你会得到什么 |
|---|---|---|
| `values-goals-alignment` | 想改善财务，却总因金钱观冲突、目标模糊或缺乏内在动力而半途而废 | 金钱信念诊断、价值观排序和与理想生活相连的财务目标 |
| `debt-cleanup` | 同时背负多笔信用卡、消费贷或其他债务，不知道先还哪一笔 | 债务清单、偿还优先级、停止新增债务的规则和阶段性还款方案 |
| `pay-yourself-first` | 每月总是花光，依靠“月底剩多少存多少”却长期存不下钱 | 储蓄比例、账户分工、发薪日自动转账和加薪后的储蓄规则 |
| `increase-income` | 收入停滞，想谈薪、提高报价、发展副业或增强市场价值 | 收入瓶颈诊断、价值证明材料和可在本周执行的增收动作 |
| `three-stages-financial-freedom` | “财务自由”过于抽象，不知道需要多少钱、先到哪个里程碑 | 财务保障、安全与自由三个目标数字，以及从当前状态倒推的行动计划 |
| `compound-feeding-money` | 已有结余，但不知道如何开始长期投资，或容易被短期波动影响 | 基于期限与风险承受能力的资金分层、持续投入和再平衡原则 |
| `coach-network` | 知道方法却执行不下去，缺少反馈、问责和可信赖的专业支持 | 教练需求定义、筛选标准、合作规则和专家网络建设计划 |

主 skill `financial-freedom-path` 会先判断问题属于哪个阶段，再按需组合上述子 skill，输出一份连贯的财务行动路径。

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
