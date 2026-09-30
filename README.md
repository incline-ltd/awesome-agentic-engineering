# Awesome AI Coding Agent Engineering [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

An opinionated, reviewed guide to building reliable AI coding agents. It
focuses on repository rules, coding workflows, tool connections, verification,
and safe execution instead of trying to list every AI agent resource.

**Last reviewed:** July 18, 2026. The list is reviewed monthly and when a linked
project changes in a way that affects its recommendation.

## Contents

- [Start Here](#start-here)
- [How This List Is Curated](#how-this-list-is-curated)
- [Coding Agents](#coding-agents)
- [Agent Rules And Memories](#agent-rules-and-memories)
- [Claude Code](#claude-code)
- [Codex](#codex)
- [Cursor](#cursor)
- [MCP Servers](#mcp-servers)
- [Skills And Plugins](#skills-and-plugins)
- [Code Review Workflows](#code-review-workflows)
- [Testing And Verification](#testing-and-verification)
- [Security And Sandboxing](#security-and-sandboxing)
- [Prompt Patterns](#prompt-patterns)
- [Case Studies](#case-studies)
- [Learning Resources](#learning-resources)
- [Related Public Projects](#related-public-projects)

## Start Here

Use these six topics as a practical path from agent setup to safe execution
and verification:

**Project instructions.** Give the agent clear repository rules and durable context.

**Coding workflow.** Learn a repository-aware working loop from an agent provider.

**Permission boundaries.** Understand sandboxing, approvals, and command execution.

**Tool connections.** Expose tools and context through MCP, then inspect them.

**Verification.** Test the changed system instead of trusting generated code.

**Security.** Check secrets, dependencies, and execution risk before release.

## How This List Is Curated

- A resource must help build, configure, test, secure, or operate an AI coding
  agent.
- Official documentation, canonical repositories, and actively maintained
  projects are preferred.
- Every description must explain a concrete engineering use.
- Generic AI directories, marketing-only pages, duplicate resources, and stale
  projects are left out.

The goal is a smaller list that helps an engineer make a decision, not a large
collection of links.


## Coding Agents

- [Aider](https://aider.chat/) - Pairs with language models in the terminal for repository-aware code edits and commits.
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) - Runs agentic coding workflows from a terminal with project context and tool use.
- [Cline](https://github.com/cline/cline) - Provides an open-source coding agent that can edit files, run commands, and use browser automation.
- [Codex](https://github.com/openai/codex) - Provides an open-source coding agent that runs locally in the terminal.
- [Continue](https://www.continue.dev/) - Adds open-source AI coding assistance and custom workflows to IDEs.
- [GitHub Copilot Coding Agent](https://docs.github.com/en/copilot/concepts/coding-agent/coding-agent) - Creates pull requests from GitHub issues using Copilot's asynchronous coding agent.
- [OpenCode](https://opencode.ai/) - Offers a terminal coding agent with pluggable model providers and project-aware workflows.

## Agent Rules And Memories

- [AGENTS.md](https://agents.md/) - Defines a simple project instruction file for coding agents.
- [Claude Code Memory](https://docs.anthropic.com/en/docs/claude-code/memory) - Shows how Claude Code loads project, user, and local memory files.
- [Coding Agent Guidelines](https://github.com/incline-ltd/coding-agent-guidelines) - Packages portable behavioral rules for Claude Code, Cursor, and AGENTS.md consumers.
- [Cursor Rules](https://docs.cursor.com/context/rules) - Describes reusable project rules that guide Cursor agents and chat.

## Claude Code

- [Claude Code Best Practices](https://www.anthropic.com/engineering/claude-code-best-practices) - Collects Anthropic engineering guidance for effective Claude Code workflows.
- [Claude Code GitHub Actions](https://docs.anthropic.com/en/docs/claude-code/github-actions) - Runs Claude Code from GitHub Actions for issue and pull-request work.
- [Claude Code Hooks](https://docs.anthropic.com/en/docs/claude-code/hooks) - Uses shell hooks to enforce checks and customize tool behavior.
- [Claude Code Plugins](https://docs.anthropic.com/en/docs/claude-code/plugins) - Packages slash commands, agents, hooks, and MCP servers for reuse.
- [Claude Code SDK](https://docs.anthropic.com/en/docs/claude-code/sdk) - Embeds Claude Code workflows into custom automation.

## Codex

- [Codex AGENTS.md](https://developers.openai.com/codex/guides/agents-md) - Shows how repository instructions are discovered and merged.
- [Codex Configuration](https://developers.openai.com/codex/config-basic) - Documents provider, sandboxing, MCP, and runtime configuration.
- [Codex MCP](https://developers.openai.com/codex/mcp) - Connects Codex to external tools and data through Model Context Protocol.
- [codex-profiles](https://github.com/Ducksss/codex-profiles) - Provides a community tool for named CODEX_HOME folders and separate local ChatGPT app data on macOS without copying tokens.
- [Codex Sandbox](https://developers.openai.com/codex/concepts/sandboxing) - Explains local sandboxing, approvals, and command execution controls.
- [Codex Security](https://developers.openai.com/codex/security) - Describes security controls and threat-model guidance for Codex.

## Cursor

- [Cursor Background Agents](https://docs.cursor.com/agent/background-agent) - Explains asynchronous agents that can work on remote development environments.
- [Cursor CLI](https://docs.cursor.com/cli/overview) - Runs Cursor agent workflows and editor commands from a terminal.
- [Cursor Documentation](https://docs.cursor.com/) - Covers editor setup, agents, rules, and model configuration.
- [Cursor MCP](https://docs.cursor.com/context/mcp) - Connects external tools and data sources to Cursor through MCP.
- [Cursor Memories](https://docs.cursor.com/context/memories) - Stores reusable user and project context for future agent sessions.

## MCP Servers

- [FastMCP](https://github.com/jlowin/fastmcp) - Provides a Python framework for building MCP servers and clients.
- [MCP Inspector](https://github.com/modelcontextprotocol/inspector) - Debugs MCP servers through an interactive developer tool.
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) - Implements the protocol for Python MCP servers and clients.
- [MCP Servers Repository](https://github.com/modelcontextprotocol/servers) - Lists reference and community MCP server implementations.
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) - Implements the protocol for TypeScript MCP servers and clients.
- [Model Context Protocol](https://modelcontextprotocol.io/) - Defines the open protocol for connecting agents to tools and context.

## Skills And Plugins

- [Claude Code Skills](https://docs.anthropic.com/en/docs/claude-code/skills) - Bundles task-specific instructions, scripts, and resources for Claude Code.
- [Continue Hub](https://hub.continue.dev/) - Shares assistants, rules, MCP servers, and reusable development context.
- [OpenAI Apps SDK](https://developers.openai.com/apps-sdk/) - Builds ChatGPT apps that expose structured tools and interactive components.
- [OpenAI Agents SDK](https://openai.github.io/openai-agents-python/) - Provides Python primitives for agents, handoffs, tools, guardrails, and tracing.
- [Smithery](https://smithery.ai/) - Indexes MCP servers for discovery, installation, and evaluation.

## Code Review Workflows

- [CodeRabbit](https://www.coderabbit.ai/) - Reviews pull requests with AI-assisted summaries and inline suggestions.
- [Danger JS](https://danger.systems/js/) - Automates pull-request checks and review comments from JavaScript or TypeScript.
- [GitHub Pull Request Reviews](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests) - Documents review states, comments, and requested changes on GitHub.
- [Reviewdog](https://github.com/reviewdog/reviewdog) - Reports linter and analyzer findings directly on pull requests.
- [Sourcegraph Cody](https://sourcegraph.com/cody) - Helps developers understand, edit, and review code with sourcegraph-aware context.

## Testing And Verification

- [Agent QA](https://github.com/vostride/agent-qa) - Runs natural-language web and mobile regression tests with persistent memory through CLI and MCP interfaces.
- [agenttrace](https://github.com/luoyuctl/agenttrace) - Analyzes local AI coding agent sessions for estimated cost, token use, elapsed time, and slow run details. Maintained by [@luoyuctl](https://github.com/luoyuctl).
- [Jest](https://jestjs.io/) - Runs JavaScript tests with snapshots, mocks, and watch mode.
- [Mneme](https://github.com/MnemeHQ/mneme) - Checks proposed code changes against declared architectural rules through agent integrations and CI. Maintained by [@TheoV823](https://github.com/TheoV823).
- [OpenAI Evals](https://github.com/openai/evals) - Provides a framework for measuring model behavior and task performance.
- [Playwright](https://playwright.dev/) - Automates browser testing across Chromium, Firefox, and WebKit.
- [pytest](https://docs.pytest.org/en/stable/) - Runs Python tests with fixtures, parametrization, and plugin support.
- [SWE-bench](https://www.swebench.com/) - Benchmarks coding agents on real-world software engineering tasks.
- [Vitest](https://vitest.dev/) - Provides a fast Vite-native test runner for JavaScript and TypeScript projects.

## Security And Sandboxing

- [Gitleaks](https://github.com/gitleaks/gitleaks) - Detects secrets and credentials in Git repositories and files.
- [GitHub Secret Scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning) - Detects committed secrets and supported token patterns in repositories.
- [OpenSSF Scorecard](https://github.com/ossf/scorecard) - Checks projects for common open-source supply-chain security risks.
- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/) - Summarizes common security risks in LLM-powered systems.
- [Semgrep](https://semgrep.dev/) - Finds security and correctness issues with customizable static-analysis rules.
- [Socket](https://socket.dev/) - Detects supply-chain risk in open-source dependencies.

## Prompt Patterns

- [Anthropic Prompt Engineering](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) - Explains prompt structure, examples, and evaluation for Claude workflows.
- [DSPy](https://dspy.ai/) - Builds and optimizes declarative language-model programs.
- [OpenAI Prompt Engineering](https://developers.openai.com/api/docs/guides/prompt-engineering) - Covers instructions, examples, context, and evaluation for OpenAI models.
- [Prompting Guide](https://www.promptingguide.ai/) - Organizes public prompt engineering techniques and examples.
- [TextGrad](https://github.com/zou-group/textgrad) - Optimizes natural-language prompts and model pipelines through textual gradients.

## Case Studies

- [Anthropic Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) - Explains agent patterns, workflow design, and when simple systems are enough.
- [Anthropic Multi-Agent Research System](https://www.anthropic.com/engineering/built-multi-agent-research-system) - Describes architecture and evaluation lessons from Anthropic's research agents.
- [Cursor Tab Model](https://cursor.com/blog/tab-update) - Explains product and model choices behind Cursor's code completion workflow.
- [GitHub Copilot Coding Agent](https://github.blog/news-insights/product-news/github-copilot-meet-the-new-coding-agent/) - Explains GitHub's approach to delegated coding tasks and pull-request workflows.
- [SWE-bench Verified](https://openai.com/index/introducing-swe-bench-verified/) - Introduces a curated benchmark for evaluating agentic software engineering.

## Learning Resources

- [AI Engineering](https://www.oreilly.com/library/view/ai-engineering/9781098166298/) - Teaches production practices for building applications with foundation models.
- [Hugging Face Agents Course](https://huggingface.co/learn/agents-course/) - Teaches agent concepts, tools, memory, and evaluation with hands-on examples.
- [Model Context Protocol Specification](https://modelcontextprotocol.io/specification) - Documents MCP protocol concepts for tools, resources, prompts, and transports.
- [OpenAI Agents Guide](https://developers.openai.com/api/docs/guides/agents) - Covers OpenAI agent design, tool use, guardrails, and orchestration.
- [The Twelve-Factor Agent](https://github.com/humanlayer/12-factor-agents) - Adapts durable software engineering principles to LLM-powered agents.

## Related Public Projects

- [Coding Agent Guidelines](https://github.com/incline-ltd/coding-agent-guidelines#readme) - Reusable rules for coding agents working in real repositories.
- [Production Launch Prompts](https://github.com/incline-ltd/production-launch-prompts) - Review prompts and scorecards for checking software before launch.

## Contributing

Contributions should add high-signal public resources with a clear engineering
use case. See [CONTRIBUTING.md](CONTRIBUTING.md) for quality, safety, and review
rules.
