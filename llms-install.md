# AlgoRover Research for Cline

AlgoRover Research is a hosted MCP service for strategy discovery and historical backtests. It does not connect exchange accounts or place orders.

1. In Cline CLI, run `cline mcp add algorover-research https://research.algorover.ai/mcp --transport http --yes`. Respect any explicitly supplied Cline configuration and data directory flags. In the Cline editor extension, open MCP Servers settings and add a remote Streamable HTTP server named `algorover-research` with URL `https://research.algorover.ai/mcp`. Merge the entry in `cline_mcp_settings.example.json` into the existing configuration, preserving other servers.
2. Public strategy search and details do not require Research sign-in. Cline authorization and authenticated backtests are still under validation. For personal operations, use Cline's authorization action when available and complete Research sign-in in the browser with `research:read` and `research:run`. Never paste access tokens, passwords or exchange credentials into chat or this configuration.
3. Verify that `search_strategies` is available. Ask Cline to search strategies using `locale: "en"` or `locale: "zh-CN"`.
4. Read a strategy's available presets and prepare a 90-day historical backtest. Show the returned preview and obtain confirmation before starting the job.
5. Read the job until it reaches its actual terminal state, then obtain its result and report link. For cancellation, cancel only the selected active job and check the final status.

Use actual tool text and returned links when the client does not render an inline card. Reconnect through Cline if authorization expires.

Support: https://www.algorover.ai/en/help/
Privacy: https://www.algorover.ai/privacy/
Terms: https://www.algorover.ai/terms/
