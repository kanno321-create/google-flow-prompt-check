# Google Flow prompt check — a free Claude Code skill

[日本語](README.ja.md) · **English** · [한국어](README.ko.md)

Paste a Google Flow (Veo) or Kling prompt into Claude Code before you press **Generate**.
The skill checks it against the seven things that wasted our credits most often, and rewrites only the sentences that fail. Everything else stays word for word.

We make history and architecture Shorts with Google Flow and Kling. These seven come from the cuts we threw away.

## What it checks

| # | Cause | What the skill changes |
|---|---|---|
| 1 | Making videos before all the stills are checked | Suggests the order: every still first, check them side by side, then the videos |
| 2 | A building that appears in many cuts has no reference image | One reference image from 2–4 real photos, plus "never changes" words pasted into every prompt |
| 3 | Size written as "huge", "massive", "towering" | Counted in people: "about as tall as seven adults stacked" |
| 4 | Two camera moves in one clip, or no way to stop | One move, ending "decelerating hard in the last second and stopping on …" |
| 5 | The end state is too far from the start | A smaller change, or two cuts |
| 6 | Words inside the picture | "No text…", the upper fifth left empty; add words in your editor |
| 7 | Words that tend to be refused | Injuries, red-stained hands, children close to adults, real names, close-up faces — removed |

If a clip already failed, tell it what you saw ("the camera drifted", "people melted", "the water went wild") and it changes the sentence that causes that.

## Install

You need Claude Code (a paid Claude plan, Pro or higher — [plans](https://claude.com/pricing), [download](https://claude.com/download)).

1. Download this repository (green **Code** button → **Download ZIP**) and unzip it.
2. Copy the folder `.claude/skills/flow-prompt-check` into one of these (folders that start with a dot are hidden on a Mac — press Cmd + Shift + . in Finder to show them):
   - `~/.claude/skills/` — to use it in every project, or
   - `<your project>/.claude/skills/` — for one project.
3. Start Claude Code, type `/flow-prompt-check`, and paste your prompt.

Or open this unzipped folder itself in Claude Code; the skill is already in place.

## Example

See [`examples/`](examples/) for a real run: a castle prompt in English and a temple prompt in Japanese, before and after.

## The one-page checklist

The same seven causes as a printable page: [日本語](checklist/flow-checklist-ja.pdf) · [English](checklist/flow-checklist-en.pdf) · [한국어](checklist/flow-checklist-ko.pdf)

## The full method

This skill is one page of a larger method: script frame, cut sheet, reference images, every still and video prompt, edit sheet. Those skills are at **[nabemall.com](https://nabemall.com/)** — Shorts with Google Flow, centuries-long time-lapses of one place, photoreal city time-lapses, fact research for Shorts and long videos, hooks, and every directing prompt we use.

## License

MIT — see [LICENSE](LICENSE).
