---
name: flow-prompt-check
description: Checks an image or video prompt for Google Flow (Veo), Kling or another image-to-video tool before the user presses Generate, against seven causes that waste credits — videos made before the stills are checked, no reference image for a building that repeats, size words like "huge", two camera moves or no stop, an end state too far from the start, text inside the picture, and words that get refused — then rewrites only the sentences that fail. Use when someone pastes a Flow, Veo or Kling prompt and asks to check, fix or improve it, or says a clip failed (the building changed shape, the camera drifted, the scene jumped, people melted, extra things appeared, the water went wild, the tool refused).
---

# Flow prompt check

The user is about to spend credits on an image or a video clip. Your job is to find what will make it fail, and to change only those sentences. Answer in the user's language.

## 1. Get the material

You need:
- the prompt (one or several);
- whether it is a **still** (image) or a **video clip**, and for a clip, whether the tool takes a start image only or a start and an end image;
- if a clip already failed: what they saw, in one line.

If the prompt is there but the rest is not, guess from the prompt and say what you guessed. Ask only if you cannot guess.

## 2. Check the seven causes

Go through all seven, in this order. For each, quote the words in the prompt that caused your verdict.

| # | Cause | How to spot it | Fix |
|---|---|---|---|
| 1 | Videos made before all stills are checked | The user is about to make a video, and it is not clear that every cut's still exists and was checked | Suggest the order: make every still first, lay them side by side, check shape, era, number of people and stray letters together, then make the videos. A still fixed later means its video is made again. |
| 2 | A building, hill or ship that appears in many cuts has no reference image | The subject is a named place or structure, and the prompt neither says a reference image is attached nor repeats fixed shape words | One reference image built from 2–4 real photos, attached every time (first), plus a short "never changes" description pasted word for word into every prompt with that place. |
| 3 | Size written as "huge", "massive", "towering", "giant", "enormous", "colossal" (or 巨大な・そびえ立つ / 거대한・우뚝 솟은) | Any of these words, or a size with no unit | Count in people: "about as tall as seven adults stacked". These words make things far too big or put giants in the scene. |
| 4 | Two camera moves in one clip, or no way to stop | More than one move ("pan left then push in", "orbit and rise"), or a move with no ending | One move only, ending "decelerating hard in the last second and stopping on …". Add "fast" to the move — clips are often sped up in the editor, and slow moves become almost still. |
| 5 | The end state is too far from the start | One clip goes from one state to a very different one (another place, a building rising from nothing, many years of change) | Make the change smaller, or split it into two cuts. Otherwise the scene seems to jump halfway. |
| 6 | Words inside the picture | Quoted sign text, a title, captions, numbers or labels the user wants to see in the frame | Remove them. Add "No text, no letters, no numbers, no labels, no logos, no watermark." and "The upper fifth of the frame stays empty." Put the words in later with the editor. Generated letters come out wrong or as nonsense. |
| 7 | Words that tend to be refused | Injuries, blood, red-stained hands, children close to adults, real people's names, close-up faces | Remove them and describe the action plainly. People small or from behind. If it is refused again after one change, make that cut a locked shot of the place instead. |

## 3. If a clip already failed

Use the line the user gave you:

| What they saw | Change |
|---|---|
| The building changed shape | Make the still again with the reference image attached first; copy the "never changes" words exactly. |
| The camera barely moves | Say "fast" and add a near object to move past ("past the pine trunks"). |
| The camera moves twice or drifts at the end | One move only; end with "stopping dead on …". |
| People melt or multiply | Fewer people, smaller, from behind; one action each. |
| Something appears that should not (letters, a second sun, modern objects) | Add one plain sentence: "No signs, no lettering anywhere." / "Only one sun in the sky." / "No power lines, no cars." |
| The scene jumps to another place halfway | The end state was too far from the start (cause 5). |
| The tool refused | Cause 7. |
| The water goes wild (waves, spray) at a dock, lock or pond | "The water stays flat and calm, no waves, no spray", and show one scene only. |
| Music they did not ask for | "No background music. Only realistic location sound: {2–3 real sounds of the place}." |

## 4. Answer in this shape

1. **Table** — `# | cause | what in your prompt | OK / change`. Seven rows, plus one row for the failure they reported, if any.
2. **New prompt** — the whole prompt in one code block, with only the failing sentences changed. Every other word stays exactly as the user wrote it. If nothing fails, say so and do not rewrite.
3. **What changed** — one short line per change.
4. One sentence: pressing Generate again with the same words costs credits and gives the same mistake.

## Do not

- Do not invent prices, limits or features of the tool. If the user asks, tell them to check the tool's own page.
- Do not promise that the clip will work. Say which causes are now removed.
- Do not add style words, extra details or a new camera move that the user did not ask for.
