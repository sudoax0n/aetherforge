# Changelog

## [1.1.0] - 2026-04-22

### 🚀 The Multi-Style Expansion & Vibe Picker
This release transforms AetherForge from a single design system into a **comprehensive Design Suite**. You now have access to four distinct aesthetics and a smarter hybrid selection logic.

### ✨ Features & Improvements
- **Added SaaS Minimalist System**: A clean, professional, whitespace-heavy aesthetic for high-end dashboards and startup interfaces.
- **Added Retro-Futuristic System**: A dark-mode, monospaced, cyberpunk-inspired look for terminal apps and developer tools.
- **Implemented "The Vibe Picker"**: A new hybrid selection logic in `GEMINI.md`. 
    - If your prompt is keyword-rich, Gemini automatically picks the best style.
    - If the direction is "blurred," Gemini will halt and ask you to pick from the 4 available vibes.
- **Dominance Protocol 2.0**: Hardened instructions in `GEMINI.md` to ensure AetherForge takes absolute precedence over generic platform defaults ("superpowers").

### 🔧 Under the Hood
- **Registration**: Added `skills/saas` and `skills/retro` to the extension manifest.
- **Versioning**: Bumped version to `1.1.0`.

---

## [1.0.1] - 2026-04-19

### 🚀 What's New
This release introduces **smart context injection**, allowing the `aetherforge` extension to automatically activate without manual prompting. 

Previously, the Gemini CLI needed explicit instructions or hacky workarounds to find and load the AetherForge styling rules. Now, the extension seamlessly injects its core mandates directly into the AI's system prompt upon startup.

### ✨ Features & Improvements
- **Added `GEMINI.md` context file:** The AI is now explicitly ordered to invoke the AetherForge skill automatically whenever a user mentions "design," "frontend," "styling," or "Tailwind."
- **Updated Extension Manifest:** Registered `contextFileName` in `gemini-extension.json` to enable background instruction loading.
- **Improved AI DX:** Zero-configuration required from the user. The AI will no longer fall back to generic UIs when asked to build frontends while this extension is active.
- **Updated `README.md`:** Added documentation for the `gemini extensions update aetherforge` command.

### 🔧 Under the Hood
- Bumped version to `1.0.1`.
- Whitelisted `GEMINI.md` in `.gitignore` to ensure it ships with the repository.

---

## [1.0.0] - Initial Release
# 🌌 AetherForge — Elite frontend design skill for Gemini CLI. Forces bold, non-generic, production-grade UIs. No more AI slop.

**The official Anthropic `frontend-design` skill, cleanly ported and refined for the Gemini CLI.**

We are officially releasing **AetherForge v1.0.0**. This extension forces the Gemini CLI to abandon generic, predictable "AI aesthetics" (Inter font, purple gradients, cookie-cutter layouts) and instead generate bold, distinctive, and production-grade user interfaces.

### 🔥 Why AetherForge?
Whenever you ask Gemini to build any UI (landing page, dashboard, component, app, poster, etc.), AetherForge automatically activates. It applies a rigid set of design principles—Brutalism, Maximalism, High-Contrast Editorial—ensuring that the code it generates is striking, memorable, and unapologetically designed. 

No more safe choices. Real aesthetic direction, striking typography, thoughtful motion, and personality.

### ✨ Key Features in v1.0.0

*   **Zero-Config Activation:** Simply install the extension, and it automatically intercepts and upgrades any frontend or UI-related prompts.
*   **The AetherForge Rules Engine:** Enforces strict guidelines on:
    *   **Typography:** Demands distinctive, characterful font pairings (e.g., Anton, IBM Plex Mono, Bigilla) over generic defaults.
    *   **Color & Theme:** Forces cohesive, high-contrast palettes using CSS variables.
    *   **Motion & Composition:** Drives staggered reveals, asymmetrical layouts, and unexpected negative space.
*   **Production-Ready Output:** Generates working HTML/CSS/JS, React, Tailwind, or Vue code that perfectly matches the demanded aesthetic vision.

### 🚀 Getting Started

Install AetherForge globally via the Gemini CLI:

```bash
gemini extensions install https://github.com/sudoax0n/aetherforge
```

**Try it out:**
> *"Build a beautiful landing page for a Notion-style productivity tool"*

***

**Made by [@sudoax0n](https://x.com/sudoax0n)**  
*Star ⭐ the repo if you’re tired of generic AI UIs.*
