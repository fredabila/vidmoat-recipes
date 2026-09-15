# Vidmoat recipes

Copy-paste prompts for [Vidmoat](https://www.vidmoat.com) — a **hosted AI video editor** with a real, reviewable timeline.

Start in the browser at [vidmoat.com](https://www.vidmoat.com), or text a clip to [@vidmoat_bot](https://t.me/vidmoat_bot) on Telegram. Same product, same projects, same credits. MCP is **one client** (Claude Code, Cursor, etc.) that can drive that same timeline — not the product itself.

This is **not** "the only MCP video editor." Palmier Pro already drives a real local Mac timeline. OpusClip already ships a hosted clipper MCP. Rendley sells MCP editing. Vidmoat's lane is **hosted + cross-platform + reviewable timeline + chat**.

## Ways in (hosted first)

1. **Browser editor** — https://www.vidmoat.com  
2. **Telegram** — [@vidmoat_bot](https://t.me/vidmoat_bot) (underscore only; `@VidmoatBot` is not us)  
3. **MCP** (optional) — same timeline, Studio for live/production; test keys on any plan  

```bash
claude mcp add --transport http vidmoat api.vidmoat.com/api/mcp
```

Then paste an API key from Account → API keys.

- **Test keys** work on any plan, including Hobby ($0).
- **Live / production MCP** is Studio ($49/mo). Creator ($19/mo) does not include live MCP.
- Manual edits do not spend credits.
- Do **not** print Hobby credit numbers here — use `/pricing` as source of truth.

Cursor: add the same URL (`https://api.vidmoat.com/api/mcp`) as a Streamable HTTP server, Authorization `Bearer vmk_…`.

Full client configs: [CONNECT.md](./CONNECT.md). Product docs: [developer.vidmoat.com](https://developer.vidmoat.com).

## Recipes

| File | Job |
|---|---|
| [podcast-to-shorts](./recipes/podcast-to-shorts.md) | Long episode → 8–12 verticals with karaoke captions |
| [silence-and-filler](./recipes/silence-and-filler.md) | Cut dead air and ums, keep comic timing |
| [karaoke-captions](./recipes/karaoke-captions.md) | Word-level captions, brand style |
| [reframe-vertical](./recipes/reframe-vertical.md) | 16:9 → 9:16, speaker stays in frame |
| [one-click-shorts](./recipes/one-click-shorts.md) | One long cut → a pack of hooks |
| [recipe-reel](./recipes/recipe-reel.md) | Phone cook → 60s banger |
| [green-screen-coach](./recipes/green-screen-coach.md) | Key + logo brush + four platforms |
| [product-demo](./recipes/product-demo.md) | Screen + talk track → changelog video |
| [check-frames-then-render](./recipes/check-frames-then-render.md) | Preview frames as images, then export |
| [telegram-chat-edit](./recipes/telegram-chat-edit.md) | Send a clip in Telegram, get a real edit back |
| [captions-without-nle](./recipes/captions-without-nle.md) | Burned-in karaoke captions without opening Premiere |

Every recipe ends with: **preview frames, then render.** An agent that cannot see the frame will put text on a face. The editor exposes **65+ timeline commands** — say that; do not print an MCP tool count (public pages disagree).

## Copy freeze

When you fork or quote this repo:

- Lead with the **hosted editor** (vidmoat.com), then Telegram `@vidmoat_bot`, then MCP as optional.
- Say **65+ timeline commands**. Do not print an MCP tool count.
- Do not print Hobby credit numbers until `/pricing` and the docs agree.
- Do not say "only MCP video editor."
- Never write `@VidmoatBot` (no underscore) — that is a different account.
- Discord is a small room, not a community.
- [Agent2Creator](https://agent2creator.vidmoat.com) is a gallery of Vidmoat renders, not a second product.

## License

MIT. Prompts are yours to reuse. Footage you send to Vidmoat stays in your account.
