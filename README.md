# Shape Color Quest ⭐

A friendly, big-tap learning game for **3–6 year olds**: shapes, colors, counting, listening, memory and careful looking.

**Play online:** https://khvr1993.github.io/shape-color-quest/

## Modes

| Mode | What the child does |
| --- | --- |
| 🔺 **Shapes** | Hears “Find the triangle” and taps the matching shape. Later: “Find 2 circles and 1 star”. |
| 🎨 **Colors** | Hears “Find something red”, then “Find 2 red things and 1 blue thing”. |
| ✨ **Shapes + Colors** | Hears “Find the red star” and must match both attributes. From level 7 the color **word** may be printed in a different color (Stroop-style). |
| 🧠 **Memory** | Flips cards and matches pairs of identical shape-and-color cards (3 → 8 pairs). |
| ⚡ **Tricky** | Mixed challenges: sneaky color words, “find the picture that is NOT a shape”, and category hunts like “find the fruit”. |

## Fifteen levels

Pick a **start level** on the start screen (1–15); the choice is remembered on the device, so a child who is comfortable at level 8 can jump straight in instead of starting at 1.

After that, difficulty adapts to **recent answers**: about three correct answers move the child up a level; a couple of mistakes move them back. Level-ups are announced with a toast, and the current level appears under the board and in the round summary.

| Levels | Board | Task |
| --- | --- | --- |
| 1–3 | 4–6 tiles | find one shape/color |
| 4–6 | 7–8 tiles | distractors share the target's color or shape |
| 7 | 8 tiles | tricky color words appear |
| 8–9 | 8 tiles | **counting**: find 2 of something |
| 10 | 10 tiles | counting with stronger distractors |
| 11–12 | 10 tiles | **two groups**: find 2 of X and 1 of Y |
| 13 | 12 tiles | two groups on a big jumbled board |
| 14–15 | 12 tiles | **3 of X and 1 of Y**, strongest distractors |

Levels 8–15 add a **collection tray** under the prompt: each target has slots, and tapping a matching shape fills the next slot with a star. Tapped shapes stay on the board marked with a green ring. The task completes only when every slot is filled — so the child has to keep count.

Boards are laid out on a grid but every tile gets a small random rotation and offset, so the higher levels look like a jumbled pile of shapes rather than a neat table.

## Why tap-to-collect instead of drag-and-drop

Dragging is fiddly for a 5-year-old's finger and easy to cancel by accident. Tapping a shape and watching it fill a slot in the tray gives the same "put it in the basket" goal, with bigger, more reliable touch targets — and the tray is a visual, pre-reading way to show how many are still needed.

## Polish

- **Start screen** with a level picker and mode picker.
- **Pause** (⏸️ or `Esc`) with resume, restart-round and home.
- **Round summary** after every 8 questions (one memory board): stars, first-try accuracy, best streak and current level.
- Praise, confetti, stars, streak bonus and a sticker every 5 stars. Wrong taps never punish — they wiggle, the prompt is repeated, and the board stays open.
- Sound and voice toggles. Voice uses the device's text-to-speech.

## Run it

Open `index.html` in any browser — no build step, no dependencies, works offline on a tablet or phone.

## Tech

Single self-contained `index.html`: HTML, CSS, vanilla JS, inline SVG shapes, Web Audio sound effects and SpeechSynthesis for the spoken prompts. Boards are generated with an exact-count guarantee (no ambiguous answers); the start level is stored in `localStorage`.
