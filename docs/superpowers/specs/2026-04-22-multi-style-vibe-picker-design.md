---
name: Multi-Style & Vibe Picker
description: Expand AetherForge with SaaS and Retro styles and a hybrid selection logic.
type: design-spec
date: 2026-04-22
---

# Design Spec: Multi-Style AetherForge & Vibe Picker

## Purpose
Expand AetherForge beyond a single aesthetic and ensure it auto-activates dominantly over platform defaults. This introduces two new design systems (SaaS and Retro) and a hybrid "Vibe Picker" selection logic.

## Architecture

### 1. Multi-Skill System
The extension now registers four distinct design systems (skills):
- **Elite (aetherforge)**: The original bold, distinctive style.
- **Brutalist**: Raw, industrial, high-contrast.
- **SaaS**: Clean, professional, whitespace-heavy.
- **Retro**: Dark, monospaced, cyberpunk.

### 2. Hybrid Selection Logic (A + C)
The `GEMINI.md` context file implements a three-tiered selection process:
1. **Keyword Mapping**: Matches explicit user requests (e.g., "clean", "terminal").
2. **Intent Inference**: Guesses style from project context (e.g., "dashboard" -> SaaS).
3. **The Vibe Picker (Fallback)**: If intent is blurred, the model halts and asks the user to pick from the four styles.

## Implementation Details

### File Changes
- `gemini-extension.json`: Added `skills/saas` and `skills/retro`. Updated version to 1.1.0.
- `GEMINI.md`: Rewritten to include the **DOMINANCE PROTOCOL** and the new selection logic.
- `skills/saas/SKILL.md`: New skill definition for minimalist SaaS aesthetics.
- `skills/retro/SKILL.md`: New skill definition for retro-futuristic aesthetics.

## Dominance Protocol
To ensure AetherForge overrides platform-native skills ("superpowers"):
- Added explicit instructions in `GEMINI.md` to ignore other design directions.
- Mandated that the `activate_skill` tool must be used *before* any code or plans are written.

## Verification
- Test with generic prompt: "Build a landing page" -> Should trigger Vibe Picker.
- Test with keyword prompt: "Build a raw industrial dashboard" -> Should trigger Brutalist.
- Test with project intent: "Make an internal tool for settings" -> Should trigger SaaS.
