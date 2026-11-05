# work-access-tools

Hosted MCP tools for agents:

- `categorize_products` — verified product categorization (model consensus)
- `package_exists` — npm / PyPI existence + latest version
- `lock_acquire` / `lock_release` — short-lived distributed locks

**MCP endpoint (streamable HTTP):** https://work-access-platform.bfurrow26.workers.dev/mcp

**Free tier:** 50 MCP calls/day per key (no signup). REST signup gives 100 free categorize items.

```bash
# tools/list
curl -s -X POST https://work-access-platform.bfurrow26.workers.dev/mcp \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/list","params":{}}'
```

- Landing: https://work-access-platform.bfurrow26.workers.dev/
- Try: https://work-access-platform.bfurrow26.workers.dev/try
- llms.txt: https://work-access-platform.bfurrow26.workers.dev/llms.txt
- Official MCP Registry: `io.github.throttler300/work-access-platform`
- Support: dirtsmith@mail.grokbot.com

Source implementation remains private; this repo is the public listing + install pointer.
