# 拆穿 · Deconstruct Anything


[![Stars](https://img.shields.io/github/stars/Leowu9839/=social)](https://github.com/Leowu9839/deconstruct-skill/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> 🏠 这是 [Leo's AI Skill Workshop](https://github.com/Leowu9839/leos-workshop) 的 6 大 Skill 之一，点击查看完整项目集。
> 把任何 AI Skill 掰开揉碎——消除黑箱，按需学习，安全审计，融合进化。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Codex%20%7C%20Claude%20%7C%20Cursor-blue)]()

---

## ⚡ 1 分钟安装

```bash
# 克隆到 Codex skills 目录
git clone https://github.com/Leowu9839/deconstruct-skill.git
cp -r deconstruct-skill/SKILL.md ~/.codex/skills/deconstruct-skill/

# 或者直接复制 SKILL.md 到任一兼容平台的 skills 目录
# Codex:        ~/.codex/skills/deconstruct-skill/
# Claude Code:  ~/.claude/skills/deconstruct-skill/
# Cursor:       .cursor/rules/
```

安装后重启 AI 工具，输入「拆穿它」+ 任意 Skill 内容即可触发。

---

## 🎯 这是什么

当你面对一个 AI Skill（无论自己写的还是 GitHub 上找的），会有三个问题：

1. **它到底用了什么手段？** 为什么比别人写的更好用？
2. **安不安全？** 里面有没有恶意指令、会不会把你的数据发到第三方？
3. **我能学到什么？** 有什么设计思路可以迁移到我自己的 Skill 里？

「拆穿」一次性回答这三个问题。它把任何完整 Skill 拆解成一份结构化的 Markdown 报告——人类可读、AI 可用。

---

## 🔬 拆解报告包含什么

| 章节 | 内容 | 为谁服务 |
|------|------|---------|
| 概览 | 一句话总结 + 本质矛盾 | 所有人 |
| 技术解剖 | API/MCP/工具/知识来源/串联方式 | 想学技术的人 |
| 安全审计 | 数据流向、外部调用、隐藏指令、权限边界 | 注重安全的人 |
| 设计决策 | 3-5 个关键决策及动机 | 想写 Skill 的人 |
| 思维组件 | 可独立复用的设计模式 + 变体 + 联动 | 积累设计能力的人 |
| 脆弱点 | 观察型 + 压力测试，最致命弱点 | 想改进 Skill 的人 |
| 进化方向 | 插件强化、串联方案、重造取舍 | 想融合创新的人 |

---

## 💡 设计哲学

**非技术用户优先。** 技术人员直接看原始 Skill 就够了。每份报告里，技术术语必加白话解释，安全判断必说「这对你意味着什么」。

**报告即基础设施。** 拆解报告不只是学习笔记，也是给 AI 的结构化上下文。AI 拿到原始 Skill 只知道「做什么」，拿到 Skill + 拆解报告才知道「为什么这么做、边界在哪、哪里容易出错」。

**积累产生复利。** 拆得越多，思维组件库越大。把一堆报告丢给 AI，它能在结构化信息上直接做组合和进化分析。

---

## 🚀 使用方式

```
「帮我拆穿这个 Skill」+ 粘贴完整 Skill 内容
```

或者：

```
「这是我从 GitHub 找的 Skill，拆穿它」+ 粘贴内容
```

**注意：** 输入必须是完整实现（完整的 SKILL.md 内容），不接受摘
要或功能描述。信息不够会直接告知，不硬凑。

---

## 📋 示例

输入一个 Skill → 输出一份包含 7 个章节的 Markdown 报告，带有：

- TOC 目录，按需跳转
- 每个技术术语的白话括号注释
- ✅/⚠️/❌ 符号标记的安全审计表
- 可独立复用的思维组件卡片

---

## ⚠️ 边界

- 输入必须是完整实现，不做逆向推断
- 安全审计基于文本静态分析，无法检测运行时网络行为
- 联动分析范围限制在本次拆解的组件之间

---

## 📄 许可

MIT License · 欢迎使用、修改、分发。

如果你用它拆出了有趣的东西，欢迎提 PR 分享报告。

---

*Made with ❤️ for the AI Skill ecosystem.*

---

## 🔗 相关项目

这是 [Leo's AI Skill Workshop](https://github.com/Leowu9839/leos-workshop) 的一部分，更多 Skill：

| Skill | 场景 |
|:---|:---|
| 🏛️ [制度顾问](https://github.com/Leowu9839/policy-counsel) | 企业合规 / 政策分析 |
| 🐕 [数据宝藏猎犬](https://github.com/Leowu9839/data-treasure-hound) | 数据调研 / 信息挖掘 |
| ⚙️ [工程化 Agent](https://github.com/Leowu9839/engineering-agent) | 开发提效 / 自动化 |
| 💎 [富人生活顾问](https://github.com/Leowu9839/luxury-experience-designer) | 生活方式 / 品质提升 |
| ✈️ [LXTI 旅行人格](https://github.com/Leowu9839/lxti-travel-personality) | 旅行规划 / 人格测试 |
| 🔍 [拆穿 Skill](https://github.com/Leowu9839/deconstruct-skill) | 批判思维 / 信息甄别 |