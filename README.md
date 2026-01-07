# Holis Claude Tool

Development skills and tools for solving Asana issues and streamlining development workflows.

## Skills Included

### solve-asana-issue
Comprehensive workflow for solving issues from Asana. Use when you're asked to solve an issue with an Asana link.

**Capabilities:**
- Reads and analyzes Asana issues
- Investigates root cause using any available tools
- Creates fix PRs with proper testing when needed
- Follows iCHEF's PR conventions (target: develop branch)

## Installation

### Step 1: Add Marketplace

```shell
/plugin marketplace add iCHEF/holis-claude-tool
```

### Step 2: Install Plugin

```shell
/plugin install holis-claude-tool@iCHEF_holis_claude_tool
```

### Alternative: Auto-Install for Teams

Add this to your project's `.claude/settings.json` for automatic installation:

```json
{
  "extraKnownMarketplaces": {
    "holis-tools": {
      "source": {
        "source": "github",
        "repo": "iCHEF/holis-claude-tool"
      }
    }
  },
  "enabledPlugins": {
    "holis-claude-tool@holis-tools": true
  }
}
```

Team members will be prompted to install automatically when working on the project.

### Verify Installation

Ask Claude:

```
What Skills are available?
```

You should see `solve-asana-issue` in the list.

## Usage

Skills activate automatically when relevant. For example:

```
"Please solve this Asana issue: https://app.asana.com/0/..."
```

Claude will automatically use the `solve-asana-issue` skill to:
1. Read the issue from Asana
2. Investigate the root cause
3. Create a fix PR if needed (with tests)
4. Follow iCHEF PR conventions

## Update

To get the latest version:

```shell
/plugin update holis-claude-tool
```

## Version History

See [CHANGELOG.md](CHANGELOG.md)

## Requirements

- Claude Code CLI
- Asana MCP server configured (for reading Asana issues)

## License

MIT
