# AlgoRover Research for Cline

Connect Cline to AlgoRover Research to discover published strategies and inspect their details using public market research data. This repository contains Cline installation instructions for the hosted MCP service at `https://research.algorover.ai/mcp`.

## Install

With Cline CLI installed, run:

```bash
cline mcp add algorover-research https://research.algorover.ai/mcp --transport http --yes
```

For the Cline editor extension, open MCP Servers settings and merge the entry from [cline_mcp_settings.example.json](cline_mcp_settings.example.json) into your configuration, preserving other servers. The transport is Streamable HTTP.

Ask Cline: "Use AlgoRover Research to search for one strategy, then read that exact strategy's details."

See [llms-install.md](llms-install.md) for agent installation and validation instructions.

## Capabilities and validation

Public strategy search and detail retrieval have been verified through Cline CLI using a connected ChatGPT subscription. The service also exposes backtest preparation and account-protected historical backtests, tasks and reports. Cline browser authorization and the complete authenticated backtest workflow are still under validation; these capabilities must not be described as verified in Cline.

Personal operations require Research authorization with `research:read` and `research:run`. Use the client's browser authorization flow when available. Never paste credentials into chat or configuration. Show a returned backtest preview and obtain confirmation before starting a job. Historical results do not establish future returns. The service does not connect exchange accounts or place orders.

## Publisher and support

Published by Rivendell Holdings Investment Limited.

- [Website](https://www.algorover.ai/)
- [Support](https://www.algorover.ai/en/help/)
- [Privacy](https://www.algorover.ai/privacy/)
- [Terms](https://www.algorover.ai/terms/)
