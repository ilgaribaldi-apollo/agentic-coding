# Agentic Coding

## File Index

### Core
- [AGENTS.md](AGENTS.md): Repo root — agent entrypoint (this file)
- [README.md](README.md): Human-readable overview and usage guide
- [AGENTS.md](.agents/AGENTS.md): Knowledge base registry — patterns, agents, skills index

### Knowledge Base
- [AGENTS.md](.agents/patterns/AGENTS.md): Code patterns index (TS, Python, cross-platform)
- [_templates/](.agents/_templates): Templates for adding new patterns, agents, libraries
- [agents/](.agents/agents): Reusable sub-agent definitions (debugger, doctor, explorer, security, react-expert)
- [skills/](.agents/skills): Multi-step skill workflows (hyperscan, planning-with-files, agent-browser, vercel-react)
- [plans/](.agents/plans): Implementation plan tracking (active + archived)

## Purpose
Portable agentic coding knowledge base — patterns, conventions, sub-agents, and skills for AI-assisted development. Drop `.agents/` into any project for structured agent context.

## Workflow
1. Read this file for repo structure.
2. Read [.agents/AGENTS.md](.agents/AGENTS.md) for the full registry with technology lookup.
3. Load relevant `patterns/*.md` files for your task.
4. Use `agents/*.md` definitions for specialized sub-agent prompts.
5. Use `skills/*/SKILL.md` for multi-step workflows.

## Do / Don't

| Do | Don't |
|----|-------|
| Start here, then navigate to .agents/AGENTS.md | Skip the registry and guess file locations |
| Use relative paths (repo is portable) | Hardcode absolute paths to any specific machine |
| Add new content via _templates/ | Create content without a registry entry |
