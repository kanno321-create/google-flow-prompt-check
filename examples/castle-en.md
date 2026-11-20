# Himeji Castle — a video clip prompt (English)

A real run in Claude Code on 20 November 2026, copied without edits.

## What the user typed

> I'm about to generate this clip in Google Flow (Frames to Video, start frame only). Last time the castle came out as a different castle. Can you check it before I press generate?
>
> A cinematic 8-second shot of the massive Himeji Castle towering over the town at sunset. The camera orbits around the keep and then rises up into the sky, as the castle is built from an empty hill to the finished keep. A wooden sign at the gate reads "Himeji Castle 1609". A samurai with a bleeding arm looks straight into the camera.

## What the skill answered

I checked your prompt as a **video clip from a start frame only**, and your report that **the castle came out as a different castle**. Five of the seven causes apply.

| # | Cause | What in your prompt | OK / change |
|---|---|---|---|
| 1 | Videos made before stills are checked | It's not clear the start frame was checked against the real castle | **Change.** Make and check the start frame first (shape, era, number of people, stray letters), then make the video |
| 2 | Named building with no reference image | "Himeji Castle" with no reference image and no fixed shape words | **Change.** Make one reference image from 2–4 real photos and attach it first. Paste the "never changes" line below into every Himeji prompt, word for word |
| 3 | Size words | "massive", "towering" | **Change.** Give the height in people instead |
| 4 | Two camera moves or no stop | "orbits around the keep **and then rises up** into the sky" | **Change.** Use one move, make it fast, and give it a hard stop |
| 5 | End state too far from the start | "built from an empty hill to the finished keep" | **Change.** This is a separate cut. In one clip the scene will seem to jump halfway |
| 6 | Words in the picture | Sign reading "Himeji Castle 1609" | **Change.** Remove it and add the title in the editor |
| 7 | Words that tend to be refused | "bleeding arm", "looks straight into the camera" (close-up face) | **Change.** Make the samurai small and seen from behind, with no injury |
| — | Your failure: the castle changed shape | No reference image and no fixed shape words | **Change.** Make the start frame again with the reference attached first, using the exact "never changes" words |

**New prompt**

```
A cinematic 8-second shot of Himeji Castle over the town at sunset. Never changes: white plastered walls, a main keep with five roof layers of grey tiles and stacked triangular and curved gables, standing on a tall curved grey stone base; the keep is about as tall as eighteen adults stacked, the stone base about as tall as nine adults stacked. The camera orbits fast around the keep, decelerating hard in the last second and stopping on the front face of the keep. A small samurai stands at the gate, seen from behind. No text, no letters, no numbers, no labels, no logos, no watermark. The upper fifth of the frame stays empty.
```

**What changed**
- Removed "massive" and "towering", and gave the height in people.
- Added the "never changes" shape line. Attach the reference image first, then make the start frame again with it.
- Kept only the orbit. It's now "fast" and ends with a hard stop. The "rises up into the sky" move is gone.
- Took out the construction from an empty hill. If you want it, make it its own cut (for example, the hill with scaffolding going to a half-built keep).
- Took out the "Himeji Castle 1609" sign. Add that title in the editor instead; the empty upper fifth leaves room for it.
- Replaced the bleeding samurai looking into the camera with a small samurai seen from behind at the gate.

These changes remove all five causes. That doesn't guarantee the clip will come out right. Pressing Generate again with the same words would cost credits and most likely give you the same wrong castle.
