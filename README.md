<p align="center">
  <img src="docs/assets/socialbanner.png" width="100%" alt="AetherForge Banner" />
</p>

# AetherForge — Elite frontend design suite for Gemini CLI

**Forces bold, non-generic, production-grade UIs. No more AI slop.**

AetherForge is a multi-aesthetic design suite that intercepts your frontend prompts and upgrades them with striking typography, intentional motion, and distinctive personality.

### What it does
Whenever you ask Gemini to build any UI (landing page, dashboard, component, app, etc.), **AetherForge** automatically activates. It uses a **Hybrid Selection Logic** to determine the best style for your project:
1.  **Keyword Matching**: Mention "brutalist," "clean," or "retro" to trigger a specific system.
2.  **Intent Inference**: It guesses the vibe based on your project (e.g., "admin dashboard" → SaaS).
3.  **The Vibe Picker**: If the direction is blurred, Gemini will stop and ask you to choose your aesthetic.

### 🌌 The Design Systems

| **Style** | **The Vibe** | **Best For...** |
| :--- | :--- | :--- |
| **Elite** | Refined, creative, unique. The "Golden Standard." | Brand landing pages, creative portfolios. |
| **Brutalist** | Raw, industrial, high-contrast, visible structures. | Experimental apps, "honest" utility tools. |
| **SaaS** | Clean, professional, whitespace-heavy, startup-ready. | Dashboards, Settings panels, B2B tools. |
| **Retro** | Dark mode, monospaced, cyberpunk, terminal-style. | Dev tools, hacker consoles, tech portfolios. |

*(Comparison screenshots coming soon!)*

### One-command install
```bash
gemini extensions install https://github.com/sudoax0n/aetherforge
```

### Update
```bash
gemini extensions update aetherforge
```

### 🔥 Pro-Level Prompts
Try these prompts to see the different systems in action. These are tuned to get the absolute best out of the AetherForge engine:

#### 🏛️ Elite & Creative
- *"Build an editorial-style landing page for a high-end architecture firm. Focus on massive serif typography and grid-breaking layouts."*
- *"Design a creative portfolio homepage for a motion designer. Use a bold, asymmetrical layout with staggered entrance animations."*

#### 🏗️ Brutalist & Raw
- *"Build a raw, brutalist dashboard for monitoring server health. Use thick borders, safety orange accents, and visible grid lines."*
- *"Create a brutalist 'links' page for my social media. Use high-contrast black and white with industrial-style typography."*

#### 💼 SaaS & Professional
- *"Build a clean, minimalist SaaS dashboard for a project management tool. Focus on generous whitespace, subtle 1px shadows, and a professional indigo accent."*
- *"Design a professional settings panel for a cloud platform. Keep it efficient, whitespace-heavy, and use a refined 'Inter' or 'Geist' vibe."*

#### 📟 Retro & Cyberpunk
- *"Build a retro-futuristic hacker console for a security toolkit. Use dark mode, phosphor green monospaced text, and a subtle scanline overlay."*
- *"Create a terminal-inspired landing page for a CLI tool. Use neon cyan accents on a deep black background with industrial brackets for borders."*

### How to test it locally
```bash
gemini extensions link .
```

### Troubleshooting

If the extension is not found or fails to activate in certain directories, check the following:

- **Safe Mode:** Gemini CLI may restrict extension execution in untrusted folders. Run `gemini trust` to enable all extension features.
- **Global Scope:** Ensure the extension is enabled at the user level to be available across all projects:
  ```bash
  gemini extensions enable aetherforge --scope user
  ```

---

**Made by [@sudoax0n](https://x.com/beyondwudan)**  
*Star ⭐ if you’re tired of generic AI UIs.*
