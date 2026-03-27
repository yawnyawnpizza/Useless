# 🎲 Fidget Cube

A fully interactive, completely useless fidget cube built in a single HTML file.

No dependencies. No frameworks. No purpose.

---

# 🚀 Usage

You have two choices!

1. Go to https://yawnyawnpizza.github.io/Useless
2. Download the source code and run 'index.html' 

```
open fidget_cube.html
```

No server. No install. No build step. Just vibes.

---

# 🎨 The Six Faces

# 🩷 Pink — Bubble Wrap
20 poppable bubbles with realistic plastic snap sounds. Each bubble has its own pitch. Hit **refill** to do it again forever.

# 🔵 Blue — Big Button
A big red button with **100 unique messages** that get increasingly unhinged the more you click. Milestone badges pop up at 10, 25, 50, 75, and 100.

# 🟠 Orange — Useless Sliders
Four sliders: vibe level, pizza desire, chaos energy, and productivity (starts at 2%). None of them affect anything.

# 🟣 Purple — Mystery Toggles
Five toggles including "Reverse time" and "Do the thing." All of them do nothing.

# 🟢 Green — Spin Dial
A spinner that lands on one of eight outcomes including *meh* and *???*. Plays satisfying ratchet click sounds as it spins and slows down.

# 🟡 Yellow — Clicky Keys
12 mechanical-style keyboard keys, each with a unique synthesized click and thud sound profile.

---

# ✨ Features

- **Drag to rotate** — click and drag anywhere to spin the cube in 3D
- **Idle auto-spin** — cube slowly drifts on load and stops the moment you grab it
- **All sounds synthesized** — Web Audio API only, zero audio files
- **Per-bubble pitch** — each bubble snap is tuned differently
- **Per-key sound profiles** — each key has its own click frequency, decay, and body tone
- **Ratchet dial ticks** — tick volume scales with spin speed, louder as it slows

---

# 🛠️ Technical Notes

- Single `.html` file — everything is self-contained
- 3D cube via CSS `transform-style: preserve-3d` with six absolutely-positioned faces
- `will-change: transform` + `backface-visibility: hidden` on every face for crisp GPU rendering
- Slider touch/mouse events block propagation so dragging them doesn't rotate the cube
- All audio built with Web Audio API buffers and biquad filters — no `.mp3` or `.wav`

---

# 🌐 Browser Support

Any browser with Web Audio API and CSS 3D transform support — basically everything since 2015.
