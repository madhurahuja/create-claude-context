# Scaffolding Tiers

The core power of `create-claude-context` lies in its ability to output robust structures spanning from solitary context files to full-blown agent workspaces.

### 1. Basic
The simplest option. It only generates `CLAUDE.md` and optionally an interaction guideline `.claudeprompt` file.

### 2. Minimal Starter Set
A well-rounded baseline for small teams.
**Injects:**
- `CLAUDE.md`
- `README.md`
- `CONTEXT/`
- `PROMPTS/`
- `ARCHITECTURE.md` (inside CONTEXT)

### 3. Production-Grade
Designed to give Claude strict enterprise rules.
**Injects everything in Minimal, plus:**
- `SYSTEM_PROMPT.md`
- `GUARDRAILS.md`
- `DECISIONS.md`
- `FAQ.md`
- `TOOLS.md`
- `AGENTS.md`
- `GLOSSARY.md`

### 4. Portfolio AI
Specifically designed to create an AI that represents your personal dev portfolio.
**Injects everything in Production-Grade, plus:**
- `PROFILE_CONTEXT.md`
- `VISITOR_INTENT_MAP.md`
- `RESPONSE_POLICIES.md`

### 5. Claude Code Workspace
Built specifically for Anthropic's new official `claude` CLI standard.
**Injects:**
- A robust `.claude/settings.json` file configuring proper `PreToolUse` and `PostToolUse` hooks mapping to linting operations.
- `.claude/commands/review.md` and `test-all.md`
- `.claude/skills/code-review/SKILL.md`
- An `.mcp.json` proxy config to connect local Model Context Protocol tools to Github and Postgres natively.
- Evaluated subagent topologies in `agents/code-reviewer.yml`.
