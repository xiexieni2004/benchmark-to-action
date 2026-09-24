# benchmark-to-action

一个面向 Codex 及其他 Agent Skills 客户端的商业对标分析 Skill。

它帮助用户：

- 在没有候选对象时，建立关键词矩阵、筛选标准和停止搜索条件；
- 验证并拆解用户提供的账号、内容、产品或业务；
- 区分事实、信号、推断和未知，不根据粉丝量或报价虚构利润；
- 检查人设—内容、内容—产品、流量—成交是否匹配；
- 把对标动作转化为符合用户资源的最小实验。

它不会替用户直接搜索、点名或推荐真实对标，也不会帮助仿写作品、复刻视觉、冒用人设或承诺盈利。

## 安装

```bash
npx -y skills add xiexieni2004/benchmark-to-action -g --all
```

## 使用

安装后可以显式调用 `$benchmark-to-action`，也可以直接描述相应任务。

### 尚无候选对象

> 使用 $benchmark-to-action。我想在小红书做家庭收纳咨询，但还没有候选对象。请帮我制定寻找和筛选对标的策略，不要直接推荐账号。

### 已有候选对象

> 使用 $benchmark-to-action。下面是我整理的一个候选账号，请区分事实、推断和未知，判断它是否值得研究，并拆解内容、产品和成交路径。

### 把动作改成自己能执行的方案

> Use $benchmark-to-action to analyze a benchmark I provide and turn its reusable mechanisms into a realistic action experiment.

建议同时提供：

- 候选对象的公开资料；
- 你的产品阶段、可投入时间和主要限制；
- 想验证的结果，例如内容表现、询单、成交或交付效率。

## 运行依赖

- 支持 Agent Skills 的客户端

## 内容

本仓库只发布运行这个 Skill 所需的文件。本地评测样本、预期答案和运行记录不包含在公开包中。

```text
skills/benchmark-to-action/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── action-adaptation.md
    ├── deconstruction.md
    ├── evidence-and-boundaries.md
    ├── finding-strategy.md
    └── xiaohongshu.md
```

## 隐私与边界

- 只分析用户主动提供或公开可访问的信息；
- 不索取或推断非公开个人与经营数据；
- 估算必须写明假设、范围、日期和置信度；
- 不把内容表现、商业结果和利润混为一谈；
- 用户应自行核实平台规则、法律、财务与专业风险。

## 许可证

[MIT License](LICENSE)
