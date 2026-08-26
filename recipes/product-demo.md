# Product demo

**Job:** screen recording + voice → a changelog clip an agent can ship.

```
This project is a product demo. There is a screen recording and a voiceover.

1. Transcribe. Cut silences over 0.5s in the voice track.
2. Auto-duck any music under speech.
3. Zoom/crop the screen to the UI being mentioned, on the sentence that mentions it.
4. Add a lower-third with the product name only where a new surface appears.
5. Captions: karaoke, small, not covering the UI.
6. Preview frames of every zoom as images. If a zoom crops a button the voice names, undo that zoom.
7. Render 1920x1080 and a 9:16 cut of the same story.
```

MCP-native version:

```
Import these files, create a 1920x1080 30fps project, lay the screen on V1 and VO on A1, then do the steps above. Preview frames as images before render.
```
