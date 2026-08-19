# Awesome AI Coding Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of AI-powered tools for developers — editors, agents, code review, testing, CLI tools, MCP servers, and more.

AI coding has gone from autocomplete to autonomous teams in two years. This list helps you cut through the noise: the tools that ship, the tools that are interesting, and the tools that are quietly winning. Curated for working developers, not benchmark-chasers.

**Maintained by [LaunchApp](https://github.com/launchapp-dev).** Contributions welcome — see [contributing.md](contributing.md).

---

## Contents

- [AI Code Editors & IDEs](#ai-code-editors--ides)
- [In-Editor Assistants & Completion](#in-editor-assistants--completion)
- [Autonomous Coding Agents](#autonomous-coding-agents)
- [CLI & Terminal Coding Tools](#cli--terminal-coding-tools)
- [Agent Orchestrators & Multi-Agent](#agent-orchestrators--multi-agent)
- [Code Review & PR Automation](#code-review--pr-automation)
- [Testing & QA](#testing--qa)
- [Code Search & Codebase Intelligence](#code-search--codebase-intelligence)
- [Documentation Generation](#documentation-generation)
- [Web-Based App Builders](#web-based-app-builders)
- [Open-Source & Self-Hosted](#open-source--self-hosted)
- [Model Context Protocol (MCP)](#model-context-protocol-mcp)
- [DevOps & CI/CD](#devops--cicd)
- [Models for Coding](#models-for-coding)
- [Prompt & Context Engineering](#prompt--context-engineering)
- [Learning Resources](#learning-resources)
- [Related Lists](#related-lists)

---

## Legend

- 🟢 Open source
- 💰 Paid / commercial
- 🆓 Free tier available
- 🏠 Self-hostable
- ⭐ Editor's pick

---

## AI Code Editors & IDEs

Full IDEs and forks built around AI as a first-class feature.

- [Cursor](https://www.cursor.com/) ⭐ 💰 — AI-first VS Code fork. Multi-file edits, agent mode, codebase chat. Currently the category leader.
- [OpenMagic](https://github.com/Kalmuraee/OpenMagic) 🟢 — AI-powered coding toolbar for any web app. Captures element context, previews diffs, and applies approved changes through a reverse proxy.
- [Windsurf](https://windsurf.com/) 💰 — VS Code fork from Codeium with the "Cascade" agent. Strong long-running task support.
- [Zed](https://zed.dev/) 🟢 🆓 — Rust-built editor with native AI assistant and multibuffer edits. Fast.
- [Void](https://voideditor.com/) 🟢 — Open-source Cursor alternative. Bring your own model.
- [Trae](https://trae.ai/) 💰 — ByteDance's AI IDE with Builder/Chat modes.
- [PearAI](https://trypear.ai/) 🟢 — Open-source AI editor fork.

## In-Editor Assistants & Completion

Extensions that add AI to existing editors (VS Code, JetBrains, Vim, etc).

- [GitHub Copilot](https://github.com/features/copilot) ⭐ 💰 — The original. Inline completion, chat, agent mode, PR review.
- [Continue](https://github.com/continuedev/continue) 🟢 🆓 — Open-source autopilot for VS Code and JetBrains. Configurable models.
- [Codeium](https://codeium.com/) 🆓 — Free AI completion across 70+ editors.
- [Tabnine](https://www.tabnine.com/) 💰 🏠 — Privacy-focused completion. On-prem deployment available.
- [Supermaven](https://supermaven.com/) 💰 🆓 — Fast, long-context completion. Acquired by Cursor.
- [Cody](https://sourcegraph.com/cody) 🆓 💰 — Sourcegraph's assistant with codebase-wide context.
- [Amazon Q Developer](https://aws.amazon.com/q/developer/) 🆓 💰 — Formerly CodeWhisperer. Tight AWS integration.
- [JetBrains AI Assistant](https://www.jetbrains.com/ai/) 💰 — Native to all JetBrains IDEs.

## Autonomous Coding Agents

Agents that take a goal and execute multi-step work — planning, editing, testing, iterating.

- [Claude Code](https://docs.claude.com/en/docs/claude-code/overview) ⭐ 💰 — Anthropic's terminal-native agent. Strong tool use, MCP support.
- [Aider](https://aider.chat/) 🟢 🆓 ⭐ — Pair-programs from your terminal with git-aware diffs. Model-agnostic.
- [OpenAI Codex CLI](https://github.com/openai/codex) 🟢 — Lightweight terminal agent from OpenAI.
- [Gemini CLI](https://github.com/google-gemini/gemini-cli) 🟢 — Google's agent for the terminal.
- [Harness Desktop](https://github.com/baiyuscc13724-max/deepseek-harness-desktop) 🟢 — Windows client for the official DeepSeek Harness coding workbench with themes, provider and subagent model routing, and an in-app plugin and Skills marketplace.
- [Devin](https://devin.ai/) 💰 — Cognition's autonomous SWE. Browser, shell, editor in one sandbox.
- [OpenHands](https://github.com/All-Hands-AI/OpenHands) 🟢 🏠 — Open-source autonomous agent platform (formerly OpenDevin).
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) 🟢 — Princeton's research agent. Strong on SWE-bench.
- [Cline](https://github.com/cline/cline) 🟢 — Autonomous VS Code agent (formerly Claude Dev).
- [Roo Code](https://github.com/RooCodeInc/Roo-Code) 🟢 — Cline fork with multi-mode agent loop.
- [opencode](https://github.com/sst/opencode) 🟢 — Terminal-native AI coding agent from SST.

## CLI & Terminal Coding Tools

Lower-level CLI tooling that pairs with agents or runs solo.

- [Animus (ao-cli)](https://github.com/launchapp-dev/animus-cli) 🟢 ⭐ — Autonomous agent orchestrator. YAML workflows, daemon scheduling, multi-model routing across Claude/Gemini/GPT.
- [llm](https://github.com/simonw/llm) 🟢 — Simon Willison's CLI for talking to any LLM. Plugin ecosystem.
- [mods](https://github.com/charmbracelet/mods) 🟢 — Charm's AI for the command line. Pipes-friendly.
- [shell-gpt (sgpt)](https://github.com/TheR1D/shell_gpt) 🟢 — Shell command generation and chat.
- [aichat](https://github.com/sigoden/aichat) 🟢 — All-in-one CLI chat & agent in Rust.

## Agent Orchestrators & Multi-Agent

Frameworks for running multiple agents, coordinating workflows, or building your own coding agent.

- [Animus](https://github.com/launchapp-dev/animus-cli) 🟢 ⭐ — Production orchestrator: define an engineering team in YAML, dispatch tasks across isolated worktrees, route by complexity.
- [LangGraph](https://github.com/langchain-ai/langgraph) 🟢 — Stateful multi-agent graphs from LangChain.
- [CrewAI](https://github.com/crewAIInc/crewAI) 🟢 — Role-based multi-agent framework.
- [AutoGen](https://github.com/microsoft/autogen) 🟢 — Microsoft's conversational multi-agent framework.
- [Claude Agent SDK](https://github.com/anthropics/claude-agent-sdk-python) 🟢 — Build production agents on Claude.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) 🟢 — OpenAI's agent framework with handoffs and tracing.
- [Orkas](https://github.com/Orkas-AI/Orkas) 🟢 🆓 🏠 — Open-source, local-first desktop AI workforce whose Commander coordinates specialist and external coding agents through one chat.
- [smolagents](https://github.com/huggingface/smolagents) 🟢 — Hugging Face's minimal code-writing agents.

## Code Review & PR Automation

Tools that review pull requests, suggest improvements, or gate merges.

- [Bubo](https://github.com/mountainowl/bubo) 🟢 🆓 🏠 — Self-hosted AI code reviewer for GitHub and GitLab that posts evidence-backed inline findings or LGTM and learns from repository feedback.
- [CodeRabbit](https://www.coderabbit.ai/) 💰 🆓 — Line-by-line PR review. Most popular in this category.
- [Qodo (Codium)](https://www.qodo.ai/) 💰 🆓 — PR-Agent + test generation. Open-source PR-Agent available.
- [Greptile](https://www.greptile.com/) 💰 — Codebase-aware PR review.
- [Bito](https://bito.ai/) 💰 🆓 — AI code review & chat.
- [Ellipsis](https://www.ellipsis.dev/) 💰 — Async AI reviewer that fixes its own comments.
- [Diamond by Graphite](https://graphite.dev/diamond) 💰 — PR review built into Graphite's stack.

## Testing & QA

- [Qodo Cover](https://www.qodo.ai/products/qodo-cover/) 🟢 — Auto-generates regression tests with coverage targets.
- [Checksum](https://checksum.ai/) 💰 — AI-generated end-to-end tests from real user behavior.
- [Octomind](https://octomind.dev/) 💰 — AI E2E test generation and maintenance.
- [Meticulous](https://www.meticulous.ai/) 💰 — Auto-generates and maintains UI tests.
- [Momentic](https://momentic.ai/) 💰 — Low-code AI testing platform.

## Code Search & Codebase Intelligence

- [Sourcegraph](https://sourcegraph.com/) 💰 🆓 ⭐ — Code search + Cody AI across massive codebases.
- [Greptile](https://www.greptile.com/) 💰 — API for codebase Q&A.
- [Bloop](https://github.com/BloopAI/bloop) 🟢 — Open-source code search with semantic understanding.
- [Aider Repo Map](https://aider.chat/docs/repomap.html) 🟢 — Repo-map approach for giving LLMs codebase context.

## Documentation Generation

- [Mintlify Writer](https://writer.mintlify.com/) 🆓 — Auto-generated docstrings.
- [Swimm](https://swimm.io/) 💰 — AI-assisted, code-coupled documentation.
- [DocuWriter.ai](https://www.docuwriter.ai/) 💰 — Generates code, API, and test documentation.

## Web-Based App Builders

Prompt-to-app tools — for prototyping or full apps.

- [v0](https://v0.app/) ⭐ 💰 🆓 — Vercel's UI generator. React + Tailwind output.
- [Bolt.new](https://bolt.new/) 🆓 💰 — StackBlitz's full-stack web app builder.
- [Lovable](https://lovable.dev/) 💰 🆓 — End-to-end app generator with deploy.
- [Replit Agent](https://replit.com/agent) 💰 — In-browser app generation + hosting.
- [Tempo](https://www.tempo.new/) 💰 — Visual + AI React app builder.
- [a0.dev](https://a0.dev/) — React Native app generator.

## Open-Source & Self-Hosted

For when you want to own the stack.

- [Continue](https://github.com/continuedev/continue) 🟢 🏠 — Self-hostable IDE assistant.
- [TabbyML](https://github.com/TabbyML/tabby) 🟢 🏠 — Self-hosted Copilot alternative.
- [OpenHands](https://github.com/All-Hands-AI/OpenHands) 🟢 🏠 — Self-host an autonomous SWE agent.
- [LiteLLM](https://github.com/BerriAI/litellm) 🟢 🏠 — Unified gateway for 100+ LLM providers.
- [Ollama](https://github.com/ollama/ollama) 🟢 🏠 — Run LLMs locally.
- [LM Studio](https://lmstudio.ai/) 🆓 🏠 — Local LLM desktop UI.

## Model Context Protocol (MCP)

Anthropic's open standard for connecting AI tools to data sources and capabilities.

- [MCP Specification](https://modelcontextprotocol.io/) — The spec.
- [Official MCP servers](https://github.com/modelcontextprotocol/servers) 🟢 — Reference implementations (filesystem, git, GitHub, Slack, etc).
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) — Curated MCP server directory.
- [mcp-agent](https://github.com/lastmile-ai/mcp-agent) 🟢 — Build agents on top of MCP.
- [FastMCP](https://github.com/jlowin/fastmcp) 🟢 — Pythonic MCP server framework.

## DevOps & CI/CD

- [Animus](https://github.com/launchapp-dev/animus-cli) 🟢 — Daemon-driven AI workflows in CI.
- [Sweep](https://github.com/sweepai/sweep) 🟢 — AI assistant that opens PRs from issues.
- [SourceLevel](https://sourcelevel.io/) 💰 — AI metrics and review automation.

## Models for Coding

Frontier and open-weight models with strong code performance.

- **Closed:** [Claude Sonnet/Opus 4.x](https://www.anthropic.com/), [GPT-5 / o-series](https://openai.com/), [Gemini 2.5/3 Pro](https://ai.google.dev/)
- **Open weights:** [Qwen2.5-Coder](https://github.com/QwenLM/Qwen2.5-Coder), [DeepSeek-Coder-V3](https://github.com/deepseek-ai/DeepSeek-Coder), [Codestral](https://mistral.ai/news/codestral/), [StarCoder2](https://github.com/bigcode-project/starcoder2)

## Prompt & Context Engineering

- [Repomix](https://github.com/yamadashy/repomix) 🟢 — Pack a repo into a single file for LLM context.
- [files-to-prompt](https://github.com/simonw/files-to-prompt) 🟢 — CLI to bundle files into a prompt.
- [Cursor Rules](https://docs.cursor.com/context/rules) — Cursor's rules format (also adopted by other tools).
- [CLAUDE.md convention](https://docs.claude.com/en/docs/claude-code/memory) — Project-level instructions for Claude Code.

## Learning Resources

- [Anthropic's Building Effective Agents](https://www.anthropic.com/research/building-effective-agents) — Patterns for production agents.
- [SWE-bench](https://www.swebench.com/) — Benchmark for resolving real GitHub issues.
- [Aider Leaderboards](https://aider.chat/docs/leaderboards/) — Real-world coding benchmark by model.

## Related Lists

- [sourcegraph/awesome-code-ai](https://github.com/sourcegraph/awesome-code-ai) — Long-running list maintained by Sourcegraph.
- [jamesmurdza/awesome-ai-devtools](https://github.com/jamesmurdza/awesome-ai-devtools) — Developer-tool focused.
- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) — MCP servers specifically.
- [Hannibal046/Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM) — Broader LLM landscape.
- [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) — LLM application examples.

---

## Contributing

Found a tool we missed? Open a PR. See [contributing.md](contributing.md) for inclusion criteria — we prioritize tools that ship, are actively maintained, and serve real developer workflows.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [LaunchApp](https://github.com/launchapp-dev) has waived all copyright and related or neighboring rights to this work.
