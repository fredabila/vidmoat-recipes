# Connect Vidmoat MCP

Endpoint: `https://api.vidmoat.com/api/mcp`  
Transport: Streamable HTTP  
Keys: Account → API keys (`vmk_test_…` or `vmk_live_…`)

Test keys: any plan, including Hobby. Live keys: **Studio**.

## Claude Code

```bash
claude mcp add --transport http vidmoat api.vidmoat.com/api/mcp
```

When prompted, add header `Authorization: Bearer YOUR_KEY`.

## Claude Desktop

`claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "vidmoat": {
      "url": "https://api.vidmoat.com/api/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_VIDMOAT_API_KEY"
      }
    }
  }
}
```

## Cursor

Settings → MCP → add a Streamable HTTP server:

- Name: `vidmoat`
- URL: `https://api.vidmoat.com/api/mcp`
- Header: `Authorization` = `Bearer YOUR_VIDMOAT_API_KEY`

## Smoke test

Ask the agent:

> List my Vidmoat projects. Then tell me which plan this key is on, and whether it is a test key or a live key.

If that returns projects, you are connected. If it asks you to upgrade, you are on a test key trying a live-only call. Stay on test until you actually need to render for real, then use Studio.

## After every edit

> Preview the current timeline as images at 0:03, 0:12, and the last 2 seconds. Fix any caption covering a face or sitting off-canvas. Then render 1080p and give me the URL.
