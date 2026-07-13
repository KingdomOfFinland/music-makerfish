# music-makerfish 🐟🔊
 
A bytebeat / floatbeat synthesis terminal, built as a companion tool to [Fish Engine](https://kingdomoffinland.github.io/Simple-Engine/).
 
Live formula editor, oscilloscope, preset library, and WAV export — all in a single HTML file, zero dependencies, runs entirely in your browser via the Web Audio API.
 
## What's bytebeat?
 
Bytebeat is a style of algorithmic music where a tiny formula — using only an ever-increasing integer counter `t` and bitwise operators (`& | ^ >> <<`) — generates 8-bit audio. Each sample is `formula(t) & 255`. The genre kicked off around 2011 on viznut's blog and spread through demoscene circles: one line of C-like code can produce surprisingly musical, glitchy, rhythmic noise.
 
**Floatbeat** is the smoother cousin — same idea, but the formula outputs a float (using `sin()`, normal arithmetic, etc.) instead of doing integer bit tricks.
 
## Features
 
- 🖥️ Live formula editor (bytebeat + floatbeat modes)
- 📊 Real-time oscilloscope
- 🎛️ Sample rate slider (4000–48000 Hz)
- 📼 12 built-in presets (classics + originals)
- 🇬🇧 🇫🇮 English / Finnish UI
- ⬇️ Export to WAV
- No build step, no dependencies, no server — just open `index.html`
## Usage
 
Open `index.html` in any modern browser, or visit the [GitHub Pages link](https://kingdomoffinland.github.io/music-makerfish/) once Pages is enabled.
 
Type a formula, hit play. Examples:
 
```
(t*(t>>10|t>>8))&255        // classic bytebeat
Math.sin(t*0.02)*0.5        // floatbeat sine drone
```
 
## Part of the Fish Engine family
 
- [Fish Engine](https://github.com/KingdomOfFinland/Simple-Engine) — arcade hub (Pong, Pac-Man, Pinball, and more)
- music-makerfish — this repo
Built by Valkeakoski Engineering.
