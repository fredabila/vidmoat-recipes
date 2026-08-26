# Check frames, then render

**Job:** the step most MCP demos skip. Use after any other recipe.

```
Do not render yet.

1. List the timeline: clips, caption tracks, duration, aspect.
2. Preview frames as images at 0:01, 0:05, 25%, 50%, 75%, and the last 1 second.
3. For each frame: is anything off-canvas, unreadable, covering a face, or the wrong aspect?
4. Fix those. Preview the same timestamps again as images.
5. Only then render 1080p and return the URL.

If a preview looks wrong and you cannot tell why, stop and describe it. Do not guess a render.
```

Why this exists: agents that only see timestamps will put karaoke on a mouth. Vidmoat returns frame previews as images on purpose. Use them.
