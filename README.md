# Animated SVG Badges for GitHub Profile

[日本語](./README.ja.md) | English

A collection of lightweight, dependency-free animated SVG badges for your GitHub Profile README.
Pure SVG + CSS/SMIL. No external servers, no images, no JavaScript.

---

## 🖼️ Gallery

### 💥 Explosion — `explosion.svg`
![Explosion](./explosion.svg)

### 👾 Cyberpunk Glitch — `glitch.svg`
Jerky left-right text jitter, red/cyan RGB split, and a laser scanline sweeping across a futuristic frame.

![Glitch](./glitch.svg)

### 🌃 Neon Sign — `neon.svg`
A white-hot core, a soft surrounding glow, and irregular real-neon flickering.

![Neon](./neon.svg)

---

## ✨ Features

- 🚀 **Zero External Dependencies**: Pure inline SVG. No server downtime risks.
- 🎞️ **Works as `<img>` on GitHub**: Animations run inside the README.
- 🎨 **Easy to Customize**: Change text and colors directly in the SVG file.

---

## 🚀 Quick Start

### 1. Download the SVG

Pick the badge you like from this repository and upload it to your own Profile Repository (e.g., `your-username/your-username`).

### 2. Add to Your README.md

```html
<div align="center">
  <img src="./glitch.svg" width="100%" alt="Glitch Badge" />
</div>
```

Replace `glitch.svg` with `neon.svg` or `explosion.svg` as you like.

> ⚠️ Pasting the SVG code directly into the README will not work. Always reference it with `<img>` or `![](...)`.

---

## 🎨 Customization

### Change the Text

| File | Where to edit |
| --- | --- |
| `glitch.svg` | The `<text id="t">` element inside `<defs>` (default: `CYBER GLITCH`) |
| `neon.svg` | The `<text id="t">` element inside `<defs>` (default: `NEON SIGN`) |
| `explosion.svg` | Replace `YOUR_NAME` in the `<text>` tag near the bottom |

If your text is longer, reduce `font-size` on the same `<text>` element.

### Change the Colors

**glitch.svg**
- Red layer: `#ff1744`
- Cyan layer / laser: `#00e5ff`, `#9ffcff`
- Background: `#14052b`, `#05010d`

**neon.svg**
- Main text glow: `#ff2e93`, `#ff4fa8`, `#ff7cc0`
- Frame: `#00e5ff`, `#33ecff`
- Background: `#1b0a24`, `#07030b`

For `neon.svg`, if you change the text, also adjust `x` and `width` of `<clipPath id="partClip">` so the "flickering part" matches the letters you want.

### Adjust Animation Speed

Edit the durations in the `<style>` section (e.g. `2.4s`, `5.3s`). Odd, uneven numbers look more natural.

---

## 📝 Notes

- Fonts depend on the viewer's OS (system fonts only), so letter widths may differ slightly.
- Animations may be reduced if the viewer has "reduce motion" enabled.

---

## ⭐️ Show Your Support

If you found this useful, please consider giving this repository a **Star** ⭐️!