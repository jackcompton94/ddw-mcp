# ddw-mcp

A Model Context Protocol (MCP) server for querying data.world NFL statistics and saving insights.

## Features

- Execute SQL queries against 2023 NFL dataset
- Save markdown reports as insights on data.world
- Runs as an MCP server via stdio transport

## Available Tables

- `all_qb_stats`: QB game statistics including passing and rushing data
- `all_team_stats`: Team game statistics including offense and defense metrics

## Installation

```bash
npm install
npm run build
```

## Usage with Claude CLI

After building the project, register the MCP server with Claude CLI:

```bash
claude mcp add ddw-mcp -- env DW_AUTH_TOKEN=<your-token-here> node ddw-mcp/build/index.js
```

## Development

```bash
# Build the project
npm run build
```

## License

ISC