# Agentic Coding

A portable knowledge base for AI-assisted software development. Drop it into any project to give your AI coding agent structured context — code patterns, reusable sub-agents, multi-step skills, and implementation plan tracking.

## What's Inside

```
.agents/
├── patterns/        # 15 code pattern docs across TS, Python, and cross-platform
├── agents/          # 5 sub-agent definitions for specialized tasks
├── skills/          # 4 multi-step skill workflows
├── skills/planning-with-files/plans/  # Implementation plans
├── templates/       # Templates for adding new content
└── AGENTS.md        # Master index with technology lookup table
```

### Patterns

Ready-to-use conventions for modern stacks. Each pattern doc includes stack choices, code examples, naming conventions, and anti-patterns.

| Domain | Patterns |
|--------|----------|
| **TypeScript / Frontend** | Next.js 15 App Router, Hono API routes, Drizzle ORM, TanStack Query v5, React 19 components, Shadcn/UI + Tailwind, Turborepo monorepos, Clerk auth |
| **Python / Backend** | Flask, psycopg2, SQLAlchemy, uv, deployment, CLI patterns, retry logic, parallel processing |
| **Data Science** | xarray/Zarr, NumPy, joblib, temporal operations |
| **Cross-Platform** | Expo SDK 55, React Native, Electron 35 |
| **Reference** | 40+ official documentation links by category |

### Agents

Sub-agent definitions that can be used as system prompts for specialized tasks:

| Agent | Purpose |
|-------|---------|
| **Debugger** | Bug investigation, root cause analysis, fix verification |
| **Doctor** | Audit documentation against actual codebase |
| **Explorer** | Codebase search, architecture understanding |
| **Security Audit** | OWASP Top 10 vulnerability assessment |
| **React Expert** | React/Next.js performance optimization (57 Vercel rules) |

### Skills

Multi-step workflows with templates and reference material:

| Skill | Purpose |
|-------|---------|
| **Hyperscan** | Deep codebase scan that produces a compact context map for implementation |
| **Planning with Files** | Manus-style file-based task planning with session recovery |
| **Vercel React Best Practices** | 57 performance rules with BAD/GOOD code examples |
| **Agent Browser** | Browser automation for testing, form filling, screenshots, and data extraction |

## Usage

### With Claude Code

Clone or copy `.agents/` into your project root. Point your `CLAUDE.md` at it:

```markdown
## Knowledge Base
Read `AGENTS.md` for the full structure. Start with `.agents/AGENTS.md` to find relevant patterns.
```

### With Other AI Coding Tools

The pattern docs, agent definitions, and skill workflows are plain Markdown — they work with any AI tool that accepts context files. Load the relevant `patterns/*.md` files as context for your task.

## Adding Content

Templates make it easy to add new patterns, libraries, or agents:

```bash
# New pattern
cp .agents/templates/pattern.md .agents/patterns/my-pattern.md

# New library reference
cp .agents/templates/library.md .agents/patterns/my-library.md

# New agent
cp .agents/templates/agent.md .agents/agents/my-agent.md
```

After filling in the template, add an entry to `.agents/AGENTS.md`.

## Plans

Track implementation plans across sessions:

```
.agents/skills/planning-with-files/plans/{plan-slug}/    # task_plan.md, findings.md, progress.md
```

## License

MIT
# agentic-coding
