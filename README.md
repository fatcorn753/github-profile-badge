#  Animated Explosion Badge for GitHub Profile

[日本語](/README.ja.md) | English

A lightweight, dependency-free SVG animation that brings an explosive entrance to your GitHub Profile README!

![Demo](./explosion.svg)

---

## ✨ Features

- 🚀 **Zero External Dependencies**: Works purely with inline SMIL SVG. No external server downtime risks.
- 🔁 **Smooth Infinite Loop**: Configured specifically to bypass GitHub Camo proxy caching issues.
- 🎨 **Easy to Customize**: Easily change text, colors, and animation speed directly within the SVG file.

---

## 🚀 Quick Start (How to Use)

### 1. Download the SVG
Download [`explosion.svg`](./explosion.svg) from this repository and upload it to your own Profile Repository (e.g., `your-username/your-username`).

### 2. Customize Your Name / Text
Open the uploaded `explosion.svg` in any text editor, locate the `<text>` tag near the bottom, and replace `YOUR_NAME` with your GitHub username or custom text:

```xml
<!-- explosion.svg -->
<text x="0" y="0" dominant-baseline="central" text-anchor="middle" class="main-text">
  YOUR_NAME <!-- 👈 Change this to your username -->
</text>
```

### 3. Add to Your README.md
Paste the following HTML code into your profile `README.md`:

```html
<div align="center">
  <img src="./explosion.svg" width="100%" alt="Explosion Badge" />
</div>
```

---

## 🎨 Customization Tips

### Change Colors
You can edit the particle and shockwave colors inside `explosion.svg`:

- **Background**: Change `fill: #0d1117;` inside `.bg`
- **Text Color**: Change `fill: #ffffff;` inside `.main-text`
- **Shockwave**: Change `stroke: #00f0ff;` inside `.shockwave-color`
- **Particles**: Modify the `fill` attributes on the `<circle>` elements

### Adjust Text Size
If your username is longer, reduce the font size in the `<style>` section:

```css
.main-text {
  font-size: 28px; /* Adjust as needed */
}
```

---

## ⭐️ Show Your Support

If you found this useful, please consider giving this repository a **Star** ⭐️!