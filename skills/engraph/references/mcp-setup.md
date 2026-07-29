# Engraph MCP Server Setup

## Install

```bash
brew install devferrazzz/tap/engraph  # local tap; see README for setup
engraph index /path/to/documents
```

## Configure MCP Client

**Claude Code** (`~/.claude/settings.json`):

```json
{
  "mcpServers": {
    "engraph": { "command": "engraph", "args": ["serve"] }
  }
}
```

**Claude Desktop** (`~/Library/Application Support/Claude/claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "engraph": { "command": "engraph", "args": ["serve"] }
  }
}
```

## HTTP Mode

```bash
engraph serve --http              # Port 3000
```
