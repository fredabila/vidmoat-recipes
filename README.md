# Vidmoat recipes

Copy-paste prompts and MCP setup for [Vidmoat](https://vidmoat.com), a hosted video editor an agent can see and a human can still open.

This is **not** "the only MCP video editor." Palmier Pro already drives a real local Mac timeline. OpusClip already ships a hosted clipper MCP. Rendley sells MCP editing. Vidmoat's lane is **hosted + cross-platform + reviewable timeline + chat** (`@VidmoatBot` on Telegram).

## Connect

```bash
claude mcp add --transport http vidmoat api.vidmoat.com/api/mcp
```

Then paste an API key from Account → API keys.

- **Test keys** work on any plan, including Hobby ($0).
- **Live / production MCP** is Studio ($49/mo). Creator ($19/mo) does not include live MCP.
- Manual edits do not spend credits.

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

Every recipe ends with: **preview frames, then render.** An agent that cannot see the frame will put text on a face.

## Copy freeze

When you fork or quote this repo:

- Say **65+ timeline commands**. Do not print an MCP tool count (public pages disagree).
- Do not print Hobby credit numbers until `/pricing` and the docs agree.
- Do not say "only MCP video editor."
- Discord is a small room, not a community.
- [Agent2Creator](https://agent2creator.vidmoat.com) is a gallery of Vidmoat renders, not a second product.

## License

MIT. Prompts are yours to reuse. Footage you send to Vidmoat stays in your account.
