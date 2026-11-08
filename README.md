# Shape Color Quest ⭐

A friendly, big-tap learning game for **3–6 year olds**: shapes, colors, listening, memory and careful looking.

**Play online:** https://khvr1993.github.io/shape-color-quest/

## Modes

| Mode | What the child does |
| --- | --- |
| 🔺 **Shapes** | Hears “Find the triangle” and taps the matching shape. |
| 🎨 **Colors** | Hears “Find something red” and taps something of that colour. |
| ✨ **Shapes + Colors** | Hears “Find the red star” and must match both attributes. |
| 🧠 **Memory** | Flips cards and matches pairs of identical shape-and-colour cards. |
| ⚡ **Tricky** | Mixed challenges: a colour word printed in a *different* colour (Stroop-style), “find the picture that is NOT a shape”, and category hunts like “find the fruit”. |

## Adaptive difficulty

Difficulty is based on **recent answers**, not the round number. Correct taps push it up, mistakes push it down:

- **Number of choices** grows from 4 → 6 → 8 tiles (memory: 3 → 6 pairs).
- **Distractor similarity** changes: at first everyone differs in both shape and colour, later tiles share the target's colour or shape, so the child has to look carefully.
- The tricky colour-word effect switches on in Shapes + Colors once the child is doing well.
- The small label under the board shows the current level (🐣 Gentle / 🌱 Growing / 🚀 Tricky).

## Polish

- **Start screen** with a mode picker.
- **Pause** button (also `Esc`) with resume, restart-round and home.
- **Round summary** after every 8 questions (one memory board) showing stars, first-try accuracy and best streak.
- Praise, confetti, stars, streak bonus and a sticker every 5 stars. Wrong taps never punish — they wiggle, the prompt is repeated, and the board stays open.
- Sound and voice toggles; voice uses the device's text-to-speech.

## Run it

Open `index.html` in any browser — no build step, no dependencies, works offline on a tablet or phone.

## Tech

Single self-contained `index.html`: HTML, CSS, vanilla JS, inline SVG shapes, Web Audio sound effects and SpeechSynthesis for the spoken prompts.
