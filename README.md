# Awesome Agent Engineering [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> The engineering map for building production AI agents.

English | [中文](README_zh.md)

This repository is organized by engineering layers rather than by asset type, so frameworks, products, patterns, skills, runtimes, and production concerns are easier to compare without mixing levels.

Companion Guides: [Agent Level](AGENT_LEVEL.md) | [RAG Level](RAG_LEVEL.md) | [AI Usage Tips](AI_TRICKS.md)

## Contents

- [Foundation](#foundation)
- [Agent Patterns](#agent-patterns)
- [Frameworks and Spec-Driven Systems](#frameworks-and-spec-driven-systems)
- [Runtime, Tooling, and Production Ops](#runtime-tooling-and-production-ops)
- [Observability, Evals, and Benchmarks](#observability-evals-and-benchmarks)
- [Coding Agents, Skills, and Agentic SDLC](#coding-agents-skills-and-agentic-sdlc)
- [Vertical Agents and Applications](#vertical-agents-and-applications)
- [Learning Path](#learning-path)
- [Research, News, and Market Signals](#research-news-and-market-signals)
- [Personal Recommendation](#personal-recommendation)

## Foundation

- [models.dev](https://models.dev/) - Open-source database for exploring AI models, capabilities, context limits, and pricing.
- [Prompt Engineering Guide](https://www.promptingguide.ai/) by DAIR.AI - Comprehensive guide to prompt engineering techniques, examples, and best practices for modern LLM applications.
- [Learn Prompting](https://learnprompting.org/docs) - Structured documentation and guides for prompting techniques and LLM usage patterns.
- [The Prompt Report: A Systematic Survey of Prompting Techniques](https://arxiv.org/pdf/2406.06608) - Survey paper covering prompting techniques, patterns, and evaluation considerations for LLM systems.
- [How to prompt o1](https://www.latent.space/p/o1-skill-issue) by Ben Hylak - Deep dive on prompting reasoning models that are not optimized for chat-style interaction.
- [Intro to Large Language Models](https://www.youtube.com/watch?v=zjkBMFhNj_g) by Andrej Karpathy - Beginner-friendly talk introducing core LLM concepts and mental models.
- [How I use LLMs](https://www.youtube.com/watch?v=EWvNQjAaOHw) by Andrej Karpathy - Practical talk on effective day-to-day use of LLMs.

## Agent Patterns

- [Agentic Design Patterns](https://adp.xindoo.xyz/) by xindoo - Systematic introduction to AI agent design patterns, covering prompt chaining, routing, parallelization, reflection, tool use, planning, multi-agent collaboration, memory management, learning and adaptation, MCP, and more.
- [Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) by Anthropic - Anthropic's guide on building LLM agents with simple, composable patterns — covers augmented LLM, prompt chaining, routing, parallelization, orchestrator-workers, evaluator-optimizer, and autonomous agents, with practical advice on tool engineering.
- [Effective Context Engineering for AI Agents](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents) by Anthropic - Practical guidance for structuring and managing context in agentic systems.
- [Don’t Build Multi-Agents](https://cognition.ai/blog/dont-build-multi-agents#principles-of-context-engineering) by Walden Yan - Argument for simpler agent systems with context engineering over unnecessary multi-agent complexity.
- [We Built a Multi-Agent Research System](https://www.anthropic.com/engineering/built-multi-agent-research-system) by Anthropic - Case study on designing and operating a multi-agent research workflow.

## Frameworks and Spec-Driven Systems

- [Agentics](https://github.com/githubnext/agentics) by GitHub Next - Sample pack of reusable GitHub Agentic Workflows for repository maintenance, code review, CI analysis, security scanning, documentation updates, and more.
- [Get Shit Done](https://github.com/gsd-build/get-shit-done) by GSD - A lightweight meta-prompting, context engineering, and spec-driven development system that solves context rot with fresh subagent sessions, parallel wave execution, and atomic git commits. Supports 15+ AI coding runtimes.
- [gstack](https://github.com/garrytan/gstack) by Garry Tan - Garry Tan's virtual engineering team for Claude Code — 23 opinionated slash-command skills covering CEO review, design, engineering, QA, security audit, and release, with real browser automation and multi-agent coordination.
- [Superpowers](https://github.com/obra/superpowers) by Jesse Vincent - An agentic skills framework and software development methodology for coding agents, featuring TDD, subagent-driven development, brainstorming, and systematic debugging skills. Supports Claude Code, Codex, Cursor, Gemini CLI, and more.

## Runtime, Tooling, and Production Ops

- [The OSS LLMOps Stack](https://oss-llmops-stack.com/) by LiteLLM and Langfuse - Reference page for an open-source LLMOps stack spanning model routing, observability, and production workflows.
- [OpenAI API Pricing](https://developers.openai.com/api/docs/pricing#web-search) by OpenAI - Official API pricing reference covering flagship, multimodal, specialized, and fine-tuning models, plus tool costs for web search, file search, containers, and agent kit.
- [system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) by asgeirtj - Curated collection of leaked and public system prompts from AI products for analysis and comparison.
- [What We Learned from a Year of Building with LLMs](https://www.oreilly.com/radar/what-we-learned-from-a-year-of-building-with-llms-part-i/) by Eugene Yan, Bryan Bischof, Charles Frye, Hamel Husain, Jason Liu, and Shreya Shankar - Three-part series on production lessons for building, evaluating, and operating LLM systems.
- [Data Flywheels for LLM Applications](https://www.sh-reya.com/blog/ai-engineering-flywheel/) by Shreya Shankar - Practical article on using data flywheels to improve LLM products.
- [Latency optimization](https://platform.openai.com/docs/guides/latency-optimization) by OpenAI - Cookbook guide for reducing end-to-end latency in LLM applications.

## Observability, Evals, and Benchmarks

- [evals](https://developers.openai.com/cookbook/topic/evals) - OpenAI Cookbook topic page for evaluation examples, patterns, and guidance.
- [Evaluating the Effectiveness of LLM-Evaluators (aka LLM-as-a-Judge)](https://eugeneyan.com/writing/llm-evaluators/) by Eugene Yan - Detailed analysis of LLM-as-a-judge strengths, failure modes, and evaluation tradeoffs.
- [AI Agent Observability & Evaluation](https://huggingface.co/learn/agents-course/bonus-unit2/introduction) by Hugging Face - Course unit on observability and evaluation for AI agents.
- [Frequently Asked Questions (And Answers) About AI Evals](https://hamel.dev/blog/posts/evals-faq/) by Hamel Husain - Practical answers to common evaluation design, process, and measurement questions.
- [Your AI Product Needs Evals](https://hamel.dev/blog/posts/evals/) by Hamel Husain - Practical case for making evals a first-class part of AI product development.
- [Creating an LLM-as-a-Judge That Drives Business Results](https://hamel.dev/blog/posts/llm-judge/) by Hamel Husain - Guide to designing judge-based evals that align with business outcomes.
- [Voice AI Evals](https://github.com/kwindla/evals-course-voice) by Kwindla Hultman Kramer - Open evaluation repo for testing voice AI agents and workflows.
- [Traceability and Observability in Multi-Step LLM Systems](https://langfuse.com/guides/videos/webinar-observability-llm-systems) by Marc Klingen - Webinar on tracing and observability for multi-step LLM applications.
- [Evaluating Voice AI Agents](https://langfuse.com/blog/2025-01-22-evaluating-voice-ai-agents) by Marc Klingen and Brooke Hopkins - Guide to evaluating voice AI agents in real-world workflows.
- [Claw-Eval](https://claw-eval.github.io/) by Bowen Ye & Lei Li (PKU/HKU) - Trustworthy evaluation benchmark for autonomous agents, covering general, multi-turn, and multimodal tasks with safety-aware scoring.
- [ProjDevBench](https://github.com/zsworld6/projdevbench) by Pengrui Lu - Benchmark for evaluating AI coding agents on end-to-end project development, with dual evaluation (Online Judge + LLM code review), Docker isolation, and support for Claude Code, Cursor, Gemini CLI, Codex, Augment, and Copilot.
- [Vellum LLM Leaderboard](https://www.vellum.ai/llm-leaderboard) by Vellum - Latest public benchmark performance for SOTA models, featuring results from GPQA Diamond, AIME 2025, SWE-Bench, Humanity's Last Exam, ARC-AGI 2, MMMLU, and more.

## Coding Agents, Skills, and Agentic SDLC

This layer follows the delivery chain from requirement and architecture to coding, testing, review, documentation, and release.

### Coding Agents and Systems

- [A List of Claude Code Agents](https://github.com/hesreallyhim/a-list-of-claude-code-agents) by Really Him - Community-submitted collection of Claude Code sub-agents and agent frameworks.
- [Harness Engineering: from Claude Code to AI Coding](https://zhanghandong.github.io/harness-engineering-from-cc-to-ai-coding/) by Handong Zhang - Practical guide to harness engineering for AI coding workflows, covering setup patterns, agent collaboration, and implementation practices.
- [Learn Claude Code](https://learn.shareai.run/en/) by CrazyBoyM / shareAI-lab - 19 chapters across 4 stages, from the minimal agent loop to a multi-agent platform, covering tool use, subagents, skills, context compaction, permissions, hooks, memory, error recovery, task scheduling, team protocols, worktree isolation, and MCP.
- [How We Built Ellipsis](https://www.ellipsis.dev/blog/how-we-built-ellipsis) by Nick Bradford - Engineering retrospective on building LLM coding agents over 27 months.

### Skills

- [Agent Skills](https://github.com/addyosmani/agent-skills) by Addy Osmani - Production-grade engineering skills for AI coding agents, covering 23 lifecycle skills, slash commands, personas, and verification-driven workflows.
- [Andrej Karpathy Skills](https://github.com/forrestchang/andrej-karpathy-skills) by Jiayuan Zhang - Karpathy-inspired CLAUDE.md guidelines addressing LLM coding pitfalls with four principles: think before coding, simplicity first, surgical changes, and goal-driven execution.
- [Andrej Karpathy Skills](https://github.com/multica-ai/andrej-karpathy-skills) by Multica AI - Karpathy-inspired Claude Code guidelines for avoiding LLM coding pitfalls with think-before-coding, simplicity-first, surgical changes, and goal-driven execution.
- [Anthropic Skills](https://github.com/anthropics/skills) by Anthropic - Anthropic's official skill collection for Claude Code, including skill-creator (create, evaluate, and optimize skills with benchmarking), and more.
- [Awesome Agent Skills](https://github.com/VoltAgent/awesome-agent-skills) by VoltAgent - Curated collection of 1100+ agent skills from official dev teams and the community, compatible with Claude Code, Codex, Gemini CLI, Cursor, and more.
- [Matt Pocock Skills](https://github.com/mattpocock/skills) by Matt Pocock - Small, composable agent skills for real engineering — covers grilling sessions, TDD, diagnosis loops, codebase architecture improvement, triage, and domain-driven documentation. Compatible with Claude Code, Codex, and other coding agents.
- [Obsidian Skills](https://github.com/kepano/obsidian-skills) by Steph Ango - Agent skills for Obsidian, teaching your coding agent to use Obsidian Markdown, Bases, JSON Canvas, CLI, and Defuddle. Follows the Agent Skills specification, compatible with Claude Code, Codex CLI, OpenCode, and more.
- [Startup Claude Skills](https://github.com/EricTechPro/startup-claude-skills) by Eric Tech - Reusable Claude Code skills for startups, covering bug fixing, feature development, PR review, automated review-fix loops, and headless browser QA testing.
- [UI UX Pro Max Skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) by NextLevelBuilder - AI skill for professional UI/UX development with intelligent design-system generation, multi-platform stack guidance, and practical workflow support for coding agents.
- [Vercel React Best Practices](https://github.com/vercel-labs/agent-skills/blob/main/skills/react-best-practices/SKILL.md) by Vercel - React and Next.js performance optimization guidelines with 70 rules across 8 categories for writing, reviewing, and refactoring frontend code.

### Agentic SDLC Learning Resources

- [YouTube Tutorials](https://github.com/owainlewis/youtube-tutorials/tree/main/tutorials) by Owain Lewis - Self-contained companion repos for YouTube tutorials on practical AI automation patterns, covering RAG, agent teams, background agents, multi-agent systems, spec-driven development, and more.
- [AI Engineer Workshop 2026](https://www.aihero.dev/ai-engineer-workshop-2026~dwnll) by AI Hero - Hands-on workshop resource for AI engineering practices, tools, and workflows.

## Vertical Agents and Applications

This is the next expansion layer for the list: domain agents for CAD, manufacturing, supply chain, ERP, BI, and knowledge work.

- [Voice AI & Voice Agents - An Illustrated Primer](https://voiceaiandvoiceagents.com/) by Kwindla Hultman Kramer - Illustrated primer on voice AI systems and voice agents.

## Learning Path

- [Hugging Face Agents Course](https://huggingface.co/agents-course) by Hugging Face - Free course on building, using, and evaluating AI agents.
- [Beginners Guide to Machine Learning in JavaScript](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6YPSwT06y_AEYTqIwbeam3y) by The Coding Train - Beginner-friendly playlist introducing machine learning concepts and practical implementations in JavaScript.

## Research, News, and Market Signals

- [AI HOT](https://aihot.virxact.com/agent) by Virxact - Curated AI news aggregator with daily digests and trend tracking, offering REST API, RSS, and SKILL.md integration for coding agents.
- [AI News](https://buttondown.com/ainews) - Daily roundup of notable AI discussions from Discord, Reddit, and X.
- [Last Week in AI](https://www.lastweekinai.com/) - Weekly podcast and newsletter covering AI news and research.
- [Latent Space](https://www.latent.space/podcast) - Podcast with deep dives and interviews on frontier AI topics.
- [Stratechery](https://stratechery.com/) - Newsletter and podcast focused on tech strategy, industry analysis, and AI trends.
- [Smol AI News](https://news.smol.ai/) by smol.ai - Daily AI newsletter with curated links, commentary, and key updates across models, tools, and research.

## Personal Recommendation

- [What Is An AI Engineer?](https://www.aihero.dev/what-is-an-ai-engineer) by AI Hero - Clear introduction to AI engineering, covering the role definition, core skills, and how it differs from ML engineering and prompt engineering.

## Contributing

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
