# VisiVault 🔮

### A DiegosDevStudio Project

> **Prompt Engineering Powerhouse** — bridge the gap between simple ideas and professional AI generations for Stable Diffusion, Midjourney, and Sora.

-----

## ✨ Features

|Feature                                 |Beginner|Pro|
|----------------------------------------|:------:|:-:|
|Image → Technical Prompt (Vision Tab)   |✅       |✅  |
|5-Scene Storyboard Generator            |✅       |✅  |
|Technical Enhancer Tags (8k, cinematic…)|—       |✅  |
|Editable Negative Prompts               |—       |✅  |
|Final Composed Prompt Builder           |—       |✅  |
|Copy-to-clipboard                       |✅       |✅  |

-----

## 🚀 Quick Start

### Prerequisites

- A modern browser (Chrome, Firefox, Edge, Safari)
- A **Google Gemini API key** (free) — get one at [aistudio.google.com](https://aistudio.google.com/app/apikey)

### Running Locally

```bash
# Clone the repo
git clone https://github.com/DiegosDevStudio/visivault.git
cd visivault

# No build step needed — open index.html directly
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or serve with any static server:

```bash
npx serve .
# or
python -m http.server 8080
```

### First-Time Setup

1. Open the app in your browser.
1. Accept the **Privacy & Consent Modal** (required for Gemini Free Tier).
1. Click the **⚙ Settings** gear icon.
1. Paste your Gemini API key and click **Save Key**.
1. Start creating!

-----

## 🖼 Vision Tab

**Purpose:** Analyze any image and generate a 100-word Technical Prompt optimized for AI image generators.

1. Upload an image (JPEG, PNG, WEBP — max 10 MB) by clicking or drag-and-drop.
1. Click **✦ Analyze Image**.
1. Gemini will return a prompt rich with:
- Lighting descriptors (golden hour, rim light, soft diffused)
- Camera gear (Fujifilm XT4, 35mm f/1.4, Canon 5D)
- Textures and materials
- Composition and color grading
1. **Pro Mode:** Toggle enhancer tags (8k, raw photo, film grain…) and add Negative Prompts, then click **⚡ Build Final Prompt** for a complete, copy-ready generation string.

-----

## 🎬 Storyboard Tab

**Purpose:** Transform a one-line premise into a professional 5-scene AI video brief.

1. Enter your premise in the input box.
1. Click **🎬 Generate Scenes**.
1. Receive 5 structured scenes:
- Scene 1: The Hook
- Scene 2: The Build
- Scene 3: The Turn
- Scene 4: The Climax
- Scene 5: The Resolution
1. Each scene is camera-direction ready for Sora, Runway, or Pika Labs.

-----

## 🔐 Privacy & Security

### Gemini Free Tier Notice

Images submitted via the Gemini Free Tier **may be used by Google** to improve their AI models. Do **not** submit:

- Personally identifiable images (faces, IDs, etc.)
- Confidential or proprietary visuals
- Sensitive medical or financial imagery

### API Key Storage

- Your key is stored in **browser localStorage** only.
- It is **never** transmitted to any server other than Google’s API endpoint.
- We do **not** log, collect, or have access to your API key.
- ⚠️ Do not use VisiVault on shared or public computers without clearing localStorage afterward.

-----

## 🎨 Design & Brand Identity

The VisiVault UI was designed to be a direct visual extension of the **DiegosDevStudio official brand identity**. Every design decision — from color to typography to layout — was intentionally derived from the studio’s established visual language:

- **Color Palette:** The Electric Cyan (`#22D3EE`) to Royal Blue (`#2563EB`) gradient is pulled directly from the official `{D>` logo mark. The deep charcoal/slate background (`#121826`) mirrors the logo’s dark circular field.
- **Logo Integration:** The `{D>` mark — combining a curly brace `{`, a play arrow `>`, and the letter `D` — is recreated as an inline SVG in both the header and footer, faithfully reproducing the cyan-to-royal gradient and glow of the official asset.
- **Glassmorphism UI:** Cards, modals, and input surfaces use `backdrop-filter: blur` with semi-transparent brand-colored backgrounds, giving the interface the same sense of depth and polish as the studio’s visual identity.
- **Typography:** Display text uses **Rajdhani** for its sharp, technical character; UI copy uses **Outfit** for readability; and code/labels use **JetBrains Mono** to reinforce the developer-studio aesthetic.
- **Motion & Detail:** Subtle scanline grid backgrounds, film grain noise overlays, and gradient glow accents all reference the precision and craftsmanship of the DiegosDevStudio brand.

-----

## 🛠 Tech Stack

|Layer   |Technology                                     |
|--------|-----------------------------------------------|
|Frontend|Vanilla HTML5 / CSS3 / JavaScript (ES2022)     |
|AI      |Google Gemini 1.5 Flash API                    |
|Fonts   |Rajdhani, Outfit, JetBrains Mono (Google Fonts)|
|Hosting |Any static host (GitHub Pages, Netlify, Vercel)|

Zero dependencies. No build step. One file.

-----

## 📁 Project Structure

```
visivault/
├── index.html          # Main application (all-in-one)
├── README.md           # This file
├── CONTRIBUTING.md     # Contribution guidelines
└── LICENSE             # MIT License
```

-----

## 🌐 Deployment

### GitHub Pages

```bash
git init
git add .
git commit -m "feat: initial VisiVault release"
git remote add origin https://github.com/DiegosDevStudio/visivault.git
git push -u origin main
# Enable Pages in repo Settings → Pages → main branch
```

### Netlify / Vercel

Drag and drop the project folder into the Netlify or Vercel dashboard. Done.

-----

## 📄 License

MIT — see <LICENSE> for details.

-----

## 🤝 Contributing

See <CONTRIBUTING.md> for how to get involved.

-----

<div align="center">

Made with ♥ by **DiegosDevStudio**

</div>
