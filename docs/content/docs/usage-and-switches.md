# Usage & Configuration

Running `npx create-claude-context` will launch a sleek interactive CLI powered by `@clack/prompts`. 

## Interactive Prompts
1. **Project Name**: This will create a local directory by this name and inject the templates into it.
2. **Framework/Environment**: You can select standard setups (React, Vue, Node.js, Python, Other). This directly shapes the baseline `CLAUDE.md` context.
3. **Scaffolding Complexity**: The depth of context you want (see [Scaffolding Tiers]({{< relref "docs/scaffolding-tiers" >}}) for details).
4. **General Guidelines**: An option to generate an extra `.claudeprompt` file containing universal AI interaction rules.

## CLI Flags & Switches

*(Currently, all options are exposed via the interactive menus for the best developer experience. Advanced command-line flag parsing for CI/CD usage may be implemented in future phases.)*
