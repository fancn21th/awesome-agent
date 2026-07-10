# Awesome Agent [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 精选 AI 智能体、框架、工具与资源列表。

[English](README.md) | 中文

学习技巧：[English Version](AI_TRICKS.md) | [AI 使用技巧](AI_TRICKS_zh.md)

## 目录

- [智能体](#智能体)
- [应用](#应用)
- [Evals](#evals)
- [框架](#框架)
- [LLM 排行榜](#llm-排行榜)
- [资讯](#资讯)
- [个人推荐](#个人推荐)
- [平台](#平台)
- [定价](#定价)
- [提示词](#提示词)
- [研究](#研究)
- [技能](#技能)
- [工具](#工具)
- [教程](#教程)

## 智能体

- [A List of Claude Code Agents](https://github.com/hesreallyhim/a-list-of-claude-code-agents) by Really Him - 社区提交的 Claude Code 子智能体与智能体框架合集。
- [Agentics](https://github.com/githubnext/agentics) by GitHub Next - 可复用的 GitHub Agentic Workflows 示例包，涵盖仓库维护、代码审查、CI 分析、安全扫描、文档更新等。

## 应用

## Evals

- [evals](https://developers.openai.com/cookbook/topic/evals) - OpenAI Cookbook 的评测主题页，涵盖评估示例、模式与实践指南。
- [Evaluating the Effectiveness of LLM-Evaluators (aka LLM-as-a-Judge)](https://eugeneyan.com/writing/llm-evaluators/) by Eugene Yan - 深入分析 LLM-as-a-judge 的优势、失效模式与评估权衡。
- [AI Agent Observability & Evaluation](https://huggingface.co/learn/agents-course/bonus-unit2/introduction) by Hugging Face - 聚焦 AI 智能体可观测性与评估的课程章节。
- [Frequently Asked Questions (And Answers) About AI Evals](https://hamel.dev/blog/posts/evals-faq/) by Hamel Husain - 围绕评测设计、流程与度量问题的实用问答。
- [Your AI Product Needs Evals](https://hamel.dev/blog/posts/evals/) by Hamel Husain - 论证为何应将 evals 作为 AI 产品开发的一等公民。
- [Creating an LLM-as-a-Judge That Drives Business Results](https://hamel.dev/blog/posts/llm-judge/) by Hamel Husain - 讲解如何设计与业务结果对齐的 judge-based evals。
- [Voice AI Evals](https://github.com/kwindla/evals-course-voice) by Kwindla Hultman Kramer - 用于测试语音 AI 智能体与工作流的开放评测仓库。

## 框架

- [Get Shit Done](https://github.com/gsd-build/get-shit-done) by GSD - 轻量级元提示、上下文工程与规范驱动开发系统，通过全新子智能体会话、并行波执行和原子 git 提交解决上下文腐化问题。支持 15+ AI 编程运行时。
- [gstack](https://github.com/garrytan/gstack) by Garry Tan - Garry Tan 为 Claude Code 打造的虚拟工程团队——23 个主观斜杠命令技能，覆盖 CEO 审查、设计、工程、QA、安全审计和发布，配备真实浏览器自动化与多智能体协调。
- [Superpowers](https://github.com/obra/superpowers) by Jesse Vincent - 面向编程智能体的技能框架与软件开发方法论，涵盖 TDD、子智能体驱动开发、头脑风暴和系统化调试技能。支持 Claude Code、Codex、Cursor、Gemini CLI 等。

## LLM 排行榜

- [Claw-Eval](https://claw-eval.github.io/) by Bowen Ye & Lei Li (PKU/HKU) - 面向自主智能体的可信评估基准，覆盖通用、多轮和多模态任务，带安全感知评分。
- [ProjDevBench](https://github.com/zsworld6/projdevbench) by Pengrui Lu - 评估 AI 编程智能体端到端项目开发能力的基准，采用双评估（在线评测 + LLM 代码审查）、Docker 隔离，支持 Claude Code、Cursor、Gemini CLI、Codex、Augment 和 Copilot。
- [Vellum LLM Leaderboard](https://www.vellum.ai/llm-leaderboard) by Vellum - SOTA 模型最新公开基准表现，包含 GPQA Diamond、AIME 2025、SWE-Bench、Humanity's Last Exam、ARC-AGI 2、MMMLU 等成绩。

## 资讯

- [AI HOT](https://aihot.virxact.com/agent) by Virxact - AI 资讯聚合与每日精选，支持趋势追踪，提供 REST API、RSS 及 SKILL.md 编程智能体集成。
- [AI News](https://buttondown.com/ainews) - 汇总 Discord、Reddit 与 X 上重要 AI 讨论的每日通讯。
- [Last Week in AI](https://www.lastweekinai.com/) - 每周覆盖 AI 新闻与研究进展的播客和通讯。
- [Latent Space](https://www.latent.space/podcast) - 聚焦前沿 AI 议题深度解析与访谈的播客。
- [Stratechery](https://stratechery.com/) - 关注科技战略、行业分析与 AI 趋势的通讯和播客。
- [Smol AI News](https://news.smol.ai/) by smol.ai - 聚合模型、工具与研究动态的 AI 每日通讯，附精选链接与评论。

## 平台

## 定价

- [OpenAI API Pricing](https://developers.openai.com/api/docs/pricing#web-search) by OpenAI - OpenAI 官方 API 定价参考，覆盖旗舰、多模态、专项与微调模型，并包含 Web Search、File Search、Containers 与 Agent Kit 等工具成本。

## 提示词

- [system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) by asgeirtj - 用于分析与比较 AI 产品系统提示词的公开与泄露提示词精选合集。
- [The Prompt Report: A Systematic Survey of Prompting Techniques](https://arxiv.org/pdf/2406.06608) - 系统梳理提示技术、模式与 LLM 系统评估考量的综述论文。
- [Prompt Engineering Guide](https://www.promptingguide.ai/) by DAIR.AI - 面向现代 LLM 应用的提示工程综合指南，涵盖技术、示例与最佳实践。
- [Learn Prompting](https://learnprompting.org/docs) - 面向提示技术与 LLM 使用模式的结构化文档与指南。
- [How to prompt o1](https://www.latent.space/p/o1-skill-issue) by Ben Hylak - 深入讨论如何为并非针对聊天交互优化的推理模型设计提示。

## 研究

## 技能

- [Agent Skills](https://github.com/addyosmani/agent-skills) by Addy Osmani - 面向 AI 编程智能体的生产级工程技能包，覆盖 23 个生命周期技能、斜杠命令、专家 persona 与以验证为核心的工作流。
- [Andrej Karpathy Skills](https://github.com/forrestchang/andrej-karpathy-skills) by Jiayuan Zhang - 受 Karpathy 启发的 CLAUDE.md 指南，针对 LLM 编程缺陷提出四项原则：先思考再编码、简洁优先、精准修改、目标驱动执行。
- [Andrej Karpathy Skills](https://github.com/multica-ai/andrej-karpathy-skills) by Multica AI - 受 Karpathy 启发的 Claude Code 指南，用于规避 LLM 编程陷阱，强调先思考再编码、简洁优先、精准修改与目标驱动执行。
- [Anthropic Skills](https://github.com/anthropics/skills) by Anthropic - Anthropic 官方 Claude Code 技能集，包括 skill-creator（创建、评估和优化技能并提供基准测试）等。
- [Awesome Agent Skills](https://github.com/VoltAgent/awesome-agent-skills) by VoltAgent - 精选 1100+ 智能体技能合集，来自官方开发团队和社区，兼容 Claude Code、Codex、Gemini CLI、Cursor 等。
- [Matt Pocock Skills](https://github.com/mattpocock/skills) by Matt Pocock - 面向真实工程的小型可组合智能体技能——涵盖深度审查、TDD、诊断循环、代码架构改进、分类和领域驱动文档。兼容 Claude Code、Codex 及其他编程智能体。
- [Obsidian Skills](https://github.com/kepano/obsidian-skills) by Steph Ango - 面向 Obsidian 的智能体技能，教编程智能体使用 Obsidian Markdown、Bases、JSON Canvas、CLI 和 Defuddle。遵循 Agent Skills 规范，兼容 Claude Code、Codex CLI、OpenCode 等。
- [Startup Claude Skills](https://github.com/EricTechPro/startup-claude-skills) by Eric Tech - 面向初创团队的可复用 Claude Code 技能，涵盖 Bug 修复、功能开发、PR 审查、自动审查-修复循环和无头浏览器 QA 测试。
- [UI UX Pro Max Skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) by NextLevelBuilder - 面向编程智能体的专业 UI/UX AI 技能，提供智能设计系统生成、多平台栈指导与实用工作流支持。
- [Vercel React Best Practices](https://github.com/vercel-labs/agent-skills/blob/main/skills/react-best-practices/SKILL.md) by Vercel - 面向 React 和 Next.js 的性能优化指南，包含 8 大类别下的 70 条规则，适用于前端代码编写、审查与重构。

## 工具

- [The OSS LLMOps Stack](https://oss-llmops-stack.com/) by LiteLLM and Langfuse - 覆盖模型路由、可观测性与生产工作流的开源 LLMOps 栈参考页面。

## 教程

- [Agentic Design Patterns](https://adp.xindoo.xyz/) by xindoo - AI 智能体设计模式系统介绍，涵盖提示链、路由、并行化、反思、工具使用、规划、多智能体协作、记忆管理、学习与适应、MCP 等。
- [Harness Engineering: from Claude Code to AI Coding](https://zhanghandong.github.io/harness-engineering-from-cc-to-ai-coding/) by Handong Zhang - 面向 AI 编程工作流的实用指南，涵盖环境搭建模式、智能体协作与实现实践。
- [Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) by Anthropic - Anthropic 关于使用简单可组合模式构建 LLM 智能体的指南——涵盖增强 LLM、提示链、路由、并行化、编排-工作者、评估-优化器和自主智能体，附工具工程实践建议。
- [Learn Claude Code](https://learn.shareai.run/en/) by CrazyBoyM / shareAI-lab - 4 阶段 19 章，从最小智能体循环到多智能体平台，涵盖工具使用、子智能体、技能、上下文压缩、权限、钩子、记忆、错误恢复、任务调度、团队协议、工作树隔离和 MCP。
- [Beginners Guide to Machine Learning in JavaScript](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6YPSwT06y_AEYTqIwbeam3y) by The Coding Train - 面向初学者的机器学习 JavaScript 播放列表，介绍核心概念与实践实现。
- [YouTube Tutorials](https://github.com/owainlewis/youtube-tutorials/tree/main/tutorials) by Owain Lewis - 面向 AI 自动化模式的 YouTube 教程配套独立仓库，涵盖 RAG、智能体团队、后台智能体、多智能体系统、规范驱动开发等。
- [Effective Context Engineering for AI Agents](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents) by Anthropic - 关于如何为智能体系统组织与管理上下文的实践指南。
- [Hugging Face Agents Course](https://huggingface.co/agents-course) by Hugging Face - 免费的 AI 智能体构建、使用与评估课程。
- [How We Built Ellipsis](https://www.ellipsis.dev/blog/how-we-built-ellipsis) by Nick Bradford - 回顾 27 个月构建 LLM 编码智能体的工程实践。
- [Don’t Build Multi-Agents](https://cognition.ai/blog/dont-build-multi-agents#principles-of-context-engineering) by Walden Yan - 主张以更简单的系统和上下文工程替代不必要的多智能体复杂度。
- [We Built a Multi-Agent Research System](https://www.anthropic.com/engineering/built-multi-agent-research-system) by Anthropic - 介绍多智能体研究工作流的设计与运行案例。
- [What We Learned from a Year of Building with LLMs](https://www.oreilly.com/radar/what-we-learned-from-a-year-of-building-with-llms-part-i/) by Eugene Yan, Bryan Bischof, Charles Frye, Hamel Husain, Jason Liu, and Shreya Shankar - 总结构建、评估与运营 LLM 系统的一年期三篇系列实战经验。
- [Traceability and Observability in Multi-Step LLM Systems](https://langfuse.com/guides/videos/webinar-observability-llm-systems) by Marc Klingen - 介绍多步骤 LLM 应用追踪与可观测性的 Webinar。
- [Data Flywheels for LLM Applications](https://www.sh-reya.com/blog/ai-engineering-flywheel/) by Shreya Shankar - 讲解如何通过数据飞轮持续改进 LLM 产品的实践文章。
- [Latency optimization](https://platform.openai.com/docs/guides/latency-optimization) by OpenAI - 用于降低 LLM 应用端到端延迟的 Cookbook 指南。
- [Voice AI & Voice Agents - An Illustrated Primer](https://voiceaiandvoiceagents.com/) by Kwindla Hultman Kramer - 语音 AI 系统与语音智能体的图解入门读物。
- [Evaluating Voice AI Agents](https://langfuse.com/blog/2025-01-22-evaluating-voice-ai-agents) by Marc Klingen and Brooke Hopkins - 讲解如何在真实工作流中评估语音 AI 智能体。
- [Intro to Large Language Models](https://www.youtube.com/watch?v=zjkBMFhNj_g) by Andrej Karpathy - 面向初学者介绍 LLM 核心概念与思维模型的演讲。
- [How I use LLMs](https://www.youtube.com/watch?v=EWvNQjAaOHw) by Andrej Karpathy - 分享如何高效日常使用 LLM 的实践演讲。
- [AI Engineer Workshop 2026](https://www.aihero.dev/ai-engineer-workshop-2026~dwnll) by AI Hero - 面向 AI 工程实践、工具与工作流的动手工作坊资源。

## 个人推荐

- [What Is An AI Engineer?](https://www.aihero.dev/what-is-an-ai-engineer) by AI Hero - 清晰介绍 AI 工程师的角色定义、核心技能，以及它与机器学习工程和提示工程的区别。

## 贡献

欢迎贡献！请先阅读[贡献指南](CONTRIBUTING.md)。

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
